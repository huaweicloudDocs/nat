# 更新NAT网关<a name="nat_apiv2_0008"></a>

## 功能介绍<a name="zh-cn_topic_0168797308_section53650918"></a>

更新NAT网关。

>![](public_sys-resources/icon-note.gif) **说明：**   
>admin\_state\_up = True & status = "ACTIVE"允许更新，支持更新名称、描述、规格  

## URI<a name="zh-cn_topic_0168797308_section13096217"></a>

PUT /v2/\{project\_id\}/nat\_gateways/\{nat\_gateway\_id\}

**表 1**  参数说明

<a name="zh-cn_topic_0168797308_table285161395713"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797308_row12912101317577"><th class="cellrowborder" valign="top" width="23.1%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797308_p791271313579"><a name="zh-cn_topic_0168797308_p791271313579"></a><a name="zh-cn_topic_0168797308_p791271313579"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="11.65%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797308_p1391221355716"><a name="zh-cn_topic_0168797308_p1391221355716"></a><a name="zh-cn_topic_0168797308_p1391221355716"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="19.43%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797308_p07191884299"><a name="zh-cn_topic_0168797308_p07191884299"></a><a name="zh-cn_topic_0168797308_p07191884299"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="45.82%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797308_p1191216131572"><a name="zh-cn_topic_0168797308_p1191216131572"></a><a name="zh-cn_topic_0168797308_p1191216131572"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797308_row11434152518489"><td class="cellrowborder" valign="top" width="23.1%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797308_p4838830204815"><a name="zh-cn_topic_0168797308_p4838830204815"></a><a name="zh-cn_topic_0168797308_p4838830204815"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="11.65%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797308_p8838123019487"><a name="zh-cn_topic_0168797308_p8838123019487"></a><a name="zh-cn_topic_0168797308_p8838123019487"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.43%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797308_p27194812920"><a name="zh-cn_topic_0168797308_p27194812920"></a><a name="zh-cn_topic_0168797308_p27194812920"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.82%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797308_p188381930124817"><a name="zh-cn_topic_0168797308_p188381930124817"></a><a name="zh-cn_topic_0168797308_p188381930124817"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797308_row1591281345717"><td class="cellrowborder" valign="top" width="23.1%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797308_p69121213115717"><a name="zh-cn_topic_0168797308_p69121213115717"></a><a name="zh-cn_topic_0168797308_p69121213115717"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="11.65%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797308_p1291281325710"><a name="zh-cn_topic_0168797308_p1291281325710"></a><a name="zh-cn_topic_0168797308_p1291281325710"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.43%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797308_p67198822914"><a name="zh-cn_topic_0168797308_p67198822914"></a><a name="zh-cn_topic_0168797308_p67198822914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.82%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797308_p20912111395719"><a name="zh-cn_topic_0168797308_p20912111395719"></a><a name="zh-cn_topic_0168797308_p20912111395719"></a>NAT网关的id。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0168797308_section54160660"></a>

