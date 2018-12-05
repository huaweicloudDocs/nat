# 创建DNAT规则<a name="ZH-CN_TOPIC_0130808145"></a>

## 功能介绍<a name="section2213133217038"></a>

创建DNAT规则

>![](public_sys-resources/icon-note.gif) **说明：**   
>创建规则时，要求网关状态status = "ACTIVE"，要求网关管理员状态admin\_state\_up = True。port\_id和private\_ip不能同时生效。对于all port类型的规则，要求internal\_service\_port = 0，external\_service\_port = 0，protocol = ANY.  

## URI<a name="section2631225217131"></a>

POST /v2.0/dnat\_rules

## 请求消息<a name="section1572764517510"></a>

请求参数如[表1](#table1482767817525)所示。

**表 1**  请求参数

<a name="table1482767817525"></a>
<table><thead align="left"><tr id="row1595640417525"><th class="cellrowborder" valign="top" width="21.21%" id="mcps1.2.5.1.1"><p id="p1740033817525"><a name="p1740033817525"></a><a name="p1740033817525"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="12.120000000000001%" id="mcps1.2.5.1.2"><p id="p14127717525"><a name="p14127717525"></a><a name="p14127717525"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p1144345217525"><a name="p1144345217525"></a><a name="p1144345217525"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="52.53%" id="mcps1.2.5.1.4"><p id="p5450440817525"><a name="p5450440817525"></a><a name="p5450440817525"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row5278088817525"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.5.1.1 "><p id="p4739350817525"><a name="p4739350817525"></a><a name="p4739350817525"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="12.120000000000001%" headers="mcps1.2.5.1.2 "><p id="p1366896517525"><a name="p1366896517525"></a><a name="p1366896517525"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p3344441917525"><a name="p3344441917525"></a><a name="p3344441917525"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="52.53%" headers="mcps1.2.5.1.4 "><p id="p20912111395719"><a name="p20912111395719"></a><a name="p20912111395719"></a>所属NAT网关的id。</p>
</td>
</tr>
<tr id="row2046427617525"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.5.1.1 "><p id="p4699362317525"><a name="p4699362317525"></a><a name="p4699362317525"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="12.120000000000001%" headers="mcps1.2.5.1.2 "><p id="p4838715617525"><a name="p4838715617525"></a><a name="p4838715617525"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p2704555317525"><a name="p2704555317525"></a><a name="p2704555317525"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="52.53%" headers="mcps1.2.5.1.4 "><p id="p1991781916569"><a name="p1991781916569"></a><a name="p1991781916569"></a>虚拟机或者裸机的Port ID，与private_ip不能共存。</p>
</td>
</tr>
<tr id="row1287293812249"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.5.1.1 "><p id="p5552194772414"><a name="p5552194772414"></a><a name="p5552194772414"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="12.120000000000001%" headers="mcps1.2.5.1.2 "><p id="p11552194732415"><a name="p11552194732415"></a><a name="p11552194732415"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p145521947142416"><a name="p145521947142416"></a><a name="p145521947142416"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="52.53%" headers="mcps1.2.5.1.4 "><p id="p19552154722418"><a name="p19552154722418"></a><a name="p19552154722418"></a>裸机VM的IP地址或者用户私有IP地址，对于all port类型的规则private_ip生效,port_id可选，若带port_id,则必须为""。</p>
</td>
</tr>
<tr id="row5331118017525"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.5.1.1 "><p id="p2323828917525"><a name="p2323828917525"></a><a name="p2323828917525"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="12.120000000000001%" headers="mcps1.2.5.1.2 "><p id="p325323417525"><a name="p325323417525"></a><a name="p325323417525"></a>Int</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p6218543317525"><a name="p6218543317525"></a><a name="p6218543317525"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="52.53%" headers="mcps1.2.5.1.4 "><p id="p385527517525"><a name="p385527517525"></a><a name="p385527517525"></a>虚拟机或者裸机对外提供服务的协议端口号。</p>
</td>
</tr>
<tr id="row3469748117525"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.5.1.1 "><p id="p5903255317525"><a name="p5903255317525"></a><a name="p5903255317525"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="12.120000000000001%" headers="mcps1.2.5.1.2 "><p id="p1690749817525"><a name="p1690749817525"></a><a name="p1690749817525"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p2733009917525"><a name="p2733009917525"></a><a name="p2733009917525"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="52.53%" headers="mcps1.2.5.1.4 "><p id="p1222834015610"><a name="p1222834015610"></a><a name="p1222834015610"></a>浮动IP的id。</p>
</td>
</tr>
<tr id="row5941910017525"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.5.1.1 "><p id="p4821779417525"><a name="p4821779417525"></a><a name="p4821779417525"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="12.120000000000001%" headers="mcps1.2.5.1.2 "><p id="p1332721217525"><a name="p1332721217525"></a><a name="p1332721217525"></a>Int</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p576237017525"><a name="p576237017525"></a><a name="p576237017525"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="52.53%" headers="mcps1.2.5.1.4 "><p id="p6409886217525"><a name="p6409886217525"></a><a name="p6409886217525"></a>Floatingip对外提供服务的端口号。</p>
</td>
</tr>
<tr id="row4001884617525"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.5.1.1 "><p id="p2030112317525"><a name="p2030112317525"></a><a name="p2030112317525"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="12.120000000000001%" headers="mcps1.2.5.1.2 "><p id="p3377828917525"><a name="p3377828917525"></a><a name="p3377828917525"></a>Str or Int</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p5168686317525"><a name="p5168686317525"></a><a name="p5168686317525"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="52.53%" headers="mcps1.2.5.1.4 "><p id="p11441165818393"><a name="p11441165818393"></a><a name="p11441165818393"></a>协议类型，目前支持TCP/UDP/ANY</p>
<p id="p164411258203913"><a name="p164411258203913"></a><a name="p164411258203913"></a>对应协议号6/17/0</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section4576293817529"></a>

响应参数如[表2](#table4946919917549)所示。

**表 2**  响应参数

<a name="table4946919917549"></a>
<table><thead align="left"><tr id="row3265693817549"><th class="cellrowborder" valign="top" width="24%" id="mcps1.2.4.1.1"><p id="p2796632617549"><a name="p2796632617549"></a><a name="p2796632617549"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="28.000000000000004%" id="mcps1.2.4.1.2"><p id="p5067993017549"><a name="p5067993017549"></a><a name="p5067993017549"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="48%" id="mcps1.2.4.1.3"><p id="p5371412517549"><a name="p5371412517549"></a><a name="p5371412517549"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row5587684317549"><td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.1 "><p id="p2973040117549"><a name="p2973040117549"></a><a name="p2973040117549"></a>dnat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.2 "><p id="p5935228017549"><a name="p5935228017549"></a><a name="p5935228017549"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="48%" headers="mcps1.2.4.1.3 "><p id="p4468272717549"><a name="p4468272717549"></a><a name="p4468272717549"></a>dnat_rule对象。</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section956164017620"></a>

-   请求样例

    1.  创建指定端口的规则

    ```
    POST/v2.0/dnat_rules{
        "dnat_rule": {
            "floating_ip_id": "bf99c679-9f41-4dac-8513-9c9228e713e1",
            "nat_gateway_id": "cda3a125-2406-456c-a11f-598e10578541",
            "port_id": "9a469561-daac-4c94-88f5-39366e5ea193",  
            "private_ip": "",
            "internal_service_port": 993,
            "protocol": "tcp",
            "external_service_port": 242
        }
    }
    ```

    1.  创建all port类型的规则。

        ```
        POST/v2.0/dnat_rules{
            "dnat_rule": {
                "floating_ip_id": "Cf99c679-9f41-4dac-8513-9c9228e713e1",
                "nat_gateway_id": "Dda3a125-2406-456c-a11f-598e10578541",
                "port_id": "",
                "private_ip": "192.168.1.100",
                "internal_service_port": 0,
                "protocol": "any",
                "external_service_port": 0
            }
        }
        ```



-   响应样例
    1.  创建指定端口的规则的响应

        ```
        {
            "dnat_rule": {
                "floating_ip_id": "bf99c679-9f41-4dac-8513-9c9228e713e1",
                "status": "ACTIVE",
                "nat_gateway_id": "cda3a125-2406-456c-a11f-598e10578541",
                "admin_state_up": true,
                "port_id": "9a469561-daac-4c94-88f5-39366e5ea193",
                "private_ip": "",
                "internal_service_port": 993,
                "protocol": "TCP",
                "tenant_id": "abc",
                "created_at": "2017-11-15 15:44:42.595173",
                "id": "79195d50-0271-41f1-bded-4c089b2502ff",
                "floating_ip_address": "5.21.11.226",
                "external_service_port": 242
            }
        }
        ```

    2.  创建all port类型的规则的响应

        ```
        {
            "dnat_rule": {
                "floating_ip_id": "cf99c679-9f41-4dac-8513-9c9228e713e1",
                "status": "ACTIVE",
                "nat_gateway_id": "dda3a125-2406-456c-a11f-598e10578541",
                "admin_state_up": true,
                "port_id": "",
                "private_ip": "192.168.1.100",
                "internal_service_port": 0,
                "protocol": "any",
                "tenant_id": "abc",
                "created_at": "2017-11-15 15:44:42.595173",
                "id": "79195d50-0271-41f1-bded-4c089b2502ff",
                "floating_ip_address": "5.21.11.227",
                "external_service_port": 0
            }
        }
        ```



## 返回值<a name="section5446226317959"></a>

请参见[通用请求返回值](通用请求返回值.md)。

