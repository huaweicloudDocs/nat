# 查询指定的DNAT规则详情<a name="ZH-CN_TOPIC_0130808174"></a>

## 功能介绍<a name="section242916116504"></a>

查询指定的DNAT规则详情。

## URI<a name="section55252672165026"></a>

GET /v2.0/dnat\_rules/\{dnat\_rule\_id\}

**表 1**  参数说明

<a name="table41603310017"></a>
<table><thead align="left"><tr id="row323012314017"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p1023043508"><a name="p1023043508"></a><a name="p1023043508"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="22%" id="mcps1.2.5.1.2"><p id="p1823017318015"><a name="p1823017318015"></a><a name="p1823017318015"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="p52301036011"><a name="p52301036011"></a><a name="p52301036011"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="32%" id="mcps1.2.5.1.4"><p id="p7230330014"><a name="p7230330014"></a><a name="p7230330014"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row9230031106"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1823033907"><a name="p1823033907"></a><a name="p1823033907"></a>dnat_rule_id</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.2.5.1.2 "><p id="p42301335017"><a name="p42301335017"></a><a name="p42301335017"></a>Uuid-Str</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p623013311018"><a name="p623013311018"></a><a name="p623013311018"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.5.1.4 "><p id="p5230735019"><a name="p5230735019"></a><a name="p5230735019"></a>所属DNAT规则的id。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section30445355165052"></a>

无

## 响应消息<a name="section1412948816517"></a>

响应参数如[表2](#table66411570165117)所示。

**表 2**  响应参数

<a name="table66411570165117"></a>
<table><thead align="left"><tr id="row43436947165117"><th class="cellrowborder" valign="top" width="28.000000000000004%" id="mcps1.2.4.1.1"><p id="p28731843165117"><a name="p28731843165117"></a><a name="p28731843165117"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="38%" id="mcps1.2.4.1.2"><p id="p45577964165117"><a name="p45577964165117"></a><a name="p45577964165117"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="34%" id="mcps1.2.4.1.3"><p id="p67033414165117"><a name="p67033414165117"></a><a name="p67033414165117"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row60997448165117"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.1 "><p id="p41846242165117"><a name="p41846242165117"></a><a name="p41846242165117"></a>dnat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.4.1.2 "><p id="p34102461165117"><a name="p34102461165117"></a><a name="p34102461165117"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="34%" headers="mcps1.2.4.1.3 "><p id="p5298260165117"><a name="p5298260165117"></a><a name="p5298260165117"></a>dnat_rule对象。</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section24779297165121"></a>

-   请求样例

    ```
    GET /v2.0/dnat_rules/5b95c675-69c2-4656-ba06-58ff72e1d338
    ```


-   响应样例

    ```
    {              
       {
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


## 返回值<a name="section16249219165526"></a>

请参见[通用请求返回值](通用请求返回值.md)。

