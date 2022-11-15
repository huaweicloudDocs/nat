# 示例1：创建公网NAT网关并配置SNAT规则<a name="nat_demo_0001"></a>

## 场景描述<a name="section127254112211"></a>

本章节指导用户通过调用API来创建SNAT规则。API的调用方法请参见[如何调用API](https://support.huaweicloud.com/api-natgateway/nat_api_0053.html)。

## 前提条件<a name="section688710355615"></a>

-   已创建VPC和子网，具体参见[创建云服务器所需要的VPC和子网](https://support.huaweicloud.com/api-vpc/vpc_apieg_0002.html)。
-   确认VPC下没有默认路由\(“华北-北京四”区域无此限制\)。
-   创建规则时，要求网关状态status = "ACTIVE"，要求网关管理员状态admin\_state\_up = True。
-   当您使用Token认证方式完成认证鉴权时，需要获取用户Token并在调用接口时增加“X-Auth-Token”到业务接口请求消息头中。Token认证，具体操作请参考[认证鉴权](https://support.huaweicloud.com/api-natgateway/nat_api_0056.html)。

>![](public_sys-resources/icon-note.gif) **说明：** 
>通过IAM服务获取到的Token有效期为24小时，需要使用同一个Token鉴权时，可以先将Token缓存，避免频繁调用。

## 操作步骤<a name="section124721712715"></a>

1.  预置NAT网关。
    1.  确定所用的VPC。
        -   查询VPC列表

            URI格式：GET /v1/\{project\_id\}/vpcs

            详情请参见[查询VPC列表](https://support.huaweicloud.com/api-vpc/vpc_api01_0003.html)。

        -   根据实际需要选择VPC并确认VPC下没有默认路由，然后记录VPC的id。

    2.  确定所用VPC下的子网。
        -   查询所用的VPC下的子网列表

            URI格式：GET /v1/\{project\_id\}/subnets?vpc\_id=\{vpc\_id\}

            详情请参见[查询子网列表](https://support.huaweicloud.com/api-vpc/vpc_subnet01_0003.html)。

        -   根据实际需要选择子网，并记录子网的id。

    3.  创建公网NAT网关。

        -   接口相关信息

            URI格式：POST /v2/\{project\_id\}/nat\_gateways

            详情请参见[创建公网NAT网关](https://support.huaweicloud.com/api-natgateway/CreateNatGateway.html)。

        -   请求示例

            POST https://\{Endpoint\}/v2/27e25061336f4af590faeabeb7fcd9a3/nat\_gateways

            \{endpoint\}信息请从[地区和终端节点](https://developer.huaweicloud.com/endpoint?NAT)获取。

        -   响应示例

        ```
        {
            "nat_gateway": {
                "name": "nat_001",
                "description": "my nat gateway 01",
                "router_id": "d84f345c-80a1-4fa2-a39c-d0d397c3f09a",
                "internal_network_id": "89d66639-aacb-4929-969d-07080b0f9fd9",
                "spec": "1",
                "enterprise_project_id": "0aad99bc-f5f6-4f78-8404-c598d76b0ed2"
            }
        }
        ```

    4.  确定公网NAT网关创建成功，并且网关状态为active。

        接口相关信息

        URI格式：GET /v2/\{project\_id\}/nat\_gateways/\{nat\_gateway\_id\}

        详情请参见[查询指定的公网NAT网关详情](https://support.huaweicloud.com/api-natgateway/ShowNatGateway.html)。

    5.  记录新创建的NAT网关的id和对应的internal\_network\_id。

2.  确定待使用的弹性公网IP。
    1.  查询弹性公网IP资源。

        接口相关信息

        URI格式：GET /v1/\{project\_id\}/publicips

        详情请参见[查询弹性公网IP列表](https://support.huaweicloud.com/api-eip/eip_api_0003.html)。

    2.  根据实际需要选择弹性EIP，并记录弹性EIP的id。

3.  创建SNAT规则。
    -   接口相关信息

        URI格式: POST /v2/\{project\_id\}/snat\_rules

        接口约束及请求参数说明详情，请参见[创建SNAT规则](https://support.huaweicloud.com/api-natgateway/CreateNatGatewaySnatRule.html)。

    -   请求示例

        POST https://\{Endpoint\}/v2/27e25061336f4af590faeabeb7fcd9a3/snat\_rules

        \{endpoint\}信息请从[地区和终端节点](https://developer.huaweicloud.com/endpoint?NAT)获取。

        Body:

        ```
        {
            "snat_rule": {
                "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
                "network_id": "eaad9cd6-2372-4be1-9535-9bd37210ae7b",
                "source_type": 0,
                "floating_ip_id": "bdc10a4c-d81a-41ec-adf7-de857f7c812a",
                "description": "my snat rule 01"
            }
        }
        ```

    -   响应示例

        ```
        {
            "snat_rule": {
                "floating_ip_id": "bdc10a4c-d81a-41ec-adf7-de857f7c812a",
                "status": "PENDING_CREATE",
                "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
                "admin_state_up": true,
                "network_id": "eaad9cd6-2372-4be1-9535-9bd37210ae7b",
                "description": "",
                "source_type": 0,
                "tenant_id": "27e25061336f4af590faeabeb7fcd9a3",
                "created_at": "2017-11-18 07:54:21.665430",
                "id": "5b95c675-69c2-4656-ba06-58ff72e1d338",
                "floating_ip_address": "5.21.11.226"
            }
        }
        ```

4.  确认SNAT规则创建成功。
    -   接口相关信息

        URI格式: GET /v2/\{project\_id\}/snat\_rules/\{snat\_rule\_id\}

        详情请参见[查询指定的SNAT规则详情](https://support.huaweicloud.com/api-natgateway/ShowNatGatewaySnatRule.html)。

    -   请求示例

        GET https://\{Endpoint\}/v2/27e25061336f4af590faeabeb7fcd9a3/snat\_rules/5b95c675-69c2-4656-ba06-58ff72e1d338

        \{endpoint\}信息请从[地区和终端节点](https://developer.huaweicloud.com/endpoint?NAT)获取。

    -   响应示例

        ```
        {
            "snat_rule": {
                "floating_ip_id": "bdc10a4c-d81a-41ec-adf7-de857f7c812a",
                "status": "ACTIVE",
                "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
                "admin_state_up": true,
                "network_id": "eaad9cd6-2372-4be1-9535-9bd37210ae7b",
                "source_type": 0,
                "tenant_id": "27e25061336f4af590faeabeb7fcd9a3",
                "created_at": "2017-11-18 07:54:21.665430",
                "id": "5b95c675-69c2-4656-ba06-58ff72e1d338",
                "floating_ip_address": "5.21.11.226",
                "freezed_ip_address": "",
                "description": "my snat rule 01"
            }
        }
        ```



