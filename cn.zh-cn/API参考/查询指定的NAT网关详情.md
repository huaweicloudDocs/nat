# 查询指定的NAT网关详情<a name="ZH-CN_TOPIC_0130808154"></a>

## 功能介绍<a name="section45827181"></a>

查询指定的NAT网关详情。

## URI<a name="section9791447"></a>

GET /v2.0/nat\_gateways/\{nat\_gateway\_id\}

**表 1**  参数说明

<a name="table285161395713"></a>
<table><thead align="left"><tr id="row12912101317577"><th class="cellrowborder" valign="top" width="21.21%" id="mcps1.2.5.1.1"><p id="p791271313579"><a name="p791271313579"></a><a name="p791271313579"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="12.120000000000001%" id="mcps1.2.5.1.2"><p id="p7912013105718"><a name="p7912013105718"></a><a name="p7912013105718"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p1391221355716"><a name="p1391221355716"></a><a name="p1391221355716"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="52.53%" id="mcps1.2.5.1.4"><p id="p1191216131572"><a name="p1191216131572"></a><a name="p1191216131572"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1591281345717"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.5.1.1 "><p id="p69121213115717"><a name="p69121213115717"></a><a name="p69121213115717"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="12.120000000000001%" headers="mcps1.2.5.1.2 "><p id="p179129138573"><a name="p179129138573"></a><a name="p179129138573"></a>Uuid-Str</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p1291281325710"><a name="p1291281325710"></a><a name="p1291281325710"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="52.53%" headers="mcps1.2.5.1.4 "><p id="p20912111395719"><a name="p20912111395719"></a><a name="p20912111395719"></a>所属NAT网关的id。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section54909781"></a>

无

## 响应消息<a name="section24425986"></a>

响应参数如[表2](#table7384096)所示。

**表 2**  响应参数

<a name="table7384096"></a>
<table><thead align="left"><tr id="row51099441"><th class="cellrowborder" valign="top" width="20.73%" id="mcps1.2.4.1.1"><p id="p45414023"><a name="p45414023"></a><a name="p45414023"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="28.050000000000004%" id="mcps1.2.4.1.2"><p id="p54657246"><a name="p54657246"></a><a name="p54657246"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p43533229"><a name="p43533229"></a><a name="p43533229"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row36530678"><td class="cellrowborder" valign="top" width="20.73%" headers="mcps1.2.4.1.1 "><p id="p6194911"><a name="p6194911"></a><a name="p6194911"></a>nat_gateway</p>
</td>
<td class="cellrowborder" valign="top" width="28.050000000000004%" headers="mcps1.2.4.1.2 "><p id="p32025744"><a name="p32025744"></a><a name="p32025744"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p3055980"><a name="p3055980"></a><a name="p3055980"></a>nat_gateway对象。</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section18507287"></a>

-   请求样例

    ```
    GET /v2.0/nat_gateways/a78fb3eb-1654-4710-8742-3fc49d5f04f8
    ```


-   响应样例

    ```
    {
        "nat_gateway": {
            "router_id": "d84f345c-80a1-4fa2-a39c-d0d397c3f09a",
            "status": "ACTIVE",
            "description": "my nat gateway 01",
            "admin_state_up": true,
            "tenant_id": "27e25061336f4af590faeabeb7fcd9a3",
            "created_at": "2017-11-18 07:34:32.203044",
            "spec": "1",
            "internal_network_id": "89d66639-aacb-4929-969d-07080b0f9fd9",
            "id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
            "name": "nat_001"
        }
    }
    ```


## 返回值<a name="section22695302"></a>

请参见[通用请求返回值](通用请求返回值.md)。

