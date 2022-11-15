# 更新SNAT规则<a name="UpdateNatGatewaySnatRule"></a>

## 功能介绍<a name="section194439566308"></a>

更新指定的SNAT规则。

## 接口约束<a name="section34521356173014"></a>

-   更新弹性公网IP的id时，要求SNAT规则状态status = ACTIVE，要求网关管理员状态admin\_state\_up = True。
-   更新描述时，要求SNAT规则状态status = ACTIVE，要求网关管理员状态admin\_state\_up = True。

## 调试<a name="section04590562302"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=nat&api=UpdateNatGatewaySnatRule)中调试该接口。

## URI<a name="section11470175616304"></a>

PUT /v2/\{project\_id\}/snat\_rules/\{snat\_rule\_id\}

**表 1**  路径参数

<a name="table3479256113018"></a>
<table><thead align="left"><tr id="row44771956103017"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p248245663012"><a name="p248245663012"></a><a name="p248245663012"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p1648585613014"><a name="p1648585613014"></a><a name="p1648585613014"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1048845612303"><a name="p1048845612303"></a><a name="p1048845612303"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p1749219567305"><a name="p1749219567305"></a><a name="p1749219567305"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row2047719567302"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p249525633010"><a name="p249525633010"></a><a name="p249525633010"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p154983569300"><a name="p154983569300"></a><a name="p154983569300"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p185029561304"><a name="p185029561304"></a><a name="p185029561304"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p750710568303"><a name="p750710568303"></a><a name="p750710568303"></a>项目的ID。</p>
<p id="p1151015610308"><a name="p1151015610308"></a><a name="p1151015610308"></a>最小长度：<strong id="b85111456163010"><a name="b85111456163010"></a><a name="b85111456163010"></a>1</strong></p>
<p id="p85136562303"><a name="p85136562303"></a><a name="p85136562303"></a>最大长度：<strong id="b55141056153018"><a name="b55141056153018"></a><a name="b55141056153018"></a>36</strong></p>
<p id="p2562026131319"><a name="p2562026131319"></a><a name="p2562026131319"></a>获取方法详见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row1047855643016"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p18517115633014"><a name="p18517115633014"></a><a name="p18517115633014"></a>snat_rule_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1521115619303"><a name="p1521115619303"></a><a name="p1521115619303"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p052585603010"><a name="p052585603010"></a><a name="p052585603010"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p195292561300"><a name="p195292561300"></a><a name="p195292561300"></a>SNAT规则的ID。</p>
<p id="p1533956133013"><a name="p1533956133013"></a><a name="p1533956133013"></a>长度：<strong id="b3534156193010"><a name="b3534156193010"></a><a name="b3534156193010"></a>36</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section0542165615305"></a>

**表 2**  请求Header参数

<a name="zh-cn_topic_0297140340_HeaderParameter"></a>
<table><thead align="left"><tr id="row115471056123011"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p9551156143018"><a name="p9551156143018"></a><a name="p9551156143018"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p13555956163010"><a name="p13555956163010"></a><a name="p13555956163010"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p455919560303"><a name="p455919560303"></a><a name="p455919560303"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p85621956183010"><a name="p85621956183010"></a><a name="p85621956183010"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row55473565302"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p656525693015"><a name="p656525693015"></a><a name="p656525693015"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p55691656163011"><a name="p55691656163011"></a><a name="p55691656163011"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p257455603018"><a name="p257455603018"></a><a name="p257455603018"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p857835603013"><a name="p857835603013"></a><a name="p857835603013"></a>用户Token。用户Token也就是调用获取用户Token获取请求认证接口的响应值，该接口是唯一不需要认证的接口。请求响应成功后在响应消息头中包含的“X-Subject-Token”的值即为Token值。</p>
<p id="p1058145683020"><a name="p1058145683020"></a><a name="p1058145683020"></a>最小长度：<strong id="b8582105653012"><a name="b8582105653012"></a><a name="b8582105653012"></a>1</strong></p>
<p id="p5584135616308"><a name="p5584135616308"></a><a name="p5584135616308"></a>最大长度：<strong id="b258515563301"><a name="b258515563301"></a><a name="b258515563301"></a>10240</strong></p>
</td>
</tr>
</tbody>
</table>

**表 3**  请求Body参数

