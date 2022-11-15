# 创建公网NAT网关<a name="CreateNatGateway"></a>

## 功能介绍<a name="section16153920194617"></a>

创建公网NAT网关实例。

## 调试<a name="section415452074618"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=nat&api=CreateNatGateway)中调试该接口。

## URI<a name="section1415419207461"></a>

POST /v2/\{project\_id\}/nat\_gateways

**表 1**  路径参数

<a name="table3157162019463"></a>
<table><thead align="left"><tr id="row1615632094618"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p11157112016464"><a name="p11157112016464"></a><a name="p11157112016464"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p515820206460"><a name="p515820206460"></a><a name="p515820206460"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p131581420194610"><a name="p131581420194610"></a><a name="p131581420194610"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p5159820114616"><a name="p5159820114616"></a><a name="p5159820114616"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row615613204468"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p6159120134618"><a name="p6159120134618"></a><a name="p6159120134618"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p191602205467"><a name="p191602205467"></a><a name="p191602205467"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p01601720124615"><a name="p01601720124615"></a><a name="p01601720124615"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p516119209469"><a name="p516119209469"></a><a name="p516119209469"></a>项目的ID。</p>
<p id="p2161162019466"><a name="p2161162019466"></a><a name="p2161162019466"></a>最小长度：<strong id="b191625202469"><a name="b191625202469"></a><a name="b191625202469"></a>1</strong></p>
<p id="p3162142017462"><a name="p3162142017462"></a><a name="p3162142017462"></a>最大长度：<strong id="b171621220174615"><a name="b171621220174615"></a><a name="b171621220174615"></a>36</strong></p>
<p id="p2562026131319"><a name="p2562026131319"></a><a name="p2562026131319"></a>获取方法详见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section81622202460"></a>

**表 2**  请求Header参数

<a name="zh-cn_topic_0297140327_HeaderParameter"></a>
<table><thead align="left"><tr id="row9163192074618"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p16165152024616"><a name="p16165152024616"></a><a name="p16165152024616"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p1016552064611"><a name="p1016552064611"></a><a name="p1016552064611"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1616632010467"><a name="p1616632010467"></a><a name="p1616632010467"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p10167420134612"><a name="p10167420134612"></a><a name="p10167420134612"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1716422011462"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p16167132012465"><a name="p16167132012465"></a><a name="p16167132012465"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p7168620104611"><a name="p7168620104611"></a><a name="p7168620104611"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p16169132016465"><a name="p16169132016465"></a><a name="p16169132016465"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p817142054610"><a name="p817142054610"></a><a name="p817142054610"></a>用户Token。用户Token也就是调用获取用户Token获取请求认证接口的响应值，该接口是唯一不需要认证的接口。请求响应成功后在响应消息头中包含的“X-Subject-Token”的值即为Token值。</p>
<p id="p0171620134616"><a name="p0171620134616"></a><a name="p0171620134616"></a>最小长度：<strong id="b1517118206465"><a name="b1517118206465"></a><a name="b1517118206465"></a>1</strong></p>
<p id="p31728209462"><a name="p31728209462"></a><a name="p31728209462"></a>最大长度：<strong id="b1517252024617"><a name="b1517252024617"></a><a name="b1517252024617"></a>10240</strong></p>
</td>
</tr>
</tbody>
</table>

**表 3**  请求Body参数

<a name="zh-cn_topic_0297140327_requestParameter"></a>
<table><thead align="left"><tr id="row1317319202464"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p17174132018468"><a name="p17174132018468"></a><a name="p17174132018468"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p1817502019462"><a name="p1817502019462"></a><a name="p1817502019462"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1517522018461"><a name="p1517522018461"></a><a name="p1517522018461"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p131764209468"><a name="p131764209468"></a><a name="p131764209468"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row417310205461"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1017642012461"><a name="p1017642012461"></a><a name="p1017642012461"></a>nat_gateway</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p11177142018469"><a name="p11177142018469"></a><a name="p11177142018469"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p171771220154616"><a name="p171771220154616"></a><a name="p171771220154616"></a><a href="#zh-cn_topic_0297140327_request_CreateNatGatewayOption">CreateNatGatewayOption</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p21788201468"><a name="p21788201468"></a><a name="p21788201468"></a>创建公网NAT网关实例的请求体。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  CreateNatGatewayOption

