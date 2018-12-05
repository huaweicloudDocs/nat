# 查询SNAT规则列表<a name="ZH-CN_TOPIC_0130808190"></a>

## 功能介绍<a name="section3132024"></a>

查询SNAT规则列表。

## URI<a name="section28188224"></a>

GET /v2.0/snat\_rules?id=\{id\}&tenant\_id=\{tenant\_id\}&nat\_gateway\_id=\{nat\_gateway\_id\}&network\_id=\{network\_id\}&floating\_ip\_id=\{floating\_ip\_id\}&floating\_ip\_address=\{floating\_ip\_address\}&status=\{status\}&created\_at=\{created\_at\}&Admin\_state\_up=\{Admin\_state\_up\}&cidr=\{cidr\}&source\_type=\{source\_type\}

## 请求消息<a name="section1544804"></a>

无

## 响应消息<a name="section13903243"></a>

响应参数如[表1](#table25574495)所示。

**表 1**  响应参数

<a name="table25574495"></a>
<table><thead align="left"><tr id="row6316572"><th class="cellrowborder" valign="top" width="20.73%" id="mcps1.2.4.1.1"><p id="p41880308"><a name="p41880308"></a><a name="p41880308"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="28.050000000000004%" id="mcps1.2.4.1.2"><p id="p36861764"><a name="p36861764"></a><a name="p36861764"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p56800622"><a name="p56800622"></a><a name="p56800622"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row37447704"><td class="cellrowborder" valign="top" width="20.73%" headers="mcps1.2.4.1.1 "><p id="p13365211"><a name="p13365211"></a><a name="p13365211"></a>snat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="28.050000000000004%" headers="mcps1.2.4.1.2 "><p id="p8840286"><a name="p8840286"></a><a name="p8840286"></a>List(snat_rule)</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p19058885"><a name="p19058885"></a><a name="p19058885"></a>snat_rule对象列表。</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section58020329"></a>

-   请求样例

    ```
    GET /v2.0/snat_rules
    ```


-   响应样例

    ```
    {
        "snat_rules": [
          {
                "floating_ip_id": "bf99c679-9f41-4dac-8513-9c9228e713e1",
                "status": "ACTIVE",
                "nat_gateway_id": "cda3a125-2406-456c-a11f-598e10578541",
                "admin_state_up": true,
                "network_id": "9a469561-daac-4c94-88f5-39366e5ea193",
                "cidr": "",
                "source_type":0,
                "tenant_id": "abc",
                "created_at": "2017-11-15 15:44:42.595173",
                "id": "79195d50-0271-41f1-bded-4c089b2502ff",
                "floating_ip_address": "5.21.11.242"
            },
            {
                "floating_ip_id": "6e496fba-abe9-4f5e-9406-2ad8c809ac8c",
                "status": "ACTIVE",
                "nat_gateway_id": "e824f1b4-4290-4ebc-8322-cfff370dbd1e",
                "admin_state_up": true,
                "network_id": "97e89905-f9c8-4ae3-9856-392b0b2fbe7f",
                "cidr": "",
                "source_type":0,
                "tenant_id": "abc",
                "created_at": "2017-11-17 07:43:44.830845",
                "id": "4a1a10d7-0d9f-4846-8cda-24cffeffef5c",
                "floating_ip_address": "5.21.11.142"
            }
        ]
    }
    ```


## 返回值<a name="section13981185113572"></a>

请参见[通用请求返回值](通用请求返回值.md)。