请求参数如[表2](#zh-cn_topic_0168797308_table52686130)所示。

**表 2**  请求参数

<a name="zh-cn_topic_0168797308_table52686130"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797308_row64917235"><th class="cellrowborder" valign="top" width="23.630000000000003%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797308_p23804665"><a name="zh-cn_topic_0168797308_p23804665"></a><a name="zh-cn_topic_0168797308_p23804665"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10.81%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797308_p20086700"><a name="zh-cn_topic_0168797308_p20086700"></a><a name="zh-cn_topic_0168797308_p20086700"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.89%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797308_p49129749"><a name="zh-cn_topic_0168797308_p49129749"></a><a name="zh-cn_topic_0168797308_p49129749"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="46.67%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797308_p16410024"><a name="zh-cn_topic_0168797308_p16410024"></a><a name="zh-cn_topic_0168797308_p16410024"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797308_row2330579495259"><td class="cellrowborder" valign="top" width="23.630000000000003%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797308_p872120095259"><a name="zh-cn_topic_0168797308_p872120095259"></a><a name="zh-cn_topic_0168797308_p872120095259"></a>nat_gateway</p>
</td>
<td class="cellrowborder" valign="top" width="10.81%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797308_p4304518595259"><a name="zh-cn_topic_0168797308_p4304518595259"></a><a name="zh-cn_topic_0168797308_p4304518595259"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.89%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797308_p3532861095259"><a name="zh-cn_topic_0168797308_p3532861095259"></a><a name="zh-cn_topic_0168797308_p3532861095259"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="46.67%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797308_p6410795695259"><a name="zh-cn_topic_0168797308_p6410795695259"></a><a name="zh-cn_topic_0168797308_p6410795695259"></a>nat_gateway对象。请参考<a href="#zh-cn_topic_0168797308_table0906373491">表3</a>。</p>
<p id="zh-cn_topic_0168797308_p2978120995417"><a name="zh-cn_topic_0168797308_p2978120995417"></a><a name="zh-cn_topic_0168797308_p2978120995417"></a>必选字段：无，只有name，description和spec字段允许更新，更新操作时至少指定一项属性。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  nat\_gateway字段说明

<a name="zh-cn_topic_0168797308_table0906373491"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797308_row1926123710498"><th class="cellrowborder" valign="top" width="23.72%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797308_p12261203754915"><a name="zh-cn_topic_0168797308_p12261203754915"></a><a name="zh-cn_topic_0168797308_p12261203754915"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10.72%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797308_p026183710495"><a name="zh-cn_topic_0168797308_p026183710495"></a><a name="zh-cn_topic_0168797308_p026183710495"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.92%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797308_p12611537194919"><a name="zh-cn_topic_0168797308_p12611537194919"></a><a name="zh-cn_topic_0168797308_p12611537194919"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="46.64%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797308_p4261537124914"><a name="zh-cn_topic_0168797308_p4261537124914"></a><a name="zh-cn_topic_0168797308_p4261537124914"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797308_row1526113794918"><td class="cellrowborder" valign="top" width="23.72%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797308_p1426114376495"><a name="zh-cn_topic_0168797308_p1426114376495"></a><a name="zh-cn_topic_0168797308_p1426114376495"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="10.72%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797308_p4261153734911"><a name="zh-cn_topic_0168797308_p4261153734911"></a><a name="zh-cn_topic_0168797308_p4261153734911"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.92%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797308_p62611137194910"><a name="zh-cn_topic_0168797308_p62611137194910"></a><a name="zh-cn_topic_0168797308_p62611137194910"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="46.64%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797308_p626113711491"><a name="zh-cn_topic_0168797308_p626113711491"></a><a name="zh-cn_topic_0168797308_p626113711491"></a>NAT网关的名字。</p>
<p id="zh-cn_topic_0168797308_p426118376490"><a name="zh-cn_topic_0168797308_p426118376490"></a><a name="zh-cn_topic_0168797308_p426118376490"></a>NAT网关的名字仅支持数字、字母、_（下划线）、-（中划线）、中文。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797308_row6261133718490"><td class="cellrowborder" valign="top" width="23.72%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797308_p1226113734915"><a name="zh-cn_topic_0168797308_p1226113734915"></a><a name="zh-cn_topic_0168797308_p1226113734915"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="10.72%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797308_p426153724918"><a name="zh-cn_topic_0168797308_p426153724918"></a><a name="zh-cn_topic_0168797308_p426153724918"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.92%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797308_p82619377493"><a name="zh-cn_topic_0168797308_p82619377493"></a><a name="zh-cn_topic_0168797308_p82619377493"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="46.64%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797308_p926113710497"><a name="zh-cn_topic_0168797308_p926113710497"></a><a name="zh-cn_topic_0168797308_p926113710497"></a>NAT网关的描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797308_row142611379498"><td class="cellrowborder" valign="top" width="23.72%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797308_p12261193794913"><a name="zh-cn_topic_0168797308_p12261193794913"></a><a name="zh-cn_topic_0168797308_p12261193794913"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="10.72%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797308_p12261153724911"><a name="zh-cn_topic_0168797308_p12261153724911"></a><a name="zh-cn_topic_0168797308_p12261153724911"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.92%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797308_p1326133711499"><a name="zh-cn_topic_0168797308_p1326133711499"></a><a name="zh-cn_topic_0168797308_p1326133711499"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.64%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797308_p142611837184914"><a name="zh-cn_topic_0168797308_p142611837184914"></a><a name="zh-cn_topic_0168797308_p142611837184914"></a>NAT网关的规格。</p>
<p id="zh-cn_topic_0168797308_p1126123713499"><a name="zh-cn_topic_0168797308_p1126123713499"></a><a name="zh-cn_topic_0168797308_p1126123713499"></a>取值为：</p>
<a name="zh-cn_topic_0168797308_ul1526193711496"></a><a name="zh-cn_topic_0168797308_ul1526193711496"></a><ul id="zh-cn_topic_0168797308_ul1526193711496"><li>“1”：小型，SNAT最大连接数10000</li><li>“2”：中型，SNAT最大连接数50000</li><li>“3”：大型，SNAT最大连接数200000</li><li>“4”：超大型，SNAT最大连接数1000000</li></ul>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="zh-cn_topic_0168797308_section17683893"></a>

响应消息如[表4](#zh-cn_topic_0168797308_table26619133)所示。

**表 4**  响应参数

<a name="zh-cn_topic_0168797308_table26619133"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797308_row25196298"><th class="cellrowborder" valign="top" width="23.54%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797308_p27634258"><a name="zh-cn_topic_0168797308_p27634258"></a><a name="zh-cn_topic_0168797308_p27634258"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.05%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797308_p23782439"><a name="zh-cn_topic_0168797308_p23782439"></a><a name="zh-cn_topic_0168797308_p23782439"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.41%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797308_p8475542"><a name="zh-cn_topic_0168797308_p8475542"></a><a name="zh-cn_topic_0168797308_p8475542"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797308_row15430272"><td class="cellrowborder" valign="top" width="23.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797308_p41892502"><a name="zh-cn_topic_0168797308_p41892502"></a><a name="zh-cn_topic_0168797308_p41892502"></a>nat_gateway</p>
</td>
<td class="cellrowborder" valign="top" width="18.05%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797308_p37849538"><a name="zh-cn_topic_0168797308_p37849538"></a><a name="zh-cn_topic_0168797308_p37849538"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="58.41%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797308_p28022645"><a name="zh-cn_topic_0168797308_p28022645"></a><a name="zh-cn_topic_0168797308_p28022645"></a>nat_gateway对象。请参考<a href="#zh-cn_topic_0168797308_table144824405116">表5</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 5**  nat\_gateway字段说明

<a name="zh-cn_topic_0168797308_table144824405116"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797308_row1265444165113"><th class="cellrowborder" valign="top" width="23.23%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797308_p2065413495118"><a name="zh-cn_topic_0168797308_p2065413495118"></a><a name="zh-cn_topic_0168797308_p2065413495118"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797308_p1465464125116"><a name="zh-cn_topic_0168797308_p1465464125116"></a><a name="zh-cn_topic_0168797308_p1465464125116"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.589999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797308_p1865414435114"><a name="zh-cn_topic_0168797308_p1865414435114"></a><a name="zh-cn_topic_0168797308_p1865414435114"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797308_row196541147512"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797308_p176541446512"><a name="zh-cn_topic_0168797308_p176541446512"></a><a name="zh-cn_topic_0168797308_p176541446512"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797308_p9654444513"><a name="zh-cn_topic_0168797308_p9654444513"></a><a name="zh-cn_topic_0168797308_p9654444513"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797308_p26546435114"><a name="zh-cn_topic_0168797308_p26546435114"></a><a name="zh-cn_topic_0168797308_p26546435114"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797308_row186542045510"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797308_p10654204185111"><a name="zh-cn_topic_0168797308_p10654204185111"></a><a name="zh-cn_topic_0168797308_p10654204185111"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797308_p2654114145119"><a name="zh-cn_topic_0168797308_p2654114145119"></a><a name="zh-cn_topic_0168797308_p2654114145119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797308_p86549465118"><a name="zh-cn_topic_0168797308_p86549465118"></a><a name="zh-cn_topic_0168797308_p86549465118"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797308_row465474125112"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797308_p36541418515"><a name="zh-cn_topic_0168797308_p36541418515"></a><a name="zh-cn_topic_0168797308_p36541418515"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797308_p146544425110"><a name="zh-cn_topic_0168797308_p146544425110"></a><a name="zh-cn_topic_0168797308_p146544425110"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797308_p196541435113"><a name="zh-cn_topic_0168797308_p196541435113"></a><a name="zh-cn_topic_0168797308_p196541435113"></a>NAT网关的名字。</p>
<p id="zh-cn_topic_0168797308_p126544413514"><a name="zh-cn_topic_0168797308_p126544413514"></a><a name="zh-cn_topic_0168797308_p126544413514"></a>NAT网关的名字仅支持数字、字母、_（下划线）、-（中划线）、中文。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797308_row467013417513"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797308_p1670248519"><a name="zh-cn_topic_0168797308_p1670248519"></a><a name="zh-cn_topic_0168797308_p1670248519"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797308_p767013465115"><a name="zh-cn_topic_0168797308_p767013465115"></a><a name="zh-cn_topic_0168797308_p767013465115"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797308_p367015455118"><a name="zh-cn_topic_0168797308_p367015455118"></a><a name="zh-cn_topic_0168797308_p367015455118"></a>NAT网关的描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797308_row367094135115"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797308_p11670104135119"><a name="zh-cn_topic_0168797308_p11670104135119"></a><a name="zh-cn_topic_0168797308_p11670104135119"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797308_p1267004195114"><a name="zh-cn_topic_0168797308_p1267004195114"></a><a name="zh-cn_topic_0168797308_p1267004195114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797308_p2067064195110"><a name="zh-cn_topic_0168797308_p2067064195110"></a><a name="zh-cn_topic_0168797308_p2067064195110"></a>NAT网关的规格。</p>
<p id="zh-cn_topic_0168797308_p76708418513"><a name="zh-cn_topic_0168797308_p76708418513"></a><a name="zh-cn_topic_0168797308_p76708418513"></a>取值为：</p>
<a name="zh-cn_topic_0168797308_ul1167010455119"></a><a name="zh-cn_topic_0168797308_ul1167010455119"></a><ul id="zh-cn_topic_0168797308_ul1167010455119"><li>“1”：小型</li><li>“2”：中型</li><li>“3”：大型</li><li>“4”：超大型</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797308_row967013418512"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797308_p18670241513"><a name="zh-cn_topic_0168797308_p18670241513"></a><a name="zh-cn_topic_0168797308_p18670241513"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797308_p2670144155116"><a name="zh-cn_topic_0168797308_p2670144155116"></a><a name="zh-cn_topic_0168797308_p2670144155116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797308_p126701419511"><a name="zh-cn_topic_0168797308_p126701419511"></a><a name="zh-cn_topic_0168797308_p126701419511"></a>路由器的UUID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797308_row86706419513"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797308_p46700418514"><a name="zh-cn_topic_0168797308_p46700418514"></a><a name="zh-cn_topic_0168797308_p46700418514"></a>internal_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797308_p56701045510"><a name="zh-cn_topic_0168797308_p56701045510"></a><a name="zh-cn_topic_0168797308_p56701045510"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797308_p12670746512"><a name="zh-cn_topic_0168797308_p12670746512"></a><a name="zh-cn_topic_0168797308_p12670746512"></a>NAT网关下行口（DVR的下一跳）所属的network id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797308_row2067015413511"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797308_p76701143516"><a name="zh-cn_topic_0168797308_p76701143516"></a><a name="zh-cn_topic_0168797308_p76701143516"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797308_p86704419513"><a name="zh-cn_topic_0168797308_p86704419513"></a><a name="zh-cn_topic_0168797308_p86704419513"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797308_ul967015411514"></a><a name="zh-cn_topic_0168797308_ul967015411514"></a><ul id="zh-cn_topic_0168797308_ul967015411514"><li>功能说明：NAT网关的状态。</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797308_row76701542515"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797308_p19670443510"><a name="zh-cn_topic_0168797308_p19670443510"></a><a name="zh-cn_topic_0168797308_p19670443510"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797308_p1741454813231"><a name="zh-cn_topic_0168797308_p1741454813231"></a><a name="zh-cn_topic_0168797308_p1741454813231"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797308_ul176703410518"></a><a name="zh-cn_topic_0168797308_ul176703410518"></a><ul id="zh-cn_topic_0168797308_ul176703410518"><li>解冻/冻结状态。</li><li>取值范围：<a name="zh-cn_topic_0168797308_ul11838172814409"></a><a name="zh-cn_topic_0168797308_ul11838172814409"></a><ul id="zh-cn_topic_0168797308_ul11838172814409"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797308_row1967044145114"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797308_p1167011416513"><a name="zh-cn_topic_0168797308_p1167011416513"></a><a name="zh-cn_topic_0168797308_p1167011416513"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797308_p2670141515"><a name="zh-cn_topic_0168797308_p2670141515"></a><a name="zh-cn_topic_0168797308_p2670141515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797308_p193171413220"><a name="zh-cn_topic_0168797308_p193171413220"></a><a name="zh-cn_topic_0168797308_p193171413220"></a>NAT网关的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797308_row6670154195113"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797308_p567013495110"><a name="zh-cn_topic_0168797308_p567013495110"></a><a name="zh-cn_topic_0168797308_p567013495110"></a>dnat_rules_limit</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797308_p467011412512"><a name="zh-cn_topic_0168797308_p467011412512"></a><a name="zh-cn_topic_0168797308_p467011412512"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797308_p1025611101226"><a name="zh-cn_topic_0168797308_p1025611101226"></a><a name="zh-cn_topic_0168797308_p1025611101226"></a>NAT网关的DNAT规则最多条数限制值。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797308_row367011495120"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797308_p136706485112"><a name="zh-cn_topic_0168797308_p136706485112"></a><a name="zh-cn_topic_0168797308_p136706485112"></a>snat_rule_public_ip_limit</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797308_p66701495116"><a name="zh-cn_topic_0168797308_p66701495116"></a><a name="zh-cn_topic_0168797308_p66701495116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797308_p54152113228"><a name="zh-cn_topic_0168797308_p54152113228"></a><a name="zh-cn_topic_0168797308_p54152113228"></a>NAT网关的任意一条SNAT规则最多绑定的弹性公网IP的数量最大限制值。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797308_row19672635205210"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797308_p126571842145215"><a name="zh-cn_topic_0168797308_p126571842145215"></a><a name="zh-cn_topic_0168797308_p126571842145215"></a>billing_info</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797308_p965719427529"><a name="zh-cn_topic_0168797308_p965719427529"></a><a name="zh-cn_topic_0168797308_p965719427529"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797308_p19128172122219"><a name="zh-cn_topic_0168797308_p19128172122219"></a><a name="zh-cn_topic_0168797308_p19128172122219"></a>包周期NAT网关订单关联信息，按需值为空字符串。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797308_row1847184815119"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797308_p16125253105113"><a name="zh-cn_topic_0168797308_p16125253105113"></a><a name="zh-cn_topic_0168797308_p16125253105113"></a>enterprise_project_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797308_p151255530514"><a name="zh-cn_topic_0168797308_p151255530514"></a><a name="zh-cn_topic_0168797308_p151255530514"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797308_ul4125185318515"></a><a name="zh-cn_topic_0168797308_ul4125185318515"></a><ul id="zh-cn_topic_0168797308_ul4125185318515"><li>功能说明：企业项目ID。默认值：0，表示默认企业项目。</li><li>取值范围：最大长度36字节，带 “-”连字符的UUID格式，或者是字符串“0”。</li><li>说明：关于企业项目ID的获取及企业项目特性的详细信息，请参考<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0123692049.html" target="_blank" rel="noopener noreferrer">《企业管理用户指南》</a>。</li></ul>
</td>
</tr>
</tbody>
</table>

## 示例<a name="zh-cn_topic_0168797308_section24937315"></a>

-   请求样例

    ```
    PUT https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/nat_gateways/a78fb3eb-1654-4710-8742-3fc49d5f04f8 
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
             "name": "new_name",
             "dnat_rules_limit": 200,
             "snat_rule_public_ip_limit": 20,
             "enterprise_project_id=0aad99bc-f5f6-4f78-8404-c598d76b0ed2",
             "billing_info": ""
         } 
     } 
    ```


## 状态码<a name="zh-cn_topic_0168797308_section6656623"></a>

请参考[状态码](状态码.md)。