<a name="zh-cn_topic_0297140327_request_CreateNatGatewayOption"></a>
<table><thead align="left"><tr id="row71811620144613"><th class="cellrowborder" valign="top" width="25.19%" id="mcps1.2.5.1.1"><p id="p1218332064615"><a name="p1218332064615"></a><a name="p1218332064615"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="14.81%" id="mcps1.2.5.1.2"><p id="p31831420114619"><a name="p31831420114619"></a><a name="p31831420114619"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p19183220154620"><a name="p19183220154620"></a><a name="p19183220154620"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p818411203463"><a name="p818411203463"></a><a name="p818411203463"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row0181142024614"><td class="cellrowborder" valign="top" width="25.19%" headers="mcps1.2.5.1.1 "><p id="p318472011464"><a name="p318472011464"></a><a name="p318472011464"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.5.1.2 "><p id="p91851120124615"><a name="p91851120124615"></a><a name="p91851120124615"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1718519201468"><a name="p1718519201468"></a><a name="p1718519201468"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p5185520194612"><a name="p5185520194612"></a><a name="p5185520194612"></a>公网NAT网关实例的名字，长度限制为64。公网NAT网关实例的名字仅支持数字、字母、_（下划线）、-（中划线）、中文。</p>
<p id="p18186192044610"><a name="p18186192044610"></a><a name="p18186192044610"></a>最大长度：<strong id="b2018613207463"><a name="b2018613207463"></a><a name="b2018613207463"></a>64</strong></p>
</td>
</tr>
<tr id="row12181192016469"><td class="cellrowborder" valign="top" width="25.19%" headers="mcps1.2.5.1.1 "><p id="p8186152094610"><a name="p8186152094610"></a><a name="p8186152094610"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.5.1.2 "><p id="p161861120104618"><a name="p161861120104618"></a><a name="p161861120104618"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p218712034612"><a name="p218712034612"></a><a name="p218712034612"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p9187192074613"><a name="p9187192074613"></a><a name="p9187192074613"></a>VPC的id。</p>
<p id="p337975464810"><a name="p337975464810"></a><a name="p337975464810"></a>获取请参见<a href="https://support.huaweicloud.com/api-vpc/vpc_api01_0003.html" target="_blank" rel="noopener noreferrer">查询VPC列表</a>。</p>
</td>
</tr>
<tr id="row518111206463"><td class="cellrowborder" valign="top" width="25.19%" headers="mcps1.2.5.1.1 "><p id="p21884205462"><a name="p21884205462"></a><a name="p21884205462"></a>internal_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.5.1.2 "><p id="p14188122074617"><a name="p14188122074617"></a><a name="p14188122074617"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1418912015468"><a name="p1418912015468"></a><a name="p1418912015468"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1189020174618"><a name="p1189020174618"></a><a name="p1189020174618"></a>公网NAT网关下行口（DVR的下一跳）所属的network id。</p>
<p id="p11314332568"><a name="p11314332568"></a><a name="p11314332568"></a>获取请参见<a href="https://support.huaweicloud.com/api-vpc/vpc_subnet01_0003.html" target="_blank" rel="noopener noreferrer">查询子网列表</a>。</p>
</td>
</tr>
<tr id="row31811820104611"><td class="cellrowborder" valign="top" width="25.19%" headers="mcps1.2.5.1.1 "><p id="p418962015463"><a name="p418962015463"></a><a name="p418962015463"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.5.1.2 "><p id="p17190132034620"><a name="p17190132034620"></a><a name="p17190132034620"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p91907208467"><a name="p91907208467"></a><a name="p91907208467"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1919062024616"><a name="p1919062024616"></a><a name="p1919062024616"></a>公网NAT网关实例的描述，长度限制为255。</p>
<p id="p18191132014469"><a name="p18191132014469"></a><a name="p18191132014469"></a>最大长度：<strong id="b719182084612"><a name="b719182084612"></a><a name="b719182084612"></a>255</strong></p>
</td>
</tr>
<tr id="row1918142024619"><td class="cellrowborder" valign="top" width="25.19%" headers="mcps1.2.5.1.1 "><p id="p119114208469"><a name="p119114208469"></a><a name="p119114208469"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.5.1.2 "><p id="p7192320134617"><a name="p7192320134617"></a><a name="p7192320134617"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p19192182044612"><a name="p19192182044612"></a><a name="p19192182044612"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1519312094612"><a name="p1519312094612"></a><a name="p1519312094612"></a>公网NAT网关的规格。取值为： “1”：小型，SNAT最大连接数10000；“2”：中型，SNAT最大连接数50000；“3”：大型，SNAT最大连接数200000；“4”：超大型，SNAT最大连接数1000000</p>
<p id="p131931620164615"><a name="p131931620164615"></a><a name="p131931620164615"></a>枚举值：</p>
<a name="ul31931120184610"></a><a name="ul31931120184610"></a><ul id="ul31931120184610"><li><strong id="b5193320144613"><a name="b5193320144613"></a><a name="b5193320144613"></a>1</strong></li><li><strong id="b1819422074614"><a name="b1819422074614"></a><a name="b1819422074614"></a>2</strong></li><li><strong id="b18194820104611"><a name="b18194820104611"></a><a name="b18194820104611"></a>3</strong></li><li><strong id="b51951520154612"><a name="b51951520154612"></a><a name="b51951520154612"></a>4</strong></li></ul>
</td>
</tr>
<tr id="row101827206461"><td class="cellrowborder" valign="top" width="25.19%" headers="mcps1.2.5.1.1 "><p id="p51951620144611"><a name="p51951620144611"></a><a name="p51951620144611"></a>enterprise_project_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.5.1.2 "><p id="p8195520124615"><a name="p8195520124615"></a><a name="p8195520124615"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p17199020104615"><a name="p17199020104615"></a><a name="p17199020104615"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1819992024610"><a name="p1819992024610"></a><a name="p1819992024610"></a>企业项目ID 创建公网NAT网关实例时，关联的企业项目ID。关于企业项目ID的获取及企业项目特性的详细信息，请参考《企业管理用户指南》。</p>
<p id="p182009204464"><a name="p182009204464"></a><a name="p182009204464"></a>缺省值：<strong id="b11200122084611"><a name="b11200122084611"></a><a name="b11200122084611"></a>0</strong></p>
<p id="p5200172074613"><a name="p5200172074613"></a><a name="p5200172074613"></a>最大长度：<strong id="b9200112064613"><a name="b9200112064613"></a><a name="b9200112064613"></a>36</strong></p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section132011420144613"></a>

