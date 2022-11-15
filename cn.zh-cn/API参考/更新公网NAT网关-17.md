# 更新公网NAT网关<a name="nat_api_0003"></a>

## 功能介绍<a name="section53650918"></a>

更新公网NAT网关。

>![](public_sys-resources/icon-note.gif) **说明：** 
>admin\_state\_up = True & status = "ACTIVE"允许更新，支持更新名称、描述、规格

## URI<a name="section13096217"></a>

PUT /v2.0/nat\_gateways/\{nat\_gateway\_id\}

**表 1**  参数说明

<a name="table285161395713"></a>
<table><thead align="left"><tr id="row12912101317577"><th class="cellrowborder" valign="top" width="21.21%" id="mcps1.2.5.1.1"><p id="p791271313579"><a name="p791271313579"></a><a name="p791271313579"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="12.120000000000001%" id="mcps1.2.5.1.2"><p id="p7912013105718"><a name="p7912013105718"></a><a name="p7912013105718"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p1391221355716"><a name="p1391221355716"></a><a name="p1391221355716"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="52.53%" id="mcps1.2.5.1.4"><p id="p1191216131572"><a name="p1191216131572"></a><a name="p1191216131572"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1591281345717"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.5.1.1 "><p id="p69121213115717"><a name="p69121213115717"></a><a name="p69121213115717"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="12.120000000000001%" headers="mcps1.2.5.1.2 "><p id="p179129138573"><a name="p179129138573"></a><a name="p179129138573"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p1291281325710"><a name="p1291281325710"></a><a name="p1291281325710"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="52.53%" headers="mcps1.2.5.1.4 "><p id="p20912111395719"><a name="p20912111395719"></a><a name="p20912111395719"></a>所属公网NAT网关的id。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section54160660"></a>

