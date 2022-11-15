# 删除公网NAT网关<a name="nat_api_0004"></a>

## 功能介绍<a name="section23460301"></a>

删除公网NAT网关。

## URI<a name="section9816121"></a>

DELETE /v2.0/nat\_gateways/\{nat\_gateway\_id\}

**表 1**  参数说明

<a name="table285161395713"></a>
<table><thead align="left"><tr id="row12912101317577"><th class="cellrowborder" valign="top" width="22.57%" id="mcps1.2.5.1.1"><p id="p791271313579"><a name="p791271313579"></a><a name="p791271313579"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.649999999999999%" id="mcps1.2.5.1.2"><p id="p1391221355716"><a name="p1391221355716"></a><a name="p1391221355716"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.9%" id="mcps1.2.5.1.3"><p id="p7912013105718"><a name="p7912013105718"></a><a name="p7912013105718"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.879999999999995%" id="mcps1.2.5.1.4"><p id="p1191216131572"><a name="p1191216131572"></a><a name="p1191216131572"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1591281345717"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="p69121213115717"><a name="p69121213115717"></a><a name="p69121213115717"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="p1291281325710"><a name="p1291281325710"></a><a name="p1291281325710"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="p179129138573"><a name="p179129138573"></a><a name="p179129138573"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="p20912111395719"><a name="p20912111395719"></a><a name="p20912111395719"></a>所属公网NAT网关的id。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section56908304"></a>

无

## 响应消息<a name="section42412694"></a>

无

## 示例<a name="section46169932"></a>

-   请求样例

    ```
    DELETE https://{Endpoint}/v2.0/nat_gateways/a78fb3eb-1654-4710-8742-3fc49d5f04f8
    ```


-   响应样例

    ```
    无（STATUS CODE 204）
    ```


## 状态码<a name="section48777045"></a>

请参考[状态码](状态码.md)。

