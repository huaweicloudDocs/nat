# 查询指定的NAT网关详情<a name="zh-cn_topic_0130808154"></a>

## 功能介绍<a name="section45827181"></a>

查询指定的NAT网关详情。

## URI<a name="section9791447"></a>

GET /v2.0/nat\_gateways/\{nat\_gateway\_id\}

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
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="p20912111395719"><a name="p20912111395719"></a><a name="p20912111395719"></a>所属NAT网关的id。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section54909781"></a>

无

## 响应消息<a name="section24425986"></a>

响应参数如[表2](#table129831149144215)所示。

**表 2**  响应参数

<a name="table129831149144215"></a>
<table><thead align="left"><tr id="row2233175015424"><th class="cellrowborder" valign="top" width="22.93%" id="mcps1.2.4.1.1"><p id="p112331950124213"><a name="p112331950124213"></a><a name="p112331950124213"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.83%" id="mcps1.2.4.1.2"><p id="p1023335020429"><a name="p1023335020429"></a><a name="p1023335020429"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.24%" id="mcps1.2.4.1.3"><p id="p1123319502426"><a name="p1123319502426"></a><a name="p1123319502426"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1223325010421"><td class="cellrowborder" valign="top" width="22.93%" headers="mcps1.2.4.1.1 "><p id="p202331450134211"><a name="p202331450134211"></a><a name="p202331450134211"></a>nat_gateway</p>
</td>
<td class="cellrowborder" valign="top" width="18.83%" headers="mcps1.2.4.1.2 "><p id="p12331150184217"><a name="p12331150184217"></a><a name="p12331150184217"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="58.24%" headers="mcps1.2.4.1.3 "><p id="p62331505427"><a name="p62331505427"></a><a name="p62331505427"></a>nat_gateway对象。详见<a href="#table514165011429">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  nat\_gateway字段说明

<a name="table514165011429"></a>
<table><thead align="left"><tr id="row1233175044210"><th class="cellrowborder" valign="top" width="23.23%" id="mcps1.2.4.1.1"><p id="p16233350194217"><a name="p16233350194217"></a><a name="p16233350194217"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.2"><p id="p1123375010428"><a name="p1123375010428"></a><a name="p1123375010428"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.589999999999996%" id="mcps1.2.4.1.3"><p id="p2023313507424"><a name="p2023313507424"></a><a name="p2023313507424"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row623313504427"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p162338502421"><a name="p162338502421"></a><a name="p162338502421"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p92331950144219"><a name="p92331950144219"></a><a name="p92331950144219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="p5233165034219"><a name="p5233165034219"></a><a name="p5233165034219"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="row72331550164211"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p1123335024220"><a name="p1123335024220"></a><a name="p1123335024220"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p8233450174216"><a name="p8233450174216"></a><a name="p8233450174216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="p172332504428"><a name="p172332504428"></a><a name="p172332504428"></a>项目的ID。</p>
</td>
</tr>
<tr id="row17233185084220"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p323355014426"><a name="p323355014426"></a><a name="p323355014426"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p323355044218"><a name="p323355044218"></a><a name="p323355044218"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="p42331650144212"><a name="p42331650144212"></a><a name="p42331650144212"></a>NAT网关的名字。</p>
<p id="p72333505429"><a name="p72333505429"></a><a name="p72333505429"></a>NAT网关的名字仅支持数字、字母、_（下划线）、-（中划线）、中文。</p>
</td>
</tr>
<tr id="row1623315018422"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p19233145020424"><a name="p19233145020424"></a><a name="p19233145020424"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p423318503426"><a name="p423318503426"></a><a name="p423318503426"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="p923335014212"><a name="p923335014212"></a><a name="p923335014212"></a>NAT网关的描述。</p>
</td>
</tr>
<tr id="row1623315506427"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p18233350184218"><a name="p18233350184218"></a><a name="p18233350184218"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p15233105018428"><a name="p15233105018428"></a><a name="p15233105018428"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="p1023385084218"><a name="p1023385084218"></a><a name="p1023385084218"></a>NAT网关的规格。</p>
<p id="p1223319508422"><a name="p1223319508422"></a><a name="p1223319508422"></a>取值为：</p>
<a name="ul132334508424"></a><a name="ul132334508424"></a><ul id="ul132334508424"><li>“1”：小型，SNAT最大连接数10000</li><li>“2”：中型，SNAT最大连接数50000</li><li>“3”：大型，SNAT最大连接数200000</li><li>“4”：超大型，SNAT最大连接数1000000</li></ul>
</td>
</tr>
<tr id="row42331050144212"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p1723325015428"><a name="p1723325015428"></a><a name="p1723325015428"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p3233115094213"><a name="p3233115094213"></a><a name="p3233115094213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="p102331150144211"><a name="p102331150144211"></a><a name="p102331150144211"></a>路由器的UUID。</p>
</td>
</tr>
<tr id="row72331650164215"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p8233195017429"><a name="p8233195017429"></a><a name="p8233195017429"></a>internal_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p223314508421"><a name="p223314508421"></a><a name="p223314508421"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="p4233125084214"><a name="p4233125084214"></a><a name="p4233125084214"></a>NAT网关下行口（DVR的下一跳）所属的network id。</p>
</td>
</tr>
<tr id="row102339502423"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p82331150114212"><a name="p82331150114212"></a><a name="p82331150114212"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p1823311508429"><a name="p1823311508429"></a><a name="p1823311508429"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><a name="ul9233155034214"></a><a name="ul9233155034214"></a><ul id="ul9233155034214"><li>功能说明：NAT网关的状态。</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="row20233450104210"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p32333502427"><a name="p32333502427"></a><a name="p32333502427"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p1764614265487"><a name="p1764614265487"></a><a name="p1764614265487"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><a name="ul71858556358"></a><a name="ul71858556358"></a><ul id="ul71858556358"><li>解冻/冻结状态。</li><li>取值范围：<a name="ul11838172814409"></a><a name="ul11838172814409"></a><ul id="ul11838172814409"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="row22331050154211"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p723305014427"><a name="p723305014427"></a><a name="p723305014427"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p423312509427"><a name="p423312509427"></a><a name="p423312509427"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="p16351227165916"><a name="p16351227165916"></a><a name="p16351227165916"></a>NAT网关的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section18507287"></a>

-   请求样例

    ```
    GET https://{Endpoint}/v2.0/nat_gateways/a78fb3eb-1654-4710-8742-3fc49d5f04f8
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


## 状态码<a name="section22695302"></a>

请参考[状态码](状态码.md)。

