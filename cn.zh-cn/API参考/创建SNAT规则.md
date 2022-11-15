# 创建SNAT规则<a name="CreateNatGatewaySnatRule"></a>

## 功能介绍<a name="section4840247192811"></a>

创建SNAT规则。

## 接口约束<a name="section384494762819"></a>

创建规则时，要求网关状态status = ACTIVE，要求网关管理员状态admin\_state\_up = True。获取网关状态和网关管理员状态请参见[查询指定的公网NAT网关详情](查询指定的公网NAT网关详情.md)。

## 调试<a name="section10848104717284"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=nat&api=CreateNatGatewaySnatRule)中调试该接口。

## URI<a name="section485584752817"></a>

POST /v2/\{project\_id\}/snat\_rules

**表 1**  路径参数

<a name="table19861134782820"></a>
<table><thead align="left"><tr id="row7860174772819"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p20863747132814"><a name="p20863747132814"></a><a name="p20863747132814"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p5865247142811"><a name="p5865247142811"></a><a name="p5865247142811"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p2086894715289"><a name="p2086894715289"></a><a name="p2086894715289"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p78701447132817"><a name="p78701447132817"></a><a name="p78701447132817"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row2086014762810"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1287217471281"><a name="p1287217471281"></a><a name="p1287217471281"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1587424711285"><a name="p1587424711285"></a><a name="p1587424711285"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p158761247172812"><a name="p158761247172812"></a><a name="p158761247172812"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p887820472285"><a name="p887820472285"></a><a name="p887820472285"></a>项目的ID。</p>
<p id="p888119475285"><a name="p888119475285"></a><a name="p888119475285"></a>最小长度：<strong id="b788210479285"><a name="b788210479285"></a><a name="b788210479285"></a>1</strong></p>
<p id="p5883847122817"><a name="p5883847122817"></a><a name="p5883847122817"></a>最大长度：<strong id="b488444711289"><a name="b488444711289"></a><a name="b488444711289"></a>36</strong></p>
<p id="p2562026131319"><a name="p2562026131319"></a><a name="p2562026131319"></a>获取方法详见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section8887184716283"></a>

**表 2**  请求Header参数

<a name="zh-cn_topic_0297140304_HeaderParameter"></a>
<table><thead align="left"><tr id="row989019471289"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p148944476287"><a name="p148944476287"></a><a name="p148944476287"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p689664712282"><a name="p689664712282"></a><a name="p689664712282"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p789854772817"><a name="p789854772817"></a><a name="p789854772817"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p2900547192817"><a name="p2900547192817"></a><a name="p2900547192817"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row389084772811"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p390354711282"><a name="p390354711282"></a><a name="p390354711282"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p4905174752810"><a name="p4905174752810"></a><a name="p4905174752810"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p890715478288"><a name="p890715478288"></a><a name="p890715478288"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p129101247162813"><a name="p129101247162813"></a><a name="p129101247162813"></a>用户Token。用户Token也就是调用获取用户Token获取请求认证接口的响应值，该接口是唯一不需要认证的接口。请求响应成功后在响应消息头中包含的“X-Subject-Token”的值即为Token值。</p>
<p id="p139111647192819"><a name="p139111647192819"></a><a name="p139111647192819"></a>最小长度：<strong id="b199124474289"><a name="b199124474289"></a><a name="b199124474289"></a>1</strong></p>
<p id="p169141475286"><a name="p169141475286"></a><a name="p169141475286"></a>最大长度：<strong id="b1091454742815"><a name="b1091454742815"></a><a name="b1091454742815"></a>10240</strong></p>
</td>
</tr>
</tbody>
</table>

**表 3**  请求Body参数