<a name="zh-cn_topic_0297140340_requestParameter"></a>
<table><thead align="left"><tr id="row8587456173012"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1859218561304"><a name="p1859218561304"></a><a name="p1859218561304"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p2059545613018"><a name="p2059545613018"></a><a name="p2059545613018"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p115986566302"><a name="p115986566302"></a><a name="p115986566302"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p106021856143012"><a name="p106021856143012"></a><a name="p106021856143012"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row205887568302"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p17606115613303"><a name="p17606115613303"></a><a name="p17606115613303"></a>snat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1061175618308"><a name="p1061175618308"></a><a name="p1061175618308"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p76151956103019"><a name="p76151956103019"></a><a name="p76151956103019"></a><a href="#zh-cn_topic_0297140340_request_UpdateNatGatewaySnatRuleOption">UpdateNatGatewaySnatRuleOption</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p961985618303"><a name="p961985618303"></a><a name="p961985618303"></a>更新SNAT规则的请求体。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  UpdateNatGatewaySnatRuleOption

<a name="zh-cn_topic_0297140340_request_UpdateNatGatewaySnatRuleOption"></a>
<table><thead align="left"><tr id="row8621185643015"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p46258565303"><a name="p46258565303"></a><a name="p46258565303"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p1262917564301"><a name="p1262917564301"></a><a name="p1262917564301"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p7632115683014"><a name="p7632115683014"></a><a name="p7632115683014"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p863675653012"><a name="p863675653012"></a><a name="p863675653012"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row13622756183018"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p12639185618303"><a name="p12639185618303"></a><a name="p12639185618303"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p17643856133013"><a name="p17643856133013"></a><a name="p17643856133013"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p13647115623016"><a name="p13647115623016"></a><a name="p13647115623016"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p565045613301"><a name="p565045613301"></a><a name="p565045613301"></a>公网NAT网关的id。</p>
</td>
</tr>
<tr id="row196228568301"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p10654145616303"><a name="p10654145616303"></a><a name="p10654145616303"></a>public_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1565715673017"><a name="p1565715673017"></a><a name="p1565715673017"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p2661195616302"><a name="p2661195616302"></a><a name="p2661195616302"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p166641568308"><a name="p166641568308"></a><a name="p166641568308"></a>功能说明：弹性公网IP，多个弹性公网IP使用逗号分隔。取值范围：最大长度1024字节。约束：弹性公网IP的id个数不能超过20个</p>
</td>
</tr>
<tr id="row1762255613308"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1566715561302"><a name="p1566715561302"></a><a name="p1566715561302"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p146711756123013"><a name="p146711756123013"></a><a name="p146711756123013"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p867515560302"><a name="p867515560302"></a><a name="p867515560302"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p7680356133013"><a name="p7680356133013"></a><a name="p7680356133013"></a>SNAT规则的描述，长度限制为255。</p>
<p id="p1368355616306"><a name="p1368355616306"></a><a name="p1368355616306"></a>最大长度：<strong id="b17684115693018"><a name="b17684115693018"></a><a name="b17684115693018"></a>255</strong></p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section268725618303"></a>

**状态码： 200**

**表 5**  响应Body参数

<a name="zh-cn_topic_0297140340_responseParameter"></a>
<table><thead align="left"><tr id="row146942561308"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1269815616300"><a name="p1269815616300"></a><a name="p1269815616300"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p77011456153010"><a name="p77011456153010"></a><a name="p77011456153010"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p2704856103019"><a name="p2704856103019"></a><a name="p2704856103019"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row16941556183011"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p5707756123017"><a name="p5707756123017"></a><a name="p5707756123017"></a>snat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1071265633017"><a name="p1071265633017"></a><a name="p1071265633017"></a><a href="#zh-cn_topic_0297140340_response_NatGatewaySnatRuleResponseBody">NatGatewaySnatRuleResponseBody</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p6715125683018"><a name="p6715125683018"></a><a name="p6715125683018"></a>SNAT规则的响应体。</p>
</td>
</tr>
</tbody>
</table>

**表 6**  NatGatewaySnatRuleResponseBody

