# 更新NAT网关<a name="ZH-CN_TOPIC_0130808162"></a>

## 功能介绍<a name="section53650918"></a>

更新NAT网关。

>![](public_sys-resources/icon-note.gif) **说明：**   
>更新名称： admin\_state\_up = True & status = "ACTIVE"允许更新  
>更新描述： admin\_state\_up = True & status = "ACTIVE"允许更新  
>更新规格： admin\_state\_up = True & status = "ACTIVE"允许更新  

## URI<a name="section13096217"></a>

PUT /v2.0/nat\_gateways/\{nat\_gateway\_id\}

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

## 请求消息<a name="section54160660"></a>

请求参数如[表2](#table52686130)所示。

**表 2**  请求参数

<a name="table52686130"></a>
<table><thead align="left"><tr id="row64917235"><th class="cellrowborder" valign="top" width="23%" id="mcps1.2.5.1.1"><p id="p23804665"><a name="p23804665"></a><a name="p23804665"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="18%" id="mcps1.2.5.1.2"><p id="p49129749"><a name="p49129749"></a><a name="p49129749"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.3"><p id="p20086700"><a name="p20086700"></a><a name="p20086700"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="43%" id="mcps1.2.5.1.4"><p id="p16410024"><a name="p16410024"></a><a name="p16410024"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2330579495259"><td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.5.1.1 "><p id="p872120095259"><a name="p872120095259"></a><a name="p872120095259"></a>nat_gateway</p>
</td>
<td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.5.1.2 "><p id="p3532861095259"><a name="p3532861095259"></a><a name="p3532861095259"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.3 "><p id="p4304518595259"><a name="p4304518595259"></a><a name="p4304518595259"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.5.1.4 "><p id="p6410795695259"><a name="p6410795695259"></a><a name="p6410795695259"></a>nat_gateway对象。</p>
<p id="p2978120995417"><a name="p2978120995417"></a><a name="p2978120995417"></a>必选字段：无，只有name，description和spec字段允许更新，更新操作时至少指定一项属性。</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section17683893"></a>

响应消息如[表3](#table26619133)所示。

**表 3**  响应参数

<a name="table26619133"></a>
<table><thead align="left"><tr id="row25196298"><th class="cellrowborder" valign="top" width="31.7%" id="mcps1.2.4.1.1"><p id="p27634258"><a name="p27634258"></a><a name="p27634258"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.080000000000002%" id="mcps1.2.4.1.2"><p id="p23782439"><a name="p23782439"></a><a name="p23782439"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p8475542"><a name="p8475542"></a><a name="p8475542"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row15430272"><td class="cellrowborder" valign="top" width="31.7%" headers="mcps1.2.4.1.1 "><p id="p41892502"><a name="p41892502"></a><a name="p41892502"></a>nat_gateway</p>
</td>
<td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.2.4.1.2 "><p id="p37849538"><a name="p37849538"></a><a name="p37849538"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p28022645"><a name="p28022645"></a><a name="p28022645"></a>nat_gateway对象。</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section24937315"></a>

-   请求样例

    ```
    PUT /v2.0/nat_gateways/a78fb3eb-1654-4710-8742-3fc49d5f04f8
      {
        "nat_gateway": {
            "name": "new_name",
            "description": "new description",
            "spec": "1"
        }
    }
    ```


-   响应样例

    ```
    {
        "nat_gateway": {
            "router_id": "d84f345c-80a1-4fa2-a39c-d0d397c3f09a",
            "status": "ACTIVE",
            "description": "new description",
            "admin_state_up": true,
            "tenant_id": "27e25061336f4af590faeabeb7fcd9a3",
            "created_at": "2017-11-18 07:34:32.203044",
            "spec": "1",
            "internal_network_id": "89d66639-aacb-4929-969d-07080b0f9fd9",
            "id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
            "name": "new_name"
        }
    } 
    ```


## 返回值<a name="section6656623"></a>

请参见[通用请求返回值](通用请求返回值.md)。

