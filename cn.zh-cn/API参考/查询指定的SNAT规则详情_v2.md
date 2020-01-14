# 查询指定的SNAT规则详情<a name="nat_apiv2_0013"></a>

## 功能介绍<a name="zh-cn_topic_0168797284_section59567946"></a>

查询指定的SNAT规则详情。

## URI<a name="zh-cn_topic_0168797284_section66349468"></a>

GET /v2/\{project\_id\}/snat\_rules/\{snat\_rule\_id\}

**表 1**  参数说明

<a name="zh-cn_topic_0168797284_table1910716134591"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797284_row3169413135915"><th class="cellrowborder" valign="top" width="24.537546245375463%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797284_p16169131375910"><a name="zh-cn_topic_0168797284_p16169131375910"></a><a name="zh-cn_topic_0168797284_p16169131375910"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="9.359064093590641%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797284_p151699135593"><a name="zh-cn_topic_0168797284_p151699135593"></a><a name="zh-cn_topic_0168797284_p151699135593"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20.11798820117988%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797284_p9368111711350"><a name="zh-cn_topic_0168797284_p9368111711350"></a><a name="zh-cn_topic_0168797284_p9368111711350"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="45.98540145985402%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797284_p016991320594"><a name="zh-cn_topic_0168797284_p016991320594"></a><a name="zh-cn_topic_0168797284_p016991320594"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797284_row14497565254"><td class="cellrowborder" valign="top" width="24.537546245375463%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797284_p1154781214258"><a name="zh-cn_topic_0168797284_p1154781214258"></a><a name="zh-cn_topic_0168797284_p1154781214258"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="9.359064093590641%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797284_p55472124251"><a name="zh-cn_topic_0168797284_p55472124251"></a><a name="zh-cn_topic_0168797284_p55472124251"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.11798820117988%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797284_p1536820170351"><a name="zh-cn_topic_0168797284_p1536820170351"></a><a name="zh-cn_topic_0168797284_p1536820170351"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.98540145985402%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797284_p12547101210255"><a name="zh-cn_topic_0168797284_p12547101210255"></a><a name="zh-cn_topic_0168797284_p12547101210255"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797284_row131691913145916"><td class="cellrowborder" valign="top" width="24.537546245375463%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797284_p116919133595"><a name="zh-cn_topic_0168797284_p116919133595"></a><a name="zh-cn_topic_0168797284_p116919133595"></a>snat_rule_id</p>
</td>
<td class="cellrowborder" valign="top" width="9.359064093590641%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797284_p6169171310597"><a name="zh-cn_topic_0168797284_p6169171310597"></a><a name="zh-cn_topic_0168797284_p6169171310597"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.11798820117988%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797284_p14368181753511"><a name="zh-cn_topic_0168797284_p14368181753511"></a><a name="zh-cn_topic_0168797284_p14368181753511"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.98540145985402%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797284_p31691313145913"><a name="zh-cn_topic_0168797284_p31691313145913"></a><a name="zh-cn_topic_0168797284_p31691313145913"></a>SNAT规则的id。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0168797284_section5597798"></a>

无

## 响应消息<a name="zh-cn_topic_0168797284_section50380184"></a>

