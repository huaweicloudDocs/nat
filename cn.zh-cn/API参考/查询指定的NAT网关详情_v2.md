# 查询指定的NAT网关详情<a name="nat_apiv2_0007"></a>

## 功能介绍<a name="zh-cn_topic_0168797268_section45827181"></a>

查询指定的NAT网关详情。

## URI<a name="zh-cn_topic_0168797268_section9791447"></a>

GET /v2/\{project\_id\}/nat\_gateways/\{nat\_gateway\_id\}

**表 1**  参数说明

<a name="zh-cn_topic_0168797268_table285161395713"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797268_row12912101317577"><th class="cellrowborder" valign="top" width="22.86771322867713%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797268_p791271313579"><a name="zh-cn_topic_0168797268_p791271313579"></a><a name="zh-cn_topic_0168797268_p791271313579"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.719128087191281%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797268_p1391221355716"><a name="zh-cn_topic_0168797268_p1391221355716"></a><a name="zh-cn_topic_0168797268_p1391221355716"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="9.13908609139086%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797268_p28313120281"><a name="zh-cn_topic_0168797268_p28313120281"></a><a name="zh-cn_topic_0168797268_p28313120281"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="59.27407259274072%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797268_p1191216131572"><a name="zh-cn_topic_0168797268_p1191216131572"></a><a name="zh-cn_topic_0168797268_p1191216131572"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797268_row168823292412"><td class="cellrowborder" valign="top" width="22.86771322867713%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797268_p105814555413"><a name="zh-cn_topic_0168797268_p105814555413"></a><a name="zh-cn_topic_0168797268_p105814555413"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.719128087191281%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797268_p1558110558417"><a name="zh-cn_topic_0168797268_p1558110558417"></a><a name="zh-cn_topic_0168797268_p1558110558417"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="9.13908609139086%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797268_p78393112285"><a name="zh-cn_topic_0168797268_p78393112285"></a><a name="zh-cn_topic_0168797268_p78393112285"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="59.27407259274072%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797268_p1858135513411"><a name="zh-cn_topic_0168797268_p1858135513411"></a><a name="zh-cn_topic_0168797268_p1858135513411"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797268_row1591281345717"><td class="cellrowborder" valign="top" width="22.86771322867713%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797268_p69121213115717"><a name="zh-cn_topic_0168797268_p69121213115717"></a><a name="zh-cn_topic_0168797268_p69121213115717"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.719128087191281%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797268_p1291281325710"><a name="zh-cn_topic_0168797268_p1291281325710"></a><a name="zh-cn_topic_0168797268_p1291281325710"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="9.13908609139086%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797268_p6836317289"><a name="zh-cn_topic_0168797268_p6836317289"></a><a name="zh-cn_topic_0168797268_p6836317289"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="59.27407259274072%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797268_p20912111395719"><a name="zh-cn_topic_0168797268_p20912111395719"></a><a name="zh-cn_topic_0168797268_p20912111395719"></a>NAT网关的id。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0168797268_section54909781"></a>

无

## 响应消息<a name="zh-cn_topic_0168797268_section24425986"></a>