<a name="zh-cn_topic_0297140340_response_NatGatewaySnatRuleResponseBody"></a>
<table><thead align="left"><tr id="row167201956183016"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p17725256113016"><a name="p17725256113016"></a><a name="p17725256113016"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p107291156183016"><a name="p107291156183016"></a><a name="p107291156183016"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p573275615307"><a name="p573275615307"></a><a name="p573275615307"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row172045620301"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4736256173010"><a name="p4736256173010"></a><a name="p4736256173010"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p173955620301"><a name="p173955620301"></a><a name="p173955620301"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17441456183015"><a name="p17441456183015"></a><a name="p17441456183015"></a>SNAT规则的ID。</p>
<p id="p3747356163011"><a name="p3747356163011"></a><a name="p3747356163011"></a>长度：<strong id="b074815611309"><a name="b074815611309"></a><a name="b074815611309"></a>36</strong></p>
</td>
</tr>
<tr id="row57201563301"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8754256193012"><a name="p8754256193012"></a><a name="p8754256193012"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p107591156193010"><a name="p107591156193010"></a><a name="p107591156193010"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p19763656193016"><a name="p19763656193016"></a><a name="p19763656193016"></a>项目的ID。</p>
</td>
</tr>
<tr id="row12720165643015"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p13766125612301"><a name="p13766125612301"></a><a name="p13766125612301"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1676915566301"><a name="p1676915566301"></a><a name="p1676915566301"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1477475619301"><a name="p1477475619301"></a><a name="p1477475619301"></a>公网NAT网关实例的ID。</p>
<p id="p9778165693015"><a name="p9778165693015"></a><a name="p9778165693015"></a>长度：<strong id="b11780256113018"><a name="b11780256113018"></a><a name="b11780256113018"></a>36</strong></p>
</td>
</tr>
<tr id="row372035633014"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p3785205610303"><a name="p3785205610303"></a><a name="p3785205610303"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p2078915613307"><a name="p2078915613307"></a><a name="p2078915613307"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p18793165618302"><a name="p18793165618302"></a><a name="p18793165618302"></a>cidr，可以是网段或者主机格式，与network_id参数二选一。source_type=0时，cidr必须是vpc 子网网段的子集（不能相等）; source_type=1时，cidr必须指定专线侧网段。</p>
<p id="p4796135633016"><a name="p4796135633016"></a><a name="p4796135633016"></a>最小长度：<strong id="b147988564306"><a name="b147988564306"></a><a name="b147988564306"></a>9</strong></p>
<p id="p08008563309"><a name="p08008563309"></a><a name="p08008563309"></a>最大长度：<strong id="b18011556203018"><a name="b18011556203018"></a><a name="b18011556203018"></a>39</strong></p>
</td>
</tr>
<tr id="row1172013569301"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p188040567302"><a name="p188040567302"></a><a name="p188040567302"></a>source_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1380875613303"><a name="p1380875613303"></a><a name="p1380875613303"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><a name="ul73841131152110"></a><a name="ul73841131152110"></a><ul id="ul73841131152110"><li>0：VPC侧，可以指定network_id 或者cidr</li><li>1：专线侧，只能指定cidr</li></ul>
<p id="p178161656153020"><a name="p178161656153020"></a><a name="p178161656153020"></a>缺省值：<strong id="b1781775663017"><a name="b1781775663017"></a><a name="b1781775663017"></a>0</strong></p>
</td>
</tr>
<tr id="row11720105653010"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p10820145613017"><a name="p10820145613017"></a><a name="p10820145613017"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p582665643010"><a name="p582665643010"></a><a name="p582665643010"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5830195614301"><a name="p5830195614301"></a><a name="p5830195614301"></a>功能说明：弹性公网IP的id，多个弹性公网IP的id使用逗号分隔。取值范围：最大长度4096字节。</p>
</td>
</tr>
<tr id="row1272020563303"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1834656143017"><a name="p1834656143017"></a><a name="p1834656143017"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1183815617302"><a name="p1183815617302"></a><a name="p1183815617302"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p28421756123018"><a name="p28421756123018"></a><a name="p28421756123018"></a>SNAT规则的描述，长度限制为255。</p>
<p id="p58461656203010"><a name="p58461656203010"></a><a name="p58461656203010"></a>最大长度：<strong id="b8847756143016"><a name="b8847756143016"></a><a name="b8847756143016"></a>255</strong></p>
</td>
</tr>
<tr id="row972015613302"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p5850556183013"><a name="p5850556183013"></a><a name="p5850556183013"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1685419565302"><a name="p1685419565302"></a><a name="p1685419565302"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p185816568307"><a name="p185816568307"></a><a name="p185816568307"></a>功能说明：SNAT规则的状态。</p>
<p id="p5862175614305"><a name="p5862175614305"></a><a name="p5862175614305"></a>枚举值：</p>
<a name="ul68678562306"></a><a name="ul68678562306"></a><ul id="ul68678562306"><li><strong id="b108701566302"><a name="b108701566302"></a><a name="b108701566302"></a>ACTIVE</strong></li><li><strong id="b487311567306"><a name="b487311567306"></a><a name="b487311567306"></a>PENDING_CREATE</strong></li><li><strong id="b16876115613308"><a name="b16876115613308"></a><a name="b16876115613308"></a>PENDING_UPDATE</strong></li><li><strong id="b1788012561303"><a name="b1788012561303"></a><a name="b1788012561303"></a>PENDING_DELETE</strong></li><li><strong id="b188849565300"><a name="b188849565300"></a><a name="b188849565300"></a>EIP_FREEZED</strong></li><li><strong id="b28881856113015"><a name="b28881856113015"></a><a name="b28881856113015"></a>INACTIVE</strong></li></ul>
</td>
</tr>
<tr id="row87201056143015"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p68901956153013"><a name="p68901956153013"></a><a name="p68901956153013"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p8894185615308"><a name="p8894185615308"></a><a name="p8894185615308"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p689955616306"><a name="p689955616306"></a><a name="p689955616306"></a>SNAT规则的创建时间，遵循UTC时间，格式是yyyy-mm-ddThh:mm:ssZ。最小长度：<strong id="b590414566304"><a name="b590414566304"></a><a name="b590414566304"></a>1</strong></p>
<p id="p3905256153016"><a name="p3905256153016"></a><a name="p3905256153016"></a>最大长度：<strong id="b1190616568303"><a name="b1190616568303"></a><a name="b1190616568303"></a>36</strong></p>
</td>
</tr>
<tr id="row15720856193016"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p2090945616301"><a name="p2090945616301"></a><a name="p2090945616301"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19114566309"><a name="p19114566309"></a><a name="p19114566309"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p7916256203014"><a name="p7916256203014"></a><a name="p7916256203014"></a>规则使用的网络id。与cidr参数二选一。</p>
<p id="p1391925623015"><a name="p1391925623015"></a><a name="p1391925623015"></a>长度：<strong id="b1892075614306"><a name="b1892075614306"></a><a name="b1892075614306"></a>36</strong></p>
</td>
</tr>
<tr id="row67211456173014"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p192614562306"><a name="p192614562306"></a><a name="p192614562306"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1593017563307"><a name="p1593017563307"></a><a name="p1593017563307"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p8934756153018"><a name="p8934756153018"></a><a name="p8934756153018"></a>解冻/冻结状态。取值范围：</p>
<a name="ul0937356103015"></a><a name="ul0937356103015"></a><ul id="ul0937356103015"><li>"true"：解冻</li><li>"false"：冻结</li></ul>
</td>
</tr>
<tr id="row1772119561307"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p794735614308"><a name="p794735614308"></a><a name="p794735614308"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p59501569304"><a name="p59501569304"></a><a name="p59501569304"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p139559565304"><a name="p139559565304"></a><a name="p139559565304"></a>功能说明：弹性公网IP，多个弹性公网IP使用逗号分隔。取值范围：最大长度1024字节。</p>
</td>
</tr>
<tr id="row8721145615301"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1958205633010"><a name="p1958205633010"></a><a name="p1958205633010"></a>freezed_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19962856133011"><a name="p19962856133011"></a><a name="p19962856133011"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1296615653018"><a name="p1296615653018"></a><a name="p1296615653018"></a>功能说明：冻结的弹性公网IP，多个冻结的弹性公网IP使用逗号分隔。取值范围：最大长度1024字节。</p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section797016568306"></a>