**状态码： 201**

**表 5**  响应Body参数

<a name="zh-cn_topic_0297140327_responseParameter"></a>
<table><thead align="left"><tr id="row4202220124619"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p20203132013466"><a name="p20203132013466"></a><a name="p20203132013466"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1020412074618"><a name="p1020412074618"></a><a name="p1020412074618"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1620415202466"><a name="p1620415202466"></a><a name="p1620415202466"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row9202320154618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1320592019460"><a name="p1320592019460"></a><a name="p1320592019460"></a>nat_gateway</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p42061020124613"><a name="p42061020124613"></a><a name="p42061020124613"></a><a href="#zh-cn_topic_0297140327_response_NatGatewayResponseBody">NatGatewayResponseBody</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p72061720154613"><a name="p72061720154613"></a><a name="p72061720154613"></a>公网NAT网关实例的响应体。</p>
</td>
</tr>
</tbody>
</table>

**表 6**  NatGatewayResponseBody

<a name="zh-cn_topic_0297140327_response_NatGatewayResponseBody"></a>
<table><thead align="left"><tr id="row720812064618"><th class="cellrowborder" valign="top" width="25.290000000000003%" id="mcps1.2.4.1.1"><p id="p11210182014612"><a name="p11210182014612"></a><a name="p11210182014612"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="14.71%" id="mcps1.2.4.1.2"><p id="p152112205469"><a name="p152112205469"></a><a name="p152112205469"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1121122018461"><a name="p1121122018461"></a><a name="p1121122018461"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row15208182020463"><td class="cellrowborder" valign="top" width="25.290000000000003%" headers="mcps1.2.4.1.1 "><p id="p1621111201463"><a name="p1621111201463"></a><a name="p1621111201463"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="14.71%" headers="mcps1.2.4.1.2 "><p id="p102123205462"><a name="p102123205462"></a><a name="p102123205462"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p72127207465"><a name="p72127207465"></a><a name="p72127207465"></a>公网NAT网关实例的ID。</p>
<p id="p152122201462"><a name="p152122201462"></a><a name="p152122201462"></a>长度：<strong id="b321262017462"><a name="b321262017462"></a><a name="b321262017462"></a>36</strong></p>
</td>
</tr>
<tr id="row4208142094616"><td class="cellrowborder" valign="top" width="25.290000000000003%" headers="mcps1.2.4.1.1 "><p id="p112131208461"><a name="p112131208461"></a><a name="p112131208461"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.71%" headers="mcps1.2.4.1.2 "><p id="p221382094611"><a name="p221382094611"></a><a name="p221382094611"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p202145200461"><a name="p202145200461"></a><a name="p202145200461"></a>项目的ID。</p>
</td>
</tr>
<tr id="row12208142074617"><td class="cellrowborder" valign="top" width="25.290000000000003%" headers="mcps1.2.4.1.1 "><p id="p102144208463"><a name="p102144208463"></a><a name="p102144208463"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="14.71%" headers="mcps1.2.4.1.2 "><p id="p82142202460"><a name="p82142202460"></a><a name="p82142202460"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p82153207468"><a name="p82153207468"></a><a name="p82153207468"></a>公网NAT网关实例的名字，长度限制为64。</p>
<p id="p17215520204620"><a name="p17215520204620"></a><a name="p17215520204620"></a>最小长度：<strong id="b521582074610"><a name="b521582074610"></a><a name="b521582074610"></a>1</strong></p>
<p id="p721512202465"><a name="p721512202465"></a><a name="p721512202465"></a>最大长度：<strong id="b1721572019465"><a name="b1721572019465"></a><a name="b1721572019465"></a>64</strong></p>
</td>
</tr>
<tr id="row1420842012468"><td class="cellrowborder" valign="top" width="25.290000000000003%" headers="mcps1.2.4.1.1 "><p id="p1021612204461"><a name="p1021612204461"></a><a name="p1021612204461"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="14.71%" headers="mcps1.2.4.1.2 "><p id="p2216192064610"><a name="p2216192064610"></a><a name="p2216192064610"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p182165209465"><a name="p182165209465"></a><a name="p182165209465"></a>公网NAT网关实例的描述，长度限制为255。</p>
<p id="p1921720208463"><a name="p1921720208463"></a><a name="p1921720208463"></a>最大长度：<strong id="b9217112016468"><a name="b9217112016468"></a><a name="b9217112016468"></a>255</strong></p>
</td>
</tr>
<tr id="row152094209463"><td class="cellrowborder" valign="top" width="25.290000000000003%" headers="mcps1.2.4.1.1 "><p id="p121716203465"><a name="p121716203465"></a><a name="p121716203465"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="14.71%" headers="mcps1.2.4.1.2 "><p id="p1021732044613"><a name="p1021732044613"></a><a name="p1021732044613"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1021815204461"><a name="p1021815204461"></a><a name="p1021815204461"></a>公网NAT网关的规格。取值为： “1”：小型，SNAT最大连接数10000；“2”：中型，SNAT最大连接数50000；“3”：大型，SNAT最大连接数200000；“4”：超大型，SNAT最大连接数1000000</p>
<p id="p021892018469"><a name="p021892018469"></a><a name="p021892018469"></a>枚举值：</p>
<a name="ul1921815201467"></a><a name="ul1921815201467"></a><ul id="ul1921815201467"><li><strong id="b32195201466"><a name="b32195201466"></a><a name="b32195201466"></a>1</strong></li><li><strong id="b13219152084619"><a name="b13219152084619"></a><a name="b13219152084619"></a>2</strong></li><li><strong id="b722010208466"><a name="b722010208466"></a><a name="b722010208466"></a>3</strong></li><li><strong id="b1322013202466"><a name="b1322013202466"></a><a name="b1322013202466"></a>4</strong></li></ul>
</td>
</tr>
<tr id="row11209142010465"><td class="cellrowborder" valign="top" width="25.290000000000003%" headers="mcps1.2.4.1.1 "><p id="p3221220194612"><a name="p3221220194612"></a><a name="p3221220194612"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="14.71%" headers="mcps1.2.4.1.2 "><p id="p13221102024613"><a name="p13221102024613"></a><a name="p13221102024613"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p122221820114612"><a name="p122221820114612"></a><a name="p122221820114612"></a>公网NAT网关实例的状态。</p>
<p id="p19222820134620"><a name="p19222820134620"></a><a name="p19222820134620"></a>枚举值：</p>
<a name="ul12222102016468"></a><a name="ul12222102016468"></a><ul id="ul12222102016468"><li><strong id="b18222122024611"><a name="b18222122024611"></a><a name="b18222122024611"></a>ACTIVE</strong></li><li><strong id="b14223112016467"><a name="b14223112016467"></a><a name="b14223112016467"></a>PENDING_CREATE</strong></li><li><strong id="b4223162015468"><a name="b4223162015468"></a><a name="b4223162015468"></a>PENDING_UPDATE</strong></li><li><strong id="b9223132004616"><a name="b9223132004616"></a><a name="b9223132004616"></a>PENDING_DELETE</strong></li><li><strong id="b1322410204463"><a name="b1322410204463"></a><a name="b1322410204463"></a>INACTIVE</strong></li></ul>
</td>
</tr>
<tr id="row1920932015467"><td class="cellrowborder" valign="top" width="25.290000000000003%" headers="mcps1.2.4.1.1 "><p id="p192245202461"><a name="p192245202461"></a><a name="p192245202461"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="14.71%" headers="mcps1.2.4.1.2 "><p id="p1922417204467"><a name="p1922417204467"></a><a name="p1922417204467"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p822519201464"><a name="p822519201464"></a><a name="p822519201464"></a>解冻/冻结状态。取值范围：</p>
<a name="ul5225220144616"></a><a name="ul5225220144616"></a><ul id="ul5225220144616"><li>"true"：解冻</li><li>"false"：冻结</li></ul>
</td>
</tr>
<tr id="row320912024618"><td class="cellrowborder" valign="top" width="25.290000000000003%" headers="mcps1.2.4.1.1 "><p id="p1122742015465"><a name="p1122742015465"></a><a name="p1122742015465"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="14.71%" headers="mcps1.2.4.1.2 "><p id="p722717204469"><a name="p722717204469"></a><a name="p722717204469"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p922882054613"><a name="p922882054613"></a><a name="p922882054613"></a>公网NAT网关实例的创建时间，遵循UTC时间，格式是yyyy-mm-ddThh:mm:ssZ。</p>
</td>
</tr>
<tr id="row62091020184615"><td class="cellrowborder" valign="top" width="25.290000000000003%" headers="mcps1.2.4.1.1 "><p id="p1522862084618"><a name="p1522862084618"></a><a name="p1522862084618"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.71%" headers="mcps1.2.4.1.2 "><p id="p162291320154616"><a name="p162291320154616"></a><a name="p162291320154616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1822915209461"><a name="p1822915209461"></a><a name="p1822915209461"></a>VPC的id。</p>
</td>
</tr>
<tr id="row6209112017463"><td class="cellrowborder" valign="top" width="25.290000000000003%" headers="mcps1.2.4.1.1 "><p id="p122301720144616"><a name="p122301720144616"></a><a name="p122301720144616"></a>internal_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.71%" headers="mcps1.2.4.1.2 "><p id="p16230182016463"><a name="p16230182016463"></a><a name="p16230182016463"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p323142044611"><a name="p323142044611"></a><a name="p323142044611"></a>公网NAT网关下行口（DVR的下一跳）所属的network id。</p>
</td>
</tr>
<tr id="row620914209469"><td class="cellrowborder" valign="top" width="25.290000000000003%" headers="mcps1.2.4.1.1 "><p id="p122321620194613"><a name="p122321620194613"></a><a name="p122321620194613"></a>enterprise_project_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.71%" headers="mcps1.2.4.1.2 "><p id="p192331620104619"><a name="p192331620104619"></a><a name="p192331620104619"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p123414201463"><a name="p123414201463"></a><a name="p123414201463"></a>企业项目ID。创建公网NAT网关实例时，关联的企业项目ID。</p>
<p id="p023432017469"><a name="p023432017469"></a><a name="p023432017469"></a>最大长度：<strong id="b2234720104616"><a name="b2234720104616"></a><a name="b2234720104616"></a>36</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section7235172064618"></a>