<a name="zh-cn_topic_0297140304_requestParameter"></a>
<table><thead align="left"><tr id="row591624711285"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p3919154714285"><a name="p3919154714285"></a><a name="p3919154714285"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p892174772814"><a name="p892174772814"></a><a name="p892174772814"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1992418472282"><a name="p1992418472282"></a><a name="p1992418472282"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p119261247202816"><a name="p119261247202816"></a><a name="p119261247202816"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row12916947162815"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p79281647132811"><a name="p79281647132811"></a><a name="p79281647132811"></a>snat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p18931114742810"><a name="p18931114742810"></a><a name="p18931114742810"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p9933647122815"><a name="p9933647122815"></a><a name="p9933647122815"></a><a href="#zh-cn_topic_0297140304_request_CreateNatGatewaySnatRuleOption">CreateNatGatewaySnatRuleOption</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p2936184711289"><a name="p2936184711289"></a><a name="p2936184711289"></a>创建SNAT规则的请求体。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  CreateNatGatewaySnatRuleOption

<a name="zh-cn_topic_0297140304_request_CreateNatGatewaySnatRuleOption"></a>
<table><thead align="left"><tr id="row7940164702811"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p7944104710288"><a name="p7944104710288"></a><a name="p7944104710288"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p994717475289"><a name="p994717475289"></a><a name="p994717475289"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p494984782818"><a name="p494984782818"></a><a name="p494984782818"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p99518474281"><a name="p99518474281"></a><a name="p99518474281"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row69401847192810"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p39539476280"><a name="p39539476280"></a><a name="p39539476280"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p12956174792814"><a name="p12956174792814"></a><a name="p12956174792814"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p199591747162817"><a name="p199591747162817"></a><a name="p199591747162817"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p596234717281"><a name="p596234717281"></a><a name="p596234717281"></a>公网NAT网关实例的ID。</p>
<p id="p2964747142813"><a name="p2964747142813"></a><a name="p2964747142813"></a>长度：<strong id="b1496504742815"><a name="b1496504742815"></a><a name="b1496504742815"></a>36</strong></p>
</td>
</tr>
<tr id="row14940144742819"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1596964713284"><a name="p1596964713284"></a><a name="p1596964713284"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p197217479288"><a name="p197217479288"></a><a name="p197217479288"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p6975194712288"><a name="p6975194712288"></a><a name="p6975194712288"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p397854718286"><a name="p397854718286"></a><a name="p397854718286"></a>cidr，可以是网段或者主机格式，与network_id参数二选一。source_type=0时，cidr必须是vpc 子网网段的子集（不能相等）; source_type=1时，cidr必须指定专线侧网段。</p>
</td>
</tr>
<tr id="row129401473287"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p198024712812"><a name="p198024712812"></a><a name="p198024712812"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p5983347112815"><a name="p5983347112815"></a><a name="p5983347112815"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1698516471287"><a name="p1698516471287"></a><a name="p1698516471287"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p13987134742815"><a name="p13987134742815"></a><a name="p13987134742815"></a>规则使用的网络id。与cidr参数二选一。</p>
<p id="p0990204710280"><a name="p0990204710280"></a><a name="p0990204710280"></a>长度：<strong id="b9991194742812"><a name="b9991194742812"></a><a name="b9991194742812"></a>36</strong></p>
</td>
</tr>
<tr id="row159404475283"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p15995124717282"><a name="p15995124717282"></a><a name="p15995124717282"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1899714762811"><a name="p1899714762811"></a><a name="p1899714762811"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p29994474281"><a name="p29994474281"></a><a name="p29994474281"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1717482284"><a name="p1717482284"></a><a name="p1717482284"></a>SNAT规则的描述，长度限制为255。</p>
<p id="p53194818289"><a name="p53194818289"></a><a name="p53194818289"></a>最大长度：<strong id="b25154815288"><a name="b25154815288"></a><a name="b25154815288"></a>255</strong></p>
</td>
</tr>
<tr id="row7940124752816"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p8664818281"><a name="p8664818281"></a><a name="p8664818281"></a>source_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p20810486288"><a name="p20810486288"></a><a name="p20810486288"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p910124818283"><a name="p910124818283"></a><a name="p910124818283"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p212248162814"><a name="p212248162814"></a><a name="p212248162814"></a>0：VPC侧，可以指定network_id 或者cidr 1：专线侧，只能指定cidr 不输入默认为0（VPC）</p>
<p id="p71474813289"><a name="p71474813289"></a><a name="p71474813289"></a>缺省值：<strong id="b191554832813"><a name="b191554832813"></a><a name="b191554832813"></a>0</strong></p>
</td>
</tr>
<tr id="row139411047132819"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p616164822813"><a name="p616164822813"></a><a name="p616164822813"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p419174852819"><a name="p419174852819"></a><a name="p419174852819"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p2021124814281"><a name="p2021124814281"></a><a name="p2021124814281"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p82414816286"><a name="p82414816286"></a><a name="p82414816286"></a>功能说明：弹性公网IP的id，多个弹性公网IP的id使用逗号分隔。取值范围：最大长度4096字节。约束：弹性公网IP的id个数不能超过20个。</p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section112694812288"></a>