请求参数如[表2](#table52686130)所示。

**表 2**  请求参数

<a name="table52686130"></a>
<table><thead align="left"><tr id="row64917235"><th class="cellrowborder" valign="top" width="24.15%" id="mcps1.2.5.1.1"><p id="p23804665"><a name="p23804665"></a><a name="p23804665"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.89%" id="mcps1.2.5.1.2"><p id="p20086700"><a name="p20086700"></a><a name="p20086700"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.61%" id="mcps1.2.5.1.3"><p id="p49129749"><a name="p49129749"></a><a name="p49129749"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="49.35%" id="mcps1.2.5.1.4"><p id="p16410024"><a name="p16410024"></a><a name="p16410024"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row2330579495259"><td class="cellrowborder" valign="top" width="24.15%" headers="mcps1.2.5.1.1 "><p id="p872120095259"><a name="p872120095259"></a><a name="p872120095259"></a>nat_gateway</p>
</td>
<td class="cellrowborder" valign="top" width="8.89%" headers="mcps1.2.5.1.2 "><p id="p4304518595259"><a name="p4304518595259"></a><a name="p4304518595259"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.61%" headers="mcps1.2.5.1.3 "><p id="p3532861095259"><a name="p3532861095259"></a><a name="p3532861095259"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="49.35%" headers="mcps1.2.5.1.4 "><p id="p6410795695259"><a name="p6410795695259"></a><a name="p6410795695259"></a>nat_gateway对象。详见<a href="#table0906373491">表3</a>。</p>
<p id="p2978120995417"><a name="p2978120995417"></a><a name="p2978120995417"></a>必选字段：无，只有name，description和spec字段允许更新，更新操作时至少指定一项属性。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  nat\_gateway字段说明

<a name="table0906373491"></a>
<table><thead align="left"><tr id="row1926123710498"><th class="cellrowborder" valign="top" width="23.72%" id="mcps1.2.5.1.1"><p id="p12261203754915"><a name="p12261203754915"></a><a name="p12261203754915"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.219999999999999%" id="mcps1.2.5.1.2"><p id="p026183710495"><a name="p026183710495"></a><a name="p026183710495"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.56%" id="mcps1.2.5.1.3"><p id="p12611537194919"><a name="p12611537194919"></a><a name="p12611537194919"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="49.5%" id="mcps1.2.5.1.4"><p id="p4261537124914"><a name="p4261537124914"></a><a name="p4261537124914"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1526113794918"><td class="cellrowborder" valign="top" width="23.72%" headers="mcps1.2.5.1.1 "><p id="p1426114376495"><a name="p1426114376495"></a><a name="p1426114376495"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="8.219999999999999%" headers="mcps1.2.5.1.2 "><p id="p4261153734911"><a name="p4261153734911"></a><a name="p4261153734911"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.56%" headers="mcps1.2.5.1.3 "><p id="p62611137194910"><a name="p62611137194910"></a><a name="p62611137194910"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="49.5%" headers="mcps1.2.5.1.4 "><p id="p626113711491"><a name="p626113711491"></a><a name="p626113711491"></a>公网NAT网关的名字。</p>
<p id="p426118376490"><a name="p426118376490"></a><a name="p426118376490"></a>公网NAT网关的名字仅支持数字、字母、_（下划线）、-（中划线）、中文。</p>
</td>
</tr>
<tr id="row6261133718490"><td class="cellrowborder" valign="top" width="23.72%" headers="mcps1.2.5.1.1 "><p id="p1226113734915"><a name="p1226113734915"></a><a name="p1226113734915"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="8.219999999999999%" headers="mcps1.2.5.1.2 "><p id="p426153724918"><a name="p426153724918"></a><a name="p426153724918"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.56%" headers="mcps1.2.5.1.3 "><p id="p82619377493"><a name="p82619377493"></a><a name="p82619377493"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="49.5%" headers="mcps1.2.5.1.4 "><p id="p926113710497"><a name="p926113710497"></a><a name="p926113710497"></a>公网NAT网关的描述。</p>
</td>
</tr>
<tr id="row142611379498"><td class="cellrowborder" valign="top" width="23.72%" headers="mcps1.2.5.1.1 "><p id="p12261193794913"><a name="p12261193794913"></a><a name="p12261193794913"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="8.219999999999999%" headers="mcps1.2.5.1.2 "><p id="p12261153724911"><a name="p12261153724911"></a><a name="p12261153724911"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.56%" headers="mcps1.2.5.1.3 "><p id="p1326133711499"><a name="p1326133711499"></a><a name="p1326133711499"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="49.5%" headers="mcps1.2.5.1.4 "><p id="p142611837184914"><a name="p142611837184914"></a><a name="p142611837184914"></a>公网NAT网关的规格。</p>
<p id="p1126123713499"><a name="p1126123713499"></a><a name="p1126123713499"></a>取值为：</p>
<a name="ul1526193711496"></a><a name="ul1526193711496"></a><ul id="ul1526193711496"><li>“1”：小型，SNAT最大连接数<span>10000</span></li><li>“2”：中型，SNAT最大连接数<span>50000</span></li><li>“3”：大型，SNAT最大连接数<span>200000</span></li><li>“4”：超大型，SNAT最大连接数<span>1000000</span></li></ul>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section17683893"></a>

响应消息如[表4](#table26619133)所示。

**表 4**  响应参数

<a name="table26619133"></a>
<table><thead align="left"><tr id="row25196298"><th class="cellrowborder" valign="top" width="23.71%" id="mcps1.2.4.1.1"><p id="p27634258"><a name="p27634258"></a><a name="p27634258"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="17.96%" id="mcps1.2.4.1.2"><p id="p23782439"><a name="p23782439"></a><a name="p23782439"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.330000000000005%" id="mcps1.2.4.1.3"><p id="p8475542"><a name="p8475542"></a><a name="p8475542"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row15430272"><td class="cellrowborder" valign="top" width="23.71%" headers="mcps1.2.4.1.1 "><p id="p41892502"><a name="p41892502"></a><a name="p41892502"></a>nat_gateway</p>
</td>
<td class="cellrowborder" valign="top" width="17.96%" headers="mcps1.2.4.1.2 "><p id="p37849538"><a name="p37849538"></a><a name="p37849538"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.2.4.1.3 "><p id="p28022645"><a name="p28022645"></a><a name="p28022645"></a>nat_gateway对象。详见<a href="#table144824405116">表5</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 5**  nat\_gateway字段说明

<a name="table144824405116"></a>
<table><thead align="left"><tr id="row1265444165113"><th class="cellrowborder" valign="top" width="23.23%" id="mcps1.2.4.1.1"><p id="p2065413495118"><a name="p2065413495118"></a><a name="p2065413495118"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.2"><p id="p1465464125116"><a name="p1465464125116"></a><a name="p1465464125116"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.589999999999996%" id="mcps1.2.4.1.3"><p id="p1865414435114"><a name="p1865414435114"></a><a name="p1865414435114"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row196541147512"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p176541446512"><a name="p176541446512"></a><a name="p176541446512"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p9654444513"><a name="p9654444513"></a><a name="p9654444513"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="p26546435114"><a name="p26546435114"></a><a name="p26546435114"></a>公网NAT网关的id。</p>
</td>
</tr>
<tr id="row186542045510"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p10654204185111"><a name="p10654204185111"></a><a name="p10654204185111"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p2654114145119"><a name="p2654114145119"></a><a name="p2654114145119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="p86549465118"><a name="p86549465118"></a><a name="p86549465118"></a>项目的ID。</p>
</td>
</tr>
<tr id="row465474125112"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p36541418515"><a name="p36541418515"></a><a name="p36541418515"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p146544425110"><a name="p146544425110"></a><a name="p146544425110"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="p196541435113"><a name="p196541435113"></a><a name="p196541435113"></a>公网NAT网关的名字。</p>
<p id="p126544413514"><a name="p126544413514"></a><a name="p126544413514"></a>公网NAT网关的名字仅支持数字、字母、_（下划线）、-（中划线）、中文。</p>
</td>
</tr>
<tr id="row467013417513"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p1670248519"><a name="p1670248519"></a><a name="p1670248519"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p767013465115"><a name="p767013465115"></a><a name="p767013465115"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="p367015455118"><a name="p367015455118"></a><a name="p367015455118"></a>公网NAT网关的描述。</p>
</td>
</tr>
<tr id="row367094135115"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p11670104135119"><a name="p11670104135119"></a><a name="p11670104135119"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p1267004195114"><a name="p1267004195114"></a><a name="p1267004195114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="p2067064195110"><a name="p2067064195110"></a><a name="p2067064195110"></a>公网NAT网关的规格。</p>
<p id="p76708418513"><a name="p76708418513"></a><a name="p76708418513"></a>取值为：</p>
<a name="ul1167010455119"></a><a name="ul1167010455119"></a><ul id="ul1167010455119"><li>“1”：小型，SNAT最大连接数<span>10000</span></li><li>“2”：中型，SNAT最大连接数<span>50000</span></li><li>“3”：大型，SNAT最大连接数<span>200000</span></li><li>“4”：超大型，SNAT最大连接数<span>1000000</span></li></ul>
</td>
</tr>
<tr id="row967013418512"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p18670241513"><a name="p18670241513"></a><a name="p18670241513"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p2670144155116"><a name="p2670144155116"></a><a name="p2670144155116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="p126701419511"><a name="p126701419511"></a><a name="p126701419511"></a>路由器的ID。</p>
</td>
</tr>
<tr id="row86706419513"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p46700418514"><a name="p46700418514"></a><a name="p46700418514"></a>internal_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p56701045510"><a name="p56701045510"></a><a name="p56701045510"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="p12670746512"><a name="p12670746512"></a><a name="p12670746512"></a>公网NAT网关下行口（DVR的下一跳）所属的network id。</p>
</td>
</tr>
<tr id="row2067015413511"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p76701143516"><a name="p76701143516"></a><a name="p76701143516"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p86704419513"><a name="p86704419513"></a><a name="p86704419513"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><a name="ul967015411514"></a><a name="ul967015411514"></a><ul id="ul967015411514"><li>功能说明：公网NAT网关的状态。</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="row76701542515"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p19670443510"><a name="p19670443510"></a><a name="p19670443510"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p1764614265487"><a name="p1764614265487"></a><a name="p1764614265487"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><a name="ul71858556358"></a><a name="ul71858556358"></a><ul id="ul71858556358"><li>解冻/冻结状态。</li><li>取值范围：<a name="ul11838172814409"></a><a name="ul11838172814409"></a><ul id="ul11838172814409"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="row1967044145114"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p1167011416513"><a name="p1167011416513"></a><a name="p1167011416513"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p2670141515"><a name="p2670141515"></a><a name="p2670141515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="p1914253805918"><a name="p1914253805918"></a><a name="p1914253805918"></a>公网NAT网关的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section24937315"></a>

-   请求样例

    ```
    PUT https://{Endpoint}/v2.0/nat_gateways/a78fb3eb-1654-4710-8742-3fc49d5f04f8 
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


## 状态码<a name="section6656623"></a>

请参考[状态码](状态码.md)。

