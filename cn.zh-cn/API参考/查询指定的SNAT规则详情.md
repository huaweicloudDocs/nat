# 查询指定的SNAT规则详情<a name="ZH-CN_TOPIC_0130808158"></a>

## 功能介绍<a name="section59567946"></a>

查询指定的SNAT规则详情。

## URI<a name="section66349468"></a>

GET /v2.0/snat\_rules/\{snat\_rule\_id\}

**表 1**  参数说明

<a name="table1910716134591"></a>
<table><thead align="left"><tr id="row3169413135915"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p16169131375910"><a name="p16169131375910"></a><a name="p16169131375910"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="19%" id="mcps1.2.5.1.2"><p id="p1716915133591"><a name="p1716915133591"></a><a name="p1716915133591"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="p151699135593"><a name="p151699135593"></a><a name="p151699135593"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="35%" id="mcps1.2.5.1.4"><p id="p016991320594"><a name="p016991320594"></a><a name="p016991320594"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row131691913145916"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p116919133595"><a name="p116919133595"></a><a name="p116919133595"></a>snat_rule_id</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.5.1.2 "><p id="p101695138597"><a name="p101695138597"></a><a name="p101695138597"></a>Uuid-Str</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p6169171310597"><a name="p6169171310597"></a><a name="p6169171310597"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><p id="p31691313145913"><a name="p31691313145913"></a><a name="p31691313145913"></a>所属SNAT规则的id。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section5597798"></a>

无

## 响应消息<a name="section50380184"></a>

响应参数如[表2](#table65459315)所示。

**表 2**  响应参数

<a name="table65459315"></a>
<table><thead align="left"><tr id="row47811128"><th class="cellrowborder" valign="top" width="20.73%" id="mcps1.2.4.1.1"><p id="p47496137"><a name="p47496137"></a><a name="p47496137"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="28.050000000000004%" id="mcps1.2.4.1.2"><p id="p21981920"><a name="p21981920"></a><a name="p21981920"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p6428601"><a name="p6428601"></a><a name="p6428601"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row50954701"><td class="cellrowborder" valign="top" width="20.73%" headers="mcps1.2.4.1.1 "><p id="p33690117"><a name="p33690117"></a><a name="p33690117"></a>snat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="28.050000000000004%" headers="mcps1.2.4.1.2 "><p id="p44544970"><a name="p44544970"></a><a name="p44544970"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p447513"><a name="p447513"></a><a name="p447513"></a>snat_rule对象。</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section50768476"></a>

-   请求样例

    ```
    GET /v2.0/snat_rules/5b95c675-69c2-4656-ba06-58ff72e1d338
    ```


-   响应样例

    ```
    {
        "snat_rule": {
            "floating_ip_id": "bdc10a4c-d81a-41ec-adf7-de857f7c812a",
            "status": "ACTIVE",
            "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
            "admin_state_up": true,
            "network_id": "eaad9cd6-2372-4be1-9535-9bd37210ae7b",
            "cidr": "",
            "source_type":0,
            "tenant_id": "27e25061336f4af590faeabeb7fcd9a3",
            "created_at": "2017-11-18 07:54:21.665430",
            "id": "5b95c675-69c2-4656-ba06-58ff72e1d338",
            "floating_ip_address": "5.21.11.226"
        }
    }
    ```


## 返回值<a name="section1941962013172"></a>

请参见[通用请求返回值](通用请求返回值.md)。