**状态码： 201**

**表 5**  响应Body参数

<a name="zh-cn_topic_0297140304_responseParameter"></a>
<table><thead align="left"><tr id="row831448192819"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1335154820288"><a name="p1335154820288"></a><a name="p1335154820288"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p137144815286"><a name="p137144815286"></a><a name="p137144815286"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p4397486282"><a name="p4397486282"></a><a name="p4397486282"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row7311448142813"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p114194842816"><a name="p114194842816"></a><a name="p114194842816"></a>snat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1044194813286"><a name="p1044194813286"></a><a name="p1044194813286"></a><a href="#zh-cn_topic_0297140304_response_NatGatewaySnatRuleResponseBody">NatGatewaySnatRuleResponseBody</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p54614852815"><a name="p54614852815"></a><a name="p54614852815"></a>SNAT规则的响应体。</p>
</td>
</tr>
</tbody>
</table>

**表 6**  NatGatewaySnatRuleResponseBody

<a name="zh-cn_topic_0297140304_response_NatGatewaySnatRuleResponseBody"></a>
<table><thead align="left"><tr id="row3482488282"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p952548112812"><a name="p952548112812"></a><a name="p952548112812"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1554194818280"><a name="p1554194818280"></a><a name="p1554194818280"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p16571748162818"><a name="p16571748162818"></a><a name="p16571748162818"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row148144892819"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p35974816282"><a name="p35974816282"></a><a name="p35974816282"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p2626487287"><a name="p2626487287"></a><a name="p2626487287"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p186513487289"><a name="p186513487289"></a><a name="p186513487289"></a>SNAT规则的ID。</p>
<p id="p367134818287"><a name="p367134818287"></a><a name="p367134818287"></a>长度：<strong id="b106724822817"><a name="b106724822817"></a><a name="b106724822817"></a>36</strong></p>
</td>
</tr>
<tr id="row948348202813"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p17111485289"><a name="p17111485289"></a><a name="p17111485289"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12732048102815"><a name="p12732048102815"></a><a name="p12732048102815"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p19751348102815"><a name="p19751348102815"></a><a name="p19751348102815"></a>项目的ID。</p>
</td>
</tr>
<tr id="row1148184862810"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p37844812282"><a name="p37844812282"></a><a name="p37844812282"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p08019482287"><a name="p08019482287"></a><a name="p08019482287"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p158354812287"><a name="p158354812287"></a><a name="p158354812287"></a>公网NAT网关实例的ID。</p>
<p id="p68510486280"><a name="p68510486280"></a><a name="p68510486280"></a>长度：<strong id="b148764811283"><a name="b148764811283"></a><a name="b148764811283"></a>36</strong></p>
</td>
</tr>
<tr id="row164810489289"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p109174892812"><a name="p109174892812"></a><a name="p109174892812"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p094144816286"><a name="p094144816286"></a><a name="p094144816286"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p149617482285"><a name="p149617482285"></a><a name="p149617482285"></a>cidr，可以是网段或者主机格式，与network_id参数二选一。source_type=0时，cidr必须是vpc子网网段的子集（不能相等）; source_type=1时，cidr必须指定专线侧网段。</p>
<p id="p098174811285"><a name="p098174811285"></a><a name="p098174811285"></a>最小长度：<strong id="b1799114812817"><a name="b1799114812817"></a><a name="b1799114812817"></a>9</strong></p>
<p id="p2010084842812"><a name="p2010084842812"></a><a name="p2010084842812"></a>最大长度：<strong id="b510044810288"><a name="b510044810288"></a><a name="b510044810288"></a>39</strong></p>
</td>
</tr>
<tr id="row104811481288"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p131021748132819"><a name="p131021748132819"></a><a name="p131021748132819"></a>source_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p161041648102818"><a name="p161041648102818"></a><a name="p161041648102818"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><a name="ul919249101912"></a><a name="ul919249101912"></a><ul id="ul919249101912"><li>0：VPC侧，可以指定network_id 或者cidr</li><li>1：专线侧，只能指定cidr</li></ul>
<p id="p410813489284"><a name="p410813489284"></a><a name="p410813489284"></a>缺省值：<strong id="b310913487289"><a name="b310913487289"></a><a name="b310913487289"></a>0</strong></p>
</td>
</tr>
<tr id="row11481484282"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1011134862819"><a name="p1011134862819"></a><a name="p1011134862819"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1311334811283"><a name="p1311334811283"></a><a name="p1311334811283"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p7115124812815"><a name="p7115124812815"></a><a name="p7115124812815"></a>功能说明：弹性公网IP的id，多个弹性公网IP的id使用逗号分隔。取值范围：最大长度4096字节。</p>
</td>
</tr>
<tr id="row449124818281"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p20117848152811"><a name="p20117848152811"></a><a name="p20117848152811"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p9119164811288"><a name="p9119164811288"></a><a name="p9119164811288"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p71221748122813"><a name="p71221748122813"></a><a name="p71221748122813"></a>SNAT规则的描述，长度限制为255。</p>
<p id="p171248485284"><a name="p171248485284"></a><a name="p171248485284"></a>最大长度：<strong id="b1612464892818"><a name="b1612464892818"></a><a name="b1612464892818"></a>255</strong></p>
</td>
</tr>
<tr id="row74964812288"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p612684842812"><a name="p612684842812"></a><a name="p612684842812"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p111281548182817"><a name="p111281548182817"></a><a name="p111281548182817"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p513214832812"><a name="p513214832812"></a><a name="p513214832812"></a>功能说明：SNAT规则的状态。</p>
<p id="p16133174813286"><a name="p16133174813286"></a><a name="p16133174813286"></a>枚举值：</p>
<a name="ul31371948102813"></a><a name="ul31371948102813"></a><ul id="ul31371948102813"><li><strong id="b9142348102818"><a name="b9142348102818"></a><a name="b9142348102818"></a>ACTIVE</strong></li><li><strong id="b414494817281"><a name="b414494817281"></a><a name="b414494817281"></a>PENDING_CREATE</strong></li><li><strong id="b1214615483286"><a name="b1214615483286"></a><a name="b1214615483286"></a>PENDING_UPDATE</strong></li><li><strong id="b1714916482285"><a name="b1714916482285"></a><a name="b1714916482285"></a>PENDING_DELETE</strong></li><li><strong id="b915218487281"><a name="b915218487281"></a><a name="b915218487281"></a>EIP_FREEZED</strong></li><li><strong id="b51541048152814"><a name="b51541048152814"></a><a name="b51541048152814"></a>INACTIVE</strong></li></ul>
</td>
</tr>
<tr id="row1349048192819"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1815654842812"><a name="p1815654842812"></a><a name="p1815654842812"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p51596488283"><a name="p51596488283"></a><a name="p51596488283"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1016234815289"><a name="p1016234815289"></a><a name="p1016234815289"></a>SNAT规则的创建时间，遵循UTC时间，格式是yyyy-mm-ddThh:mm:ssZ。</p>
<p id="p9164144810284"><a name="p9164144810284"></a><a name="p9164144810284"></a>最小长度：<strong id="b1716534872812"><a name="b1716534872812"></a><a name="b1716534872812"></a>1</strong></p>
<p id="p2167124810284"><a name="p2167124810284"></a><a name="p2167124810284"></a>最大长度：<strong id="b181682048162819"><a name="b181682048162819"></a><a name="b181682048162819"></a>36</strong></p>
</td>
</tr>
<tr id="row149144832811"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19170174852816"><a name="p19170174852816"></a><a name="p19170174852816"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p3173174862813"><a name="p3173174862813"></a><a name="p3173174862813"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p31762487287"><a name="p31762487287"></a><a name="p31762487287"></a>规则使用的网络id。与cidr参数二选一。</p>
<p id="p117812487282"><a name="p117812487282"></a><a name="p117812487282"></a>长度：<strong id="b517994814283"><a name="b517994814283"></a><a name="b517994814283"></a>36</strong></p>
</td>
</tr>
<tr id="row1849144810286"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1183948132810"><a name="p1183948132810"></a><a name="p1183948132810"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p61850481282"><a name="p61850481282"></a><a name="p61850481282"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p618715487283"><a name="p618715487283"></a><a name="p618715487283"></a>解冻/冻结状态。取值范围：</p>
<a name="ul1618917481287"></a><a name="ul1618917481287"></a><ul id="ul1618917481287"><li>"true"：解冻</li><li>"false"：冻结</li></ul>
</td>
</tr>
<tr id="row19495487288"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1319794872819"><a name="p1319794872819"></a><a name="p1319794872819"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1619934852815"><a name="p1619934852815"></a><a name="p1619934852815"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p192011948122818"><a name="p192011948122818"></a><a name="p192011948122818"></a>功能说明：弹性公网IP，多个弹性公网IP使用逗号分隔。取值范围：最大长度1024字节。</p>
</td>
</tr>
<tr id="row16495486284"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p3204154818289"><a name="p3204154818289"></a><a name="p3204154818289"></a>freezed_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1420614822812"><a name="p1420614822812"></a><a name="p1420614822812"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p6209164815286"><a name="p6209164815286"></a><a name="p6209164815286"></a>功能说明：冻结的弹性公网IP，多个冻结的弹性公网IP使用逗号分隔。取值范围：最大长度1024字节。</p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section1921164822816"></a>