响应参数如[表2](#zh-cn_topic_0168797284_table65459315)所示。

**表 2**  响应参数

<a name="zh-cn_topic_0168797284_table65459315"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797284_row47811128"><th class="cellrowborder" valign="top" width="20.73%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797284_p47496137"><a name="zh-cn_topic_0168797284_p47496137"></a><a name="zh-cn_topic_0168797284_p47496137"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="28.050000000000004%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797284_p21981920"><a name="zh-cn_topic_0168797284_p21981920"></a><a name="zh-cn_topic_0168797284_p21981920"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797284_p6428601"><a name="zh-cn_topic_0168797284_p6428601"></a><a name="zh-cn_topic_0168797284_p6428601"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797284_row50954701"><td class="cellrowborder" valign="top" width="20.73%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797284_p33690117"><a name="zh-cn_topic_0168797284_p33690117"></a><a name="zh-cn_topic_0168797284_p33690117"></a>snat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="28.050000000000004%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797284_p44544970"><a name="zh-cn_topic_0168797284_p44544970"></a><a name="zh-cn_topic_0168797284_p44544970"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797284_p447513"><a name="zh-cn_topic_0168797284_p447513"></a><a name="zh-cn_topic_0168797284_p447513"></a>snat_rule对象。请参考<a href="#zh-cn_topic_0168797284_table113261845122312">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  snat\_rule字段说明

<a name="zh-cn_topic_0168797284_table113261845122312"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797284_row3326164512310"><th class="cellrowborder" valign="top" width="21.04210421042104%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797284_p144282010346"><a name="zh-cn_topic_0168797284_p144282010346"></a><a name="zh-cn_topic_0168797284_p144282010346"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="27.722772277227726%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797284_p1742881017412"><a name="zh-cn_topic_0168797284_p1742881017412"></a><a name="zh-cn_topic_0168797284_p1742881017412"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.23512351235123%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797284_p1442813106416"><a name="zh-cn_topic_0168797284_p1442813106416"></a><a name="zh-cn_topic_0168797284_p1442813106416"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797284_row73267459231"><td class="cellrowborder" valign="top" width="21.04210421042104%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797284_p277043414264"><a name="zh-cn_topic_0168797284_p277043414264"></a><a name="zh-cn_topic_0168797284_p277043414264"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797284_p477113419260"><a name="zh-cn_topic_0168797284_p477113419260"></a><a name="zh-cn_topic_0168797284_p477113419260"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.23512351235123%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797284_p187711342265"><a name="zh-cn_topic_0168797284_p187711342265"></a><a name="zh-cn_topic_0168797284_p187711342265"></a>SNAT规则的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797284_row11326845102317"><td class="cellrowborder" valign="top" width="21.04210421042104%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797284_p14771113482614"><a name="zh-cn_topic_0168797284_p14771113482614"></a><a name="zh-cn_topic_0168797284_p14771113482614"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797284_p177112342260"><a name="zh-cn_topic_0168797284_p177112342260"></a><a name="zh-cn_topic_0168797284_p177112342260"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.23512351235123%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797284_p4771153412265"><a name="zh-cn_topic_0168797284_p4771153412265"></a><a name="zh-cn_topic_0168797284_p4771153412265"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797284_row13261445132318"><td class="cellrowborder" valign="top" width="21.04210421042104%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797284_p147711234172619"><a name="zh-cn_topic_0168797284_p147711234172619"></a><a name="zh-cn_topic_0168797284_p147711234172619"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797284_p777153419268"><a name="zh-cn_topic_0168797284_p777153419268"></a><a name="zh-cn_topic_0168797284_p777153419268"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.23512351235123%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797284_p13771193402618"><a name="zh-cn_topic_0168797284_p13771193402618"></a><a name="zh-cn_topic_0168797284_p13771193402618"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797284_row2032617455238"><td class="cellrowborder" valign="top" width="21.04210421042104%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797284_p27711634142612"><a name="zh-cn_topic_0168797284_p27711634142612"></a><a name="zh-cn_topic_0168797284_p27711634142612"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797284_p47713345265"><a name="zh-cn_topic_0168797284_p47713345265"></a><a name="zh-cn_topic_0168797284_p47713345265"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.23512351235123%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797284_p1477173418267"><a name="zh-cn_topic_0168797284_p1477173418267"></a><a name="zh-cn_topic_0168797284_p1477173418267"></a>规则使用的网络id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797284_row1632610451230"><td class="cellrowborder" valign="top" width="21.04210421042104%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797284_p15771193452617"><a name="zh-cn_topic_0168797284_p15771193452617"></a><a name="zh-cn_topic_0168797284_p15771193452617"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797284_p11771103402617"><a name="zh-cn_topic_0168797284_p11771103402617"></a><a name="zh-cn_topic_0168797284_p11771103402617"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.23512351235123%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797284_p9771123413265"><a name="zh-cn_topic_0168797284_p9771123413265"></a><a name="zh-cn_topic_0168797284_p9771123413265"></a>cidr，vpc 子网网段的子集或专线侧网段。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797284_row11326645162317"><td class="cellrowborder" valign="top" width="21.04210421042104%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797284_p1177153414264"><a name="zh-cn_topic_0168797284_p1177153414264"></a><a name="zh-cn_topic_0168797284_p1177153414264"></a>source_type</p>
</td>
<td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797284_p673291135216"><a name="zh-cn_topic_0168797284_p673291135216"></a><a name="zh-cn_topic_0168797284_p673291135216"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="51.23512351235123%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797284_p3771123432614"><a name="zh-cn_topic_0168797284_p3771123432614"></a><a name="zh-cn_topic_0168797284_p3771123432614"></a>0：VPC侧，可以指定network_id 或者cidr</p>
<p id="zh-cn_topic_0168797284_p1477163422610"><a name="zh-cn_topic_0168797284_p1477163422610"></a><a name="zh-cn_topic_0168797284_p1477163422610"></a>1：专线侧，只能指定cidr</p>
<p id="zh-cn_topic_0168797284_p3771163472614"><a name="zh-cn_topic_0168797284_p3771163472614"></a><a name="zh-cn_topic_0168797284_p3771163472614"></a>不输入默认为0（VPC）</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797284_row4326104512234"><td class="cellrowborder" valign="top" width="21.04210421042104%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797284_p7771183419260"><a name="zh-cn_topic_0168797284_p7771183419260"></a><a name="zh-cn_topic_0168797284_p7771183419260"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797284_p137711134192620"><a name="zh-cn_topic_0168797284_p137711134192620"></a><a name="zh-cn_topic_0168797284_p137711134192620"></a>String(4096)</p>
</td>
<td class="cellrowborder" valign="top" width="51.23512351235123%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797284_ul1777153492615"></a><a name="zh-cn_topic_0168797284_ul1777153492615"></a><ul id="zh-cn_topic_0168797284_ul1777153492615"><li>功能说明：弹性公网IP的id，多个弹性公网IP使用逗号分隔。</li><li>取值范围：最大长度4096字节。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797284_row2785103161819"><td class="cellrowborder" valign="top" width="21.04210421042104%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797284_p77711434122610"><a name="zh-cn_topic_0168797284_p77711434122610"></a><a name="zh-cn_topic_0168797284_p77711434122610"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797284_p9771534182618"><a name="zh-cn_topic_0168797284_p9771534182618"></a><a name="zh-cn_topic_0168797284_p9771534182618"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="51.23512351235123%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797284_p10771234122616"><a name="zh-cn_topic_0168797284_p10771234122616"></a><a name="zh-cn_topic_0168797284_p10771234122616"></a>SNAT规则的描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797284_row62381927111816"><td class="cellrowborder" valign="top" width="21.04210421042104%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797284_p4772234182617"><a name="zh-cn_topic_0168797284_p4772234182617"></a><a name="zh-cn_topic_0168797284_p4772234182617"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797284_p157726343268"><a name="zh-cn_topic_0168797284_p157726343268"></a><a name="zh-cn_topic_0168797284_p157726343268"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.23512351235123%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797284_ul67723342269"></a><a name="zh-cn_topic_0168797284_ul67723342269"></a><ul id="zh-cn_topic_0168797284_ul67723342269"><li>功能说明：SNAT规则的状态。</li><li>取值范围：<u id="zh-cn_topic_0168797284_u377263414265"><a name="zh-cn_topic_0168797284_u377263414265"></a><a name="zh-cn_topic_0168797284_u377263414265"></a><u id="zh-cn_topic_0168797284_u0772173422619"><a name="zh-cn_topic_0168797284_u0772173422619"></a><a name="zh-cn_topic_0168797284_u0772173422619"></a><a href="资源状态说明.md">资源状态说明</a></u></u>。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797284_row11326184562315"><td class="cellrowborder" valign="top" width="21.04210421042104%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797284_p47722034192616"><a name="zh-cn_topic_0168797284_p47722034192616"></a><a name="zh-cn_topic_0168797284_p47722034192616"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797284_p82513253268"><a name="zh-cn_topic_0168797284_p82513253268"></a><a name="zh-cn_topic_0168797284_p82513253268"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="51.23512351235123%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797284_ul71858556358"></a><a name="zh-cn_topic_0168797284_ul71858556358"></a><ul id="zh-cn_topic_0168797284_ul71858556358"><li>解冻/冻结状态。</li><li>取值范围：<a name="zh-cn_topic_0168797284_ul11838172814409"></a><a name="zh-cn_topic_0168797284_ul11838172814409"></a><ul id="zh-cn_topic_0168797284_ul11838172814409"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797284_row932614518236"><td class="cellrowborder" valign="top" width="21.04210421042104%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797284_p137721134102614"><a name="zh-cn_topic_0168797284_p137721134102614"></a><a name="zh-cn_topic_0168797284_p137721134102614"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797284_p2772143432610"><a name="zh-cn_topic_0168797284_p2772143432610"></a><a name="zh-cn_topic_0168797284_p2772143432610"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.23512351235123%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797284_p85641346102413"><a name="zh-cn_topic_0168797284_p85641346102413"></a><a name="zh-cn_topic_0168797284_p85641346102413"></a>SNAT规则的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797284_row3326134518239"><td class="cellrowborder" valign="top" width="21.04210421042104%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797284_p17772113422615"><a name="zh-cn_topic_0168797284_p17772113422615"></a><a name="zh-cn_topic_0168797284_p17772113422615"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797284_p12772534172610"><a name="zh-cn_topic_0168797284_p12772534172610"></a><a name="zh-cn_topic_0168797284_p12772534172610"></a>String(1024)</p>
</td>
<td class="cellrowborder" valign="top" width="51.23512351235123%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797284_ul277273442611"></a><a name="zh-cn_topic_0168797284_ul277273442611"></a><ul id="zh-cn_topic_0168797284_ul277273442611"><li>功能说明：弹性公网IP，多个弹性公网IP使用逗号分隔。</li><li>取值范围：最大长度1024字节。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797284_row1932664512234"><td class="cellrowborder" valign="top" width="21.04210421042104%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797284_p12772103442617"><a name="zh-cn_topic_0168797284_p12772103442617"></a><a name="zh-cn_topic_0168797284_p12772103442617"></a>freezed_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797284_p97721334182615"><a name="zh-cn_topic_0168797284_p97721334182615"></a><a name="zh-cn_topic_0168797284_p97721334182615"></a>String(1024)</p>
</td>
<td class="cellrowborder" valign="top" width="51.23512351235123%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797284_ul1777293472612"></a><a name="zh-cn_topic_0168797284_ul1777293472612"></a><ul id="zh-cn_topic_0168797284_ul1777293472612"><li>功能说明：冻结的弹性公网IP，多个冻结的弹性公网IP使用逗号分隔。</li><li>取值范围：最大长度1024字节。</li></ul>
</td>
</tr>
</tbody>
</table>

## 示例<a name="zh-cn_topic_0168797284_section50768476"></a>

-   请求样例

    ```
    GET https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/snat_rules/5b95c675-69c2-4656-ba06-58ff72e1d338
    ```


-   响应样例

    ```
    { 
         "snat_rule": { 
             "floating_ip_id": "bdc10a4c-d81a-41ec-adf7-de857f7c812a", 
             "status": "ACTIVE", 
             "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8", 
             "admin_state_up": true, 
             "network_id": "eaad9cd6-2372-4be1-9535-9bd37210ae7b",
             "source_type":0,
             "tenant_id": "d199ba7e0ba64899b2e81518104b1526", 
             "created_at": "2017-11-18 07:54:21.665430", 
             "id": "5b95c675-69c2-4656-ba06-58ff72e1d338", 
             "floating_ip_address": "5.21.11.226", 
             "freezed_ip_address": "", 
             "description": "my snat rule 01" 
         } 
     }
    ```


## 状态码<a name="zh-cn_topic_0168797284_section1941962013172"></a>

请参考[状态码](状态码.md)。