响应参数如[表2](#zh-cn_topic_0168797268_table129831149144215)所示。

**表 2**  响应参数

<a name="zh-cn_topic_0168797268_table129831149144215"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797268_row2233175015424"><th class="cellrowborder" valign="top" width="20.200000000000003%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797268_p112331950124213"><a name="zh-cn_topic_0168797268_p112331950124213"></a><a name="zh-cn_topic_0168797268_p112331950124213"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="21.45%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797268_p1023335020429"><a name="zh-cn_topic_0168797268_p1023335020429"></a><a name="zh-cn_topic_0168797268_p1023335020429"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.35%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797268_p1123319502426"><a name="zh-cn_topic_0168797268_p1123319502426"></a><a name="zh-cn_topic_0168797268_p1123319502426"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797268_row1223325010421"><td class="cellrowborder" valign="top" width="20.200000000000003%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797268_p202331450134211"><a name="zh-cn_topic_0168797268_p202331450134211"></a><a name="zh-cn_topic_0168797268_p202331450134211"></a>nat_gateway</p>
</td>
<td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797268_p12331150184217"><a name="zh-cn_topic_0168797268_p12331150184217"></a><a name="zh-cn_topic_0168797268_p12331150184217"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="58.35%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797268_p62331505427"><a name="zh-cn_topic_0168797268_p62331505427"></a><a name="zh-cn_topic_0168797268_p62331505427"></a>nat_gateway对象。请参考<a href="#zh-cn_topic_0168797268_table514165011429">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  nat\_gateway字段说明

<a name="zh-cn_topic_0168797268_table514165011429"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797268_row1233175044210"><th class="cellrowborder" valign="top" width="20.66%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797268_p16233350194217"><a name="zh-cn_topic_0168797268_p16233350194217"></a><a name="zh-cn_topic_0168797268_p16233350194217"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.75%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797268_p1123375010428"><a name="zh-cn_topic_0168797268_p1123375010428"></a><a name="zh-cn_topic_0168797268_p1123375010428"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.589999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797268_p2023313507424"><a name="zh-cn_topic_0168797268_p2023313507424"></a><a name="zh-cn_topic_0168797268_p2023313507424"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797268_row623313504427"><td class="cellrowborder" valign="top" width="20.66%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797268_p162338502421"><a name="zh-cn_topic_0168797268_p162338502421"></a><a name="zh-cn_topic_0168797268_p162338502421"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20.75%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797268_p92331950144219"><a name="zh-cn_topic_0168797268_p92331950144219"></a><a name="zh-cn_topic_0168797268_p92331950144219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797268_p5233165034219"><a name="zh-cn_topic_0168797268_p5233165034219"></a><a name="zh-cn_topic_0168797268_p5233165034219"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797268_row72331550164211"><td class="cellrowborder" valign="top" width="20.66%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797268_p1123335024220"><a name="zh-cn_topic_0168797268_p1123335024220"></a><a name="zh-cn_topic_0168797268_p1123335024220"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.75%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797268_p8233450174216"><a name="zh-cn_topic_0168797268_p8233450174216"></a><a name="zh-cn_topic_0168797268_p8233450174216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797268_p172332504428"><a name="zh-cn_topic_0168797268_p172332504428"></a><a name="zh-cn_topic_0168797268_p172332504428"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797268_row17233185084220"><td class="cellrowborder" valign="top" width="20.66%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797268_p323355014426"><a name="zh-cn_topic_0168797268_p323355014426"></a><a name="zh-cn_topic_0168797268_p323355014426"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20.75%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797268_p323355044218"><a name="zh-cn_topic_0168797268_p323355044218"></a><a name="zh-cn_topic_0168797268_p323355044218"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797268_p42331650144212"><a name="zh-cn_topic_0168797268_p42331650144212"></a><a name="zh-cn_topic_0168797268_p42331650144212"></a>NAT网关的名字。</p>
<p id="zh-cn_topic_0168797268_p72333505429"><a name="zh-cn_topic_0168797268_p72333505429"></a><a name="zh-cn_topic_0168797268_p72333505429"></a>NAT网关的名字仅支持数字、字母、_（下划线）、-（中划线）、中文。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797268_row1623315018422"><td class="cellrowborder" valign="top" width="20.66%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797268_p19233145020424"><a name="zh-cn_topic_0168797268_p19233145020424"></a><a name="zh-cn_topic_0168797268_p19233145020424"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20.75%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797268_p423318503426"><a name="zh-cn_topic_0168797268_p423318503426"></a><a name="zh-cn_topic_0168797268_p423318503426"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797268_p923335014212"><a name="zh-cn_topic_0168797268_p923335014212"></a><a name="zh-cn_topic_0168797268_p923335014212"></a>NAT网关的描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797268_row1623315506427"><td class="cellrowborder" valign="top" width="20.66%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797268_p18233350184218"><a name="zh-cn_topic_0168797268_p18233350184218"></a><a name="zh-cn_topic_0168797268_p18233350184218"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="20.75%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797268_p15233105018428"><a name="zh-cn_topic_0168797268_p15233105018428"></a><a name="zh-cn_topic_0168797268_p15233105018428"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797268_p1023385084218"><a name="zh-cn_topic_0168797268_p1023385084218"></a><a name="zh-cn_topic_0168797268_p1023385084218"></a>NAT网关的规格。</p>
<p id="zh-cn_topic_0168797268_p1223319508422"><a name="zh-cn_topic_0168797268_p1223319508422"></a><a name="zh-cn_topic_0168797268_p1223319508422"></a>取值为：</p>
<a name="zh-cn_topic_0168797268_ul132334508424"></a><a name="zh-cn_topic_0168797268_ul132334508424"></a><ul id="zh-cn_topic_0168797268_ul132334508424"><li>“1”：小型，SNAT最大连接数10000</li><li>“2”：中型，SNAT最大连接数50000</li><li>“3”：大型，SNAT最大连接数200000</li><li>“4”：超大型，SNAT最大连接数1000000</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797268_row42331050144212"><td class="cellrowborder" valign="top" width="20.66%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797268_p1723325015428"><a name="zh-cn_topic_0168797268_p1723325015428"></a><a name="zh-cn_topic_0168797268_p1723325015428"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.75%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797268_p3233115094213"><a name="zh-cn_topic_0168797268_p3233115094213"></a><a name="zh-cn_topic_0168797268_p3233115094213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797268_p102331150144211"><a name="zh-cn_topic_0168797268_p102331150144211"></a><a name="zh-cn_topic_0168797268_p102331150144211"></a>路由器的UUID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797268_row72331650164215"><td class="cellrowborder" valign="top" width="20.66%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797268_p8233195017429"><a name="zh-cn_topic_0168797268_p8233195017429"></a><a name="zh-cn_topic_0168797268_p8233195017429"></a>internal_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.75%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797268_p223314508421"><a name="zh-cn_topic_0168797268_p223314508421"></a><a name="zh-cn_topic_0168797268_p223314508421"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797268_p4233125084214"><a name="zh-cn_topic_0168797268_p4233125084214"></a><a name="zh-cn_topic_0168797268_p4233125084214"></a>NAT网关下行口（DVR的下一跳）所属的network id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797268_row102339502423"><td class="cellrowborder" valign="top" width="20.66%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797268_p82331150114212"><a name="zh-cn_topic_0168797268_p82331150114212"></a><a name="zh-cn_topic_0168797268_p82331150114212"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20.75%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797268_p1823311508429"><a name="zh-cn_topic_0168797268_p1823311508429"></a><a name="zh-cn_topic_0168797268_p1823311508429"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797268_ul9233155034214"></a><a name="zh-cn_topic_0168797268_ul9233155034214"></a><ul id="zh-cn_topic_0168797268_ul9233155034214"><li>功能说明：NAT网关的状态。</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797268_row20233450104210"><td class="cellrowborder" valign="top" width="20.66%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797268_p32333502427"><a name="zh-cn_topic_0168797268_p32333502427"></a><a name="zh-cn_topic_0168797268_p32333502427"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="20.75%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797268_p12233650124214"><a name="zh-cn_topic_0168797268_p12233650124214"></a><a name="zh-cn_topic_0168797268_p12233650124214"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797268_ul71858556358"></a><a name="zh-cn_topic_0168797268_ul71858556358"></a><ul id="zh-cn_topic_0168797268_ul71858556358"><li>解冻/冻结状态。</li><li>取值范围：<a name="zh-cn_topic_0168797268_ul11838172814409"></a><a name="zh-cn_topic_0168797268_ul11838172814409"></a><ul id="zh-cn_topic_0168797268_ul11838172814409"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797268_row22331050154211"><td class="cellrowborder" valign="top" width="20.66%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797268_p723305014427"><a name="zh-cn_topic_0168797268_p723305014427"></a><a name="zh-cn_topic_0168797268_p723305014427"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="20.75%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797268_p423312509427"><a name="zh-cn_topic_0168797268_p423312509427"></a><a name="zh-cn_topic_0168797268_p423312509427"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797268_p1374571812110"><a name="zh-cn_topic_0168797268_p1374571812110"></a><a name="zh-cn_topic_0168797268_p1374571812110"></a>NAT网关的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797268_row22335505423"><td class="cellrowborder" valign="top" width="20.66%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797268_p1023355016427"><a name="zh-cn_topic_0168797268_p1023355016427"></a><a name="zh-cn_topic_0168797268_p1023355016427"></a>dnat_rules_limit</p>
</td>
<td class="cellrowborder" valign="top" width="20.75%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797268_p723325014423"><a name="zh-cn_topic_0168797268_p723325014423"></a><a name="zh-cn_topic_0168797268_p723325014423"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797268_ul162332503424"></a><a name="zh-cn_topic_0168797268_ul162332503424"></a><ul id="zh-cn_topic_0168797268_ul162332503424"><li>NAT网关的DNAT规则最多条数限制值</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797268_row1323310501424"><td class="cellrowborder" valign="top" width="20.66%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797268_p152331950164220"><a name="zh-cn_topic_0168797268_p152331950164220"></a><a name="zh-cn_topic_0168797268_p152331950164220"></a>snat_rule_public_ip_limit</p>
</td>
<td class="cellrowborder" valign="top" width="20.75%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797268_p14233550164219"><a name="zh-cn_topic_0168797268_p14233550164219"></a><a name="zh-cn_topic_0168797268_p14233550164219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797268_ul923365014217"></a><a name="zh-cn_topic_0168797268_ul923365014217"></a><ul id="zh-cn_topic_0168797268_ul923365014217"><li>NAT网关的任意一条SNAT规则最多绑定的弹性公网IP的数量最大限制值。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797268_row23472010154515"><td class="cellrowborder" valign="top" width="20.66%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797268_p176051213458"><a name="zh-cn_topic_0168797268_p176051213458"></a><a name="zh-cn_topic_0168797268_p176051213458"></a>billing_info</p>
</td>
<td class="cellrowborder" valign="top" width="20.75%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797268_p1260520218454"><a name="zh-cn_topic_0168797268_p1260520218454"></a><a name="zh-cn_topic_0168797268_p1260520218454"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797268_p1084224152118"><a name="zh-cn_topic_0168797268_p1084224152118"></a><a name="zh-cn_topic_0168797268_p1084224152118"></a>包周期NAT网关订单关联信息，按需值为空字符串。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797268_row18741113314515"><td class="cellrowborder" valign="top" width="20.66%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797268_p187473370512"><a name="zh-cn_topic_0168797268_p187473370512"></a><a name="zh-cn_topic_0168797268_p187473370512"></a>enterprise_project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.75%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797268_p1874773717512"><a name="zh-cn_topic_0168797268_p1874773717512"></a><a name="zh-cn_topic_0168797268_p1874773717512"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797268_ul1174733719512"></a><a name="zh-cn_topic_0168797268_ul1174733719512"></a><ul id="zh-cn_topic_0168797268_ul1174733719512"><li>功能说明：企业项目ID。默认值：0，表示默认企业项目。</li><li>取值范围：最大长度36字节，带 “-”连字符的UUID格式，或者是字符串“0”。</li><li>说明：关于企业项目ID的获取及企业项目特性的详细信息，请参考<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0123692049.html" target="_blank" rel="noopener noreferrer">《企业管理用户指南》</a>。</li></ul>
</td>
</tr>
</tbody>
</table>

## 示例<a name="zh-cn_topic_0168797268_section18507287"></a>

-   请求样例

    ```
    GET https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/nat_gateways/a78fb3eb-1654-4710-8742-3fc49d5f04f8
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
             "name": "nat_001",
             "dnat_rules_limit": 200,
             "snat_rule_public_ip_limit": 20,
             "enterprise_project_id=0aad99bc-f5f6-4f78-8404-c598d76b0ed2",
             "billing_info": ""
         } 
     }
    ```


## 状态码<a name="zh-cn_topic_0168797268_section22695302"></a>

请参考[状态码](状态码.md)。