创建SNAT规则。

```
POST https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/snat_rules

{
  "snat_rule" : {
    "nat_gateway_id" : "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
    "cidr" : "172.30.0.0/24",
    "source_type" : 1,
    "floating_ip_id" : "bdc10a4c-d81a-41ec-adf7-de857f7c812a",
    "description" : "my snat rule 01"
  }
}
```

## 响应示例<a name="section824012482280"></a>

**状态码： 201**

创建SNAT规则成功。

```
{
  "snat_rule" : {
    "floating_ip_id" : "bdc10a4c-d81a-41ec-adf7-de857f7c812a",
    "status" : "PENDING_CREATE",
    "nat_gateway_id" : "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
    "admin_state_up" : true,
    "cidr" : "172.30.0.0/24",
    "description" : "",
    "source_type" : 1,
    "tenant_id" : "27e25061336f4af590faeabeb7fcd9a3",
    "created_at" : "2017-11-18 07:54:21.665430",
    "id" : "5b95c675-69c2-4656-ba06-58ff72e1d338",
    "floating_ip_address" : "5.21.11.226"
  }
}
```

## 状态码<a name="section32801482286"></a>

<a name="zh-cn_topic_0297140304_status_code"></a>
<table><thead align="left"><tr id="row92832048182818"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p1728574816283"><a name="p1728574816283"></a><a name="p1728574816283"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p228794815280"><a name="p228794815280"></a><a name="p228794815280"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row11283448102820"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1928904813285"><a name="p1928904813285"></a><a name="p1928904813285"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p72931348182817"><a name="p72931348182817"></a><a name="p72931348182817"></a>创建SNAT规则成功。</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section42951848202815"></a>

请参见[错误码](错误码.md)。

