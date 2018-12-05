# 查询DNAT规则列表<a name="ZH-CN_TOPIC_0130808186"></a>

## 功能介绍<a name="section28610428164132"></a>

查询DNAT规则列表。

## URI<a name="section19503903164158"></a>

GET /v2.0/dnat\_rules?id=\{id\}&tenant\_id=\{tenant\_id\}&port\_id=\{port\_id\}&internal\_service\_port=\{internal\_service\_port\}&floating\_ip\_id=\{floating\_ip\_id\}&floating\_ip\_address=\{floating\_ip\_address\}&external\_service\_port=\{external\_service\_port\}&protocol=protocol&status=\{status\}&created\_at=\{created\_at\}&admin\_state\_up=\{admin\_state\_up\}&private\_ip=\{private\_ip\}

## 请求消息<a name="section2749321016454"></a>

无

## 响应消息<a name="section55770648164519"></a>

响应参数如[表1](#table47307406164538)所示。

**表 1**  响应参数

<a name="table47307406164538"></a>
<table><thead align="left"><tr id="row43170063164538"><th class="cellrowborder" valign="top" width="20.73%" id="mcps1.2.4.1.1"><p id="p7114239164538"><a name="p7114239164538"></a><a name="p7114239164538"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="28.050000000000004%" id="mcps1.2.4.1.2"><p id="p39382504164538"><a name="p39382504164538"></a><a name="p39382504164538"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p19483074164538"><a name="p19483074164538"></a><a name="p19483074164538"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row34625156164538"><td class="cellrowborder" valign="top" width="20.73%" headers="mcps1.2.4.1.1 "><p id="p53174238164538"><a name="p53174238164538"></a><a name="p53174238164538"></a>dnat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="28.050000000000004%" headers="mcps1.2.4.1.2 "><p id="p12146041164538"><a name="p12146041164538"></a><a name="p12146041164538"></a>List(dnat_rule)</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p31957648164538"><a name="p31957648164538"></a><a name="p31957648164538"></a>dnat_rule对象列表。</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section39793997164640"></a>

-   请求样例

    ```
    GET /v2.0/dnat_rules
    ```


-   响应样例

    ```
    {
        "dnat_rules": [
            {
                "floating_ip_id": "bf99c679-9f41-4dac-8513-9c9228e713e1",
                "status": "ACTIVE",
                "nat_gateway_id": "cda3a125-2406-456c-a11f-598e10578541",
                "admin_state_up": true,
                "port_id": "9a469561-daac-4c94-88f5-39366e5ea193",
                "private_ip": "",
                "internal_service_port": 993,
                "protocol": "tcp",
                "tenant_id": "abc",
                "created_at": "2017-11-15 15:44:42.595173",
                "id": "79195d50-0271-41f1-bded-4c089b2502ff",
                "floating_ip_address": "5.21.11.226",
                "external_service_port": 242
            },
            {
                "floating_ip_id": "cf99c679-9f41-4dac-8513-9c9228e713e1",
                "status": "ACTIVE",
                "nat_gateway_id": "dda3a125-2406-456c-a11f-598e10578541",
                "admin_state_up": true,
                "port_id": "",
                "private_ip": "192.168.1.100",
                "internal_service_port": 0,
                "protocol": "any",
                "tenant_id": "abc",
                "created_at": "2017-11-16 15:44:42.595173",
                "id": "89195d50-0271-41f1-bded-4c089b2502ff",
                "floating_ip_address": "5.21.11.227",
                "external_service_port": 0
            }
        ]
    }
    ```


## 返回值<a name="section45841191164749"></a>

请参见[通用请求返回值](通用请求返回值.md)。