创建公网NAT网关

```
POST https://{Endpoint}/v2/70505c941b9b4dfd82fd351932328a2f/nat_gateways 

{
  "nat_gateway" : {
    "name" : "nat_001",
    "description" : "my nat gateway 01",
    "router_id" : "d84f345c-80a1-4fa2-a39c-d0d397c3f09a",
    "internal_network_id" : "89d66639-aacb-4929-969d-07080b0f9fd9",
    "spec" : "1",
    "enterprise_project_id" : "0aad99bc-f5f6-4f78-8404-c598d76b0ed2"
  }
}
```

## 响应示例<a name="section122411320114617"></a>

**状态码： 201**

创建公网NAT网关实例成功。

```
{
  "nat_gateway" : {
    "id" : "14338426-6afe-4019-996b-3a9525296e11",
    "name" : "nat_001",
    "description" : "my nat gateway 01",
    "router_id" : "d84f345c-80a1-4fa2-a39c-d0d397c3f09a",
    "spec" : "1",
    "admin_state_up" : true,
    "tenant_id" : "70505c941b9b4dfd82fd351932328a2f",
    "internal_network_id" : "89d66639-aacb-4929-969d-07080b0f9fd9",
    "enterprise_project_id" : "0aad99bc-f5f6-4f78-8404-c598d76b0ed2",
    "status" : "ACTIVE",
    "created_at" : "2019-04-22T08:47:13"
  }
}
```

## 状态码<a name="section224762011468"></a>

<a name="zh-cn_topic_0297140327_status_code"></a>
<table><thead align="left"><tr id="row02481920184612"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p162492020134611"><a name="p162492020134611"></a><a name="p162492020134611"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p1024912019467"><a name="p1024912019467"></a><a name="p1024912019467"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row124811200469"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p425015203463"><a name="p425015203463"></a><a name="p425015203463"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p12250162014462"><a name="p12250162014462"></a><a name="p12250162014462"></a>创建公网NAT网关实例成功。</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section19251102014465"></a>

请参见[错误码](错误码.md)。