更新SNAT规则。

```
PUT https://{Endpoint}/v2/27e25061336f4af590faeabeb7fcd9a3/snat_rules/5b95c675-69c2-4656-ba06-58ff72e1d338 

{
  "snat_rule" : {
    "nat_gateway_id" : "bbe7c2e7-3bad-445b-a067-b30acce66053",
    "description" : "my_snat_rule_update",
    "public_ip_address" : "10.15.10.11,10.15.10.12"
  }
}
```

## 响应示例<a name="section49357193018"></a>

**状态码： 200**

PUT操作正常返回。

```
{
  "snat_rule" : {
    "floating_ip_id" : " bdc10a4c-d81a-41ec-adf7-de857f7c812a,7a094014-9657-463f-972b-e84d56b931a0",
    "status" : "PENDING_CREATE",
    "nat_gateway_id" : "bbe7c2e7-3bad-445b-a067-b30acce66053",
    "admin_state_up" : true,
    "network_id" : "eaad9cd6-2372-4be1-9535-9bd37210ae7b",
    "source_type" : 0,
    "tenant_id" : "27e25061336f4af590faeabeb7fcd9a3",
    "created_at" : "2017-11-18 07:54:21.665430",
    "id" : "5b95c675-69c2-4656-ba06-58ff72e1d338",
    "public_ip_address" : "10.15.10.11,10.15.10.12",
    "description" : "my_snat_rule_update"
  }
}
```

## 状态码<a name="section26785718308"></a>

<a name="zh-cn_topic_0297140340_status_code"></a>
<table><thead align="left"><tr id="row371195716307"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p574155743010"><a name="p574155743010"></a><a name="p574155743010"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p137713573306"><a name="p137713573306"></a><a name="p137713573306"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row97110578305"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p128015723012"><a name="p128015723012"></a><a name="p128015723012"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p783957193011"><a name="p783957193011"></a><a name="p783957193011"></a>PUT操作正常返回。</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section16862571300"></a>

请参见[错误码](错误码.md)。

