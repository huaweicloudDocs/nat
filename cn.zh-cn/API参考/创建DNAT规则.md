# 创建DNAT规则<a name="CreateNatGatewayDnatRule"></a>

## 功能介绍<a name="section2859182218267"></a>

创建DNAT规则。

## 接口约束<a name="section19862162217268"></a>

-   创建规则时，要求网关状态status = ACTIVE，要求网关管理员状态admin\_state\_up = True。
-   port\_id和private\_ip不能同时生效。
-   对于all port类型的规则，要求internal\_service\_port = 0，external\_service\_port = 0，protocol = ANY。

## 调试<a name="section4865172242612"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=nat&api=CreateNatGatewayDnatRule)中调试该接口。

## URI<a name="section38691222202618"></a>

POST /v2/\{project\_id\}/dnat\_rules

**表 1**  路径参数

<a name="table387382272619"></a>
<table><thead align="left"><tr id="row287252212261"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p18746225263"><a name="p18746225263"></a><a name="p18746225263"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p8875112292615"><a name="p8875112292615"></a><a name="p8875112292615"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1087632215261"><a name="p1087632215261"></a><a name="p1087632215261"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p9878422172616"><a name="p9878422172616"></a><a name="p9878422172616"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row2872182212619"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1887912228265"><a name="p1887912228265"></a><a name="p1887912228265"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p188012229269"><a name="p188012229269"></a><a name="p188012229269"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p178821822172619"><a name="p178821822172619"></a><a name="p178821822172619"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p11883182215261"><a name="p11883182215261"></a><a name="p11883182215261"></a>项目的ID。</p>
<p id="p178843225265"><a name="p178843225265"></a><a name="p178843225265"></a>最小长度：<strong id="b188510223267"><a name="b188510223267"></a><a name="b188510223267"></a>1</strong></p>
<p id="p08850229267"><a name="p08850229267"></a><a name="p08850229267"></a>最大长度：<strong id="b108861122182613"><a name="b108861122182613"></a><a name="b108861122182613"></a>36</strong></p>
<p id="p2562026131319"><a name="p2562026131319"></a><a name="p2562026131319"></a>获取方法详见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section10887122222616"></a>

**表 2**  请求Header参数

<a name="zh-cn_topic_0297140302_HeaderParameter"></a>
<table><thead align="left"><tr id="row19889162211268"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p18918225263"><a name="p18918225263"></a><a name="p18918225263"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p7893522172612"><a name="p7893522172612"></a><a name="p7893522172612"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p138941722102618"><a name="p138941722102618"></a><a name="p138941722102618"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p208961722142610"><a name="p208961722142610"></a><a name="p208961722142610"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row888915221260"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p2089892219269"><a name="p2089892219269"></a><a name="p2089892219269"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p98990227265"><a name="p98990227265"></a><a name="p98990227265"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p7900122218269"><a name="p7900122218269"></a><a name="p7900122218269"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p59018222267"><a name="p59018222267"></a><a name="p59018222267"></a>用户Token。用户Token也就是调用获取用户Token获取请求认证接口的响应值，该接口是唯一不需要认证的接口。请求响应成功后在响应消息头中包含的“X-Subject-Token”的值即为Token值。</p>
<p id="p139031722102616"><a name="p139031722102616"></a><a name="p139031722102616"></a>最小长度：<strong id="b1490417225263"><a name="b1490417225263"></a><a name="b1490417225263"></a>1</strong></p>
<p id="p10904122122618"><a name="p10904122122618"></a><a name="p10904122122618"></a>最大长度：<strong id="b18905142219263"><a name="b18905142219263"></a><a name="b18905142219263"></a>10240</strong></p>
</td>
</tr>
</tbody>
</table>

**表 3**  请求Body参数

<a name="zh-cn_topic_0297140302_requestParameter"></a>
<table><thead align="left"><tr id="row199077221263"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1790922219267"><a name="p1790922219267"></a><a name="p1790922219267"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p189111822152612"><a name="p189111822152612"></a><a name="p189111822152612"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1491252282614"><a name="p1491252282614"></a><a name="p1491252282614"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p18913922102612"><a name="p18913922102612"></a><a name="p18913922102612"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row090732216269"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p7915122211261"><a name="p7915122211261"></a><a name="p7915122211261"></a>dnat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1991719226263"><a name="p1991719226263"></a><a name="p1991719226263"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p691892217261"><a name="p691892217261"></a><a name="p691892217261"></a><a href="#zh-cn_topic_0297140302_request_CreateNatGatewayDnatOption">CreateNatGatewayDnatOption</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p792082212269"><a name="p792082212269"></a><a name="p792082212269"></a>创建DNAT规则的请求体。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  CreateNatGatewayDnatOption

<a name="zh-cn_topic_0297140302_request_CreateNatGatewayDnatOption"></a>
<table><thead align="left"><tr id="row39231922112614"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p7927122222612"><a name="p7927122222612"></a><a name="p7927122222612"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p9929102282612"><a name="p9929102282612"></a><a name="p9929102282612"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p12931322192620"><a name="p12931322192620"></a><a name="p12931322192620"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p169328225268"><a name="p169328225268"></a><a name="p169328225268"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1392372217268"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p179346225268"><a name="p179346225268"></a><a name="p179346225268"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p19351222268"><a name="p19351222268"></a><a name="p19351222268"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p49362224267"><a name="p49362224267"></a><a name="p49362224267"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p15938142212260"><a name="p15938142212260"></a><a name="p15938142212260"></a>DNAT规则的描述，长度限制为255。</p>
<p id="p1393912224266"><a name="p1393912224266"></a><a name="p1393912224266"></a>最大长度：<strong id="b2094015226264"><a name="b2094015226264"></a><a name="b2094015226264"></a>255</strong></p>
</td>
</tr>
<tr id="row1392362219263"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p794172219269"><a name="p794172219269"></a><a name="p794172219269"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p494242242612"><a name="p494242242612"></a><a name="p494242242612"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1094412215262"><a name="p1094412215262"></a><a name="p1094412215262"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1794510228266"><a name="p1794510228266"></a><a name="p1794510228266"></a>虚拟机或者裸机的Port ID，与private_ip参数二选一。</p>
<p id="p1194720221262"><a name="p1194720221262"></a><a name="p1194720221262"></a>长度：<strong id="b3947122242620"><a name="b3947122242620"></a><a name="b3947122242620"></a>36</strong></p>
</td>
</tr>
<tr id="row119242223268"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p4950182220262"><a name="p4950182220262"></a><a name="p4950182220262"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1295152262610"><a name="p1295152262610"></a><a name="p1295152262610"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p99531322162612"><a name="p99531322162612"></a><a name="p99531322162612"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p10955022122611"><a name="p10955022122611"></a><a name="p10955022122611"></a>用户私有IP地址，例如专线连接的私有云地址，与port_id参数二选一。</p>
</td>
</tr>
<tr id="row392402215262"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p10956722102615"><a name="p10956722102615"></a><a name="p10956722102615"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p169587228261"><a name="p169587228261"></a><a name="p169587228261"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1295918227262"><a name="p1295918227262"></a><a name="p1295918227262"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p13961172272611"><a name="p13961172272611"></a><a name="p13961172272611"></a>公网NAT网关实例的ID。</p>
<p id="p139621922182620"><a name="p139621922182620"></a><a name="p139621922182620"></a>长度：<strong id="b10962162262610"><a name="b10962162262610"></a><a name="b10962162262610"></a>36</strong></p>
</td>
</tr>
<tr id="row1192482218262"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p19965022152611"><a name="p19965022152611"></a><a name="p19965022152611"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p3967132292611"><a name="p3967132292611"></a><a name="p3967132292611"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1396816228265"><a name="p1396816228265"></a><a name="p1396816228265"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p4970172214266"><a name="p4970172214266"></a><a name="p4970172214266"></a>虚拟机或者裸机对外提供服务的协议端口号。取值范围：0~65535。</p>
<p id="p1697216224265"><a name="p1697216224265"></a><a name="p1697216224265"></a>最小值：<strong id="b1897322212266"><a name="b1897322212266"></a><a name="b1897322212266"></a>0</strong></p>
<p id="p29731222122615"><a name="p29731222122615"></a><a name="p29731222122615"></a>最大值：<strong id="b1097416223263"><a name="b1097416223263"></a><a name="b1097416223263"></a>65535</strong></p>
</td>
</tr>
<tr id="row16924112212611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p15975182210266"><a name="p15975182210266"></a><a name="p15975182210266"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p597618227268"><a name="p597618227268"></a><a name="p597618227268"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p14978162242617"><a name="p14978162242617"></a><a name="p14978162242617"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p39794225265"><a name="p39794225265"></a><a name="p39794225265"></a>弹性公网IP的id。</p>
</td>
</tr>
<tr id="row492412211268"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p16980122202619"><a name="p16980122202619"></a><a name="p16980122202619"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p3982132219269"><a name="p3982132219269"></a><a name="p3982132219269"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p199832223269"><a name="p199832223269"></a><a name="p199832223269"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1298410228268"><a name="p1298410228268"></a><a name="p1298410228268"></a>Floatingip对外提供服务的端口号。取值范围：0~65535。</p>
<p id="p798652211269"><a name="p798652211269"></a><a name="p798652211269"></a>最小值：<strong id="b199871022112614"><a name="b199871022112614"></a><a name="b199871022112614"></a>0</strong></p>
<p id="p1398862212263"><a name="p1398862212263"></a><a name="p1398862212263"></a>最大值：<strong id="b10989122192619"><a name="b10989122192619"></a><a name="b10989122192619"></a>65535</strong></p>
</td>
</tr>
<tr id="row2924142292611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p799012213265"><a name="p799012213265"></a><a name="p799012213265"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1999232272616"><a name="p1999232272616"></a><a name="p1999232272616"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p199931022152611"><a name="p199931022152611"></a><a name="p199931022152611"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p5995112262611"><a name="p5995112262611"></a><a name="p5995112262611"></a>协议类型，目前支持TCP/tcp、UDP/udp、ANY/any。对应协议号6、17、0。</p>
</td>
</tr>
<tr id="row1192410224265"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p16997162242615"><a name="p16997162242615"></a><a name="p16997162242615"></a>internal_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p099812213269"><a name="p099812213269"></a><a name="p099812213269"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p001523112610"><a name="p001523112610"></a><a name="p001523112610"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p2122315269"><a name="p2122315269"></a><a name="p2122315269"></a>虚拟机或者裸机对外提供服务的协议端口号范围。功能说明：该端口范围与external _service_port_range按顺序实现1:1映射。取值范围：1~65535。约束：只能以’-’字符连接端口范围。</p>
</td>
</tr>
<tr id="row292502202610"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p931423162615"><a name="p931423162615"></a><a name="p931423162615"></a>external_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p2552318263"><a name="p2552318263"></a><a name="p2552318263"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p26142352617"><a name="p26142352617"></a><a name="p26142352617"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p3842318265"><a name="p3842318265"></a><a name="p3842318265"></a>Floatingip对外提供服务的端口号范围。功能说明：该端口范围与internal _service_port_range按顺序实现1:1映射。取值范围：1~65535。约束：只能以’-’字符连接端口范围。</p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section79223142619"></a>

**状态码： 201**

**表 5**  响应Body参数

<a name="zh-cn_topic_0297140302_responseParameter"></a>
<table><thead align="left"><tr id="row14125231269"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p0147233263"><a name="p0147233263"></a><a name="p0147233263"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p11612342619"><a name="p11612342619"></a><a name="p11612342619"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p4171723142617"><a name="p4171723142617"></a><a name="p4171723142617"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row141232311264"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4191623102610"><a name="p4191623102610"></a><a name="p4191623102610"></a>dnat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p521192372620"><a name="p521192372620"></a><a name="p521192372620"></a><a href="#zh-cn_topic_0297140302_response_NatGatewayDnatRuleResponseBody">NatGatewayDnatRuleResponseBody</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p122272311268"><a name="p122272311268"></a><a name="p122272311268"></a>DNAT规则的响应体。</p>
</td>
</tr>
</tbody>
</table>

**表 6**  NatGatewayDnatRuleResponseBody

<a name="zh-cn_topic_0297140302_response_NatGatewayDnatRuleResponseBody"></a>
<table><thead align="left"><tr id="row325152314265"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p82872382618"><a name="p82872382618"></a><a name="p82872382618"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p9299237264"><a name="p9299237264"></a><a name="p9299237264"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1231823102613"><a name="p1231823102613"></a><a name="p1231823102613"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row125223132612"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p23215234264"><a name="p23215234264"></a><a name="p23215234264"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p73315233263"><a name="p73315233263"></a><a name="p73315233263"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p93510232268"><a name="p93510232268"></a><a name="p93510232268"></a>DNAT规则的ID。</p>
<p id="p936323172614"><a name="p936323172614"></a><a name="p936323172614"></a>长度：<strong id="b153692342612"><a name="b153692342612"></a><a name="b153692342612"></a>36</strong></p>
</td>
</tr>
<tr id="row20256238261"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p133914236264"><a name="p133914236264"></a><a name="p133914236264"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p174042314269"><a name="p174042314269"></a><a name="p174042314269"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1141142316260"><a name="p1141142316260"></a><a name="p1141142316260"></a>项目的ID。</p>
</td>
</tr>
<tr id="row122532310265"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p142102310265"><a name="p142102310265"></a><a name="p142102310265"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p174418231260"><a name="p174418231260"></a><a name="p174418231260"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1646112352614"><a name="p1646112352614"></a><a name="p1646112352614"></a>DNAT规则的描述。长度限制为255。</p>
<p id="p104762342612"><a name="p104762342612"></a><a name="p104762342612"></a>最大长度：<strong id="b1548423112612"><a name="b1548423112612"></a><a name="b1548423112612"></a>255</strong></p>
</td>
</tr>
<tr id="row325323122615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p164816237262"><a name="p164816237262"></a><a name="p164816237262"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p4508238261"><a name="p4508238261"></a><a name="p4508238261"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p752723102611"><a name="p752723102611"></a><a name="p752723102611"></a>虚拟机或者裸机的Port ID，与private_ip参数二选一。</p>
<p id="p1154162316263"><a name="p1154162316263"></a><a name="p1154162316263"></a>长度：<strong id="b95412372610"><a name="b95412372610"></a><a name="b95412372610"></a>36</strong></p>
</td>
</tr>
<tr id="row52512332615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p3572235266"><a name="p3572235266"></a><a name="p3572235266"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p145816237265"><a name="p145816237265"></a><a name="p145816237265"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p760152312262"><a name="p760152312262"></a><a name="p760152312262"></a>用户私有IP地址，例如专线连接的私有云地址，与port_id参数二选一。</p>
</td>
</tr>
<tr id="row1425182362615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1261122311267"><a name="p1261122311267"></a><a name="p1261122311267"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p106292352612"><a name="p106292352612"></a><a name="p106292352612"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1764152316264"><a name="p1764152316264"></a><a name="p1764152316264"></a>虚拟机或者裸机对外提供服务的协议端口号。取值范围：0~65535。</p>
<p id="p96614230268"><a name="p96614230268"></a><a name="p96614230268"></a>最小值：<strong id="b176610234266"><a name="b176610234266"></a><a name="b176610234266"></a>0</strong></p>
<p id="p206732319268"><a name="p206732319268"></a><a name="p206732319268"></a>最大值：<strong id="b196752372619"><a name="b196752372619"></a><a name="b196752372619"></a>65535</strong></p>
<p id="p12681723102611"><a name="p12681723102611"></a><a name="p12681723102611"></a>最小长度：<strong id="b36982317268"><a name="b36982317268"></a><a name="b36982317268"></a>1</strong></p>
<p id="p570102320268"><a name="p570102320268"></a><a name="p570102320268"></a>最大长度：<strong id="b1070142310268"><a name="b1070142310268"></a><a name="b1070142310268"></a>5</strong></p>
</td>
</tr>
<tr id="row525023202612"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p157162332610"><a name="p157162332610"></a><a name="p157162332610"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p57317231264"><a name="p57317231264"></a><a name="p57317231264"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p77517235264"><a name="p77517235264"></a><a name="p77517235264"></a>公网NAT网关实例的ID。</p>
<p id="p176523122616"><a name="p176523122616"></a><a name="p176523122616"></a>最小长度：<strong id="b2766232261"><a name="b2766232261"></a><a name="b2766232261"></a>1</strong></p>
<p id="p13778233261"><a name="p13778233261"></a><a name="p13778233261"></a>最大长度：<strong id="b77815233264"><a name="b77815233264"></a><a name="b77815233264"></a>36</strong></p>
</td>
</tr>
<tr id="row1125923122616"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1279102311267"><a name="p1279102311267"></a><a name="p1279102311267"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19827238269"><a name="p19827238269"></a><a name="p19827238269"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p198412312264"><a name="p198412312264"></a><a name="p198412312264"></a>弹性公网IP的id。</p>
<p id="p7851423152619"><a name="p7851423152619"></a><a name="p7851423152619"></a>最小长度：<strong id="b158532382613"><a name="b158532382613"></a><a name="b158532382613"></a>1</strong></p>
<p id="p1861123182611"><a name="p1861123182611"></a><a name="p1861123182611"></a>最大长度：<strong id="b158792313264"><a name="b158792313264"></a><a name="b158792313264"></a>36</strong></p>
</td>
</tr>
<tr id="row22517237261"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p118810238267"><a name="p118810238267"></a><a name="p118810238267"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19092314267"><a name="p19092314267"></a><a name="p19092314267"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1991142311262"><a name="p1991142311262"></a><a name="p1991142311262"></a>弹性公网IP的IP地址。</p>
</td>
</tr>
<tr id="row2025182322615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8931723142617"><a name="p8931723142617"></a><a name="p8931723142617"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p094023192613"><a name="p094023192613"></a><a name="p094023192613"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p29617236261"><a name="p29617236261"></a><a name="p29617236261"></a>Floatingip对外提供服务的端口号。取值范围：0~65535。</p>
</td>
</tr>
<tr id="row625102319268"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1797323132614"><a name="p1797323132614"></a><a name="p1797323132614"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19993230262"><a name="p19993230262"></a><a name="p19993230262"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12101192302611"><a name="p12101192302611"></a><a name="p12101192302611"></a>功能说明：DNAT规则的状态。</p>
<p id="p12102152342610"><a name="p12102152342610"></a><a name="p12102152342610"></a>枚举值：</p>
<a name="ul61041123172612"></a><a name="ul61041123172612"></a><ul id="ul61041123172612"><li><strong id="b17105423102615"><a name="b17105423102615"></a><a name="b17105423102615"></a>ACTIVE</strong></li><li><strong id="b20107122312619"><a name="b20107122312619"></a><a name="b20107122312619"></a>PENDING_CREATE</strong></li><li><strong id="b20108172316266"><a name="b20108172316266"></a><a name="b20108172316266"></a>PENDING_UPDATE</strong></li><li><strong id="b16109142311267"><a name="b16109142311267"></a><a name="b16109142311267"></a>PENDING_DELETE</strong></li><li><strong id="b5110102302610"><a name="b5110102302610"></a><a name="b5110102302610"></a>EIP_FREEZED</strong></li><li><strong id="b181121238262"><a name="b181121238262"></a><a name="b181121238262"></a>INACTIVE</strong></li></ul>
</td>
</tr>
<tr id="row20252023132612"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p191137239268"><a name="p191137239268"></a><a name="p191137239268"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p201145236262"><a name="p201145236262"></a><a name="p201145236262"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1759663022519"><a name="p1759663022519"></a><a name="p1759663022519"></a>解冻/冻结状态。取值范围：</p>
<a name="ul195721758266"></a><a name="ul195721758266"></a><ul id="ul195721758266"><li>"true"： 解冻</li><li>"false"： 冻结</li></ul>
</td>
</tr>
<tr id="row4251823192610"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19117623162616"><a name="p19117623162616"></a><a name="p19117623162616"></a>internal_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p91188235268"><a name="p91188235268"></a><a name="p91188235268"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1911932372610"><a name="p1911932372610"></a><a name="p1911932372610"></a>虚拟机或者裸机对外提供服务的协议端口号范围。功能说明：该端口范围与external _service_port_range按顺序实现1:1映射。取值范围：1~65535。约束：只能以’-’字符连接端口范围。</p>
</td>
</tr>
<tr id="row14252237265"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p912142319264"><a name="p912142319264"></a><a name="p912142319264"></a>external_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p912218234261"><a name="p912218234261"></a><a name="p912218234261"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p131231723102612"><a name="p131231723102612"></a><a name="p131231723102612"></a>Floatingip对外提供服务的端口号范围。功能说明：该端口范围与internal _service_port_range按顺序实现1:1映射。取值范围：1~65535。约束：只能以’-’字符连接端口范围</p>
</td>
</tr>
<tr id="row1925152322613"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p7124192315268"><a name="p7124192315268"></a><a name="p7124192315268"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p141266238262"><a name="p141266238262"></a><a name="p141266238262"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2127162317269"><a name="p2127162317269"></a><a name="p2127162317269"></a>协议类型，目前支持TCP/tcp、UDP/udp、ANY/any。对应协议号6、17、0。</p>
<p id="p1912832312265"><a name="p1912832312265"></a><a name="p1912832312265"></a>最小长度：<strong id="b912992312612"><a name="b912992312612"></a><a name="b912992312612"></a>1</strong></p>
<p id="p713072312614"><a name="p713072312614"></a><a name="p713072312614"></a>最大长度：<strong id="b1913052312619"><a name="b1913052312619"></a><a name="b1913052312619"></a>3</strong></p>
<p id="p181311323202614"><a name="p181311323202614"></a><a name="p181311323202614"></a>枚举值：</p>
<a name="ul16132023182614"></a><a name="ul16132023182614"></a><ul id="ul16132023182614"><li><strong id="b201331123152617"><a name="b201331123152617"></a><a name="b201331123152617"></a>tcp</strong></li><li><strong id="b1213418235266"><a name="b1213418235266"></a><a name="b1213418235266"></a>udp</strong></li><li><strong id="b51362023182617"><a name="b51362023182617"></a><a name="b51362023182617"></a>any</strong></li></ul>
</td>
</tr>
<tr id="row13269237262"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p0137123112614"><a name="p0137123112614"></a><a name="p0137123112614"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p161381923182615"><a name="p161381923182615"></a><a name="p161381923182615"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1014012311261"><a name="p1014012311261"></a><a name="p1014012311261"></a>DNAT规则的创建时间，遵循UTC时间，格式是yyyy-mm-ddThh:mm:ssZ。</p>
<p id="p614118239268"><a name="p614118239268"></a><a name="p614118239268"></a>最小长度：<strong id="b10142112319269"><a name="b10142112319269"></a><a name="b10142112319269"></a>1</strong></p>
<p id="p214282382610"><a name="p214282382610"></a><a name="p214282382610"></a>最大长度：<strong id="b5143112310268"><a name="b5143112310268"></a><a name="b5143112310268"></a>36</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section8144223192615"></a>

创建dnat规则。

```
POST https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/dnat_rules

{
  "dnat_rule" : {
    "nat_gateway_id" : "cda3a125-2406-456c-a11f-598e10578541",
    "floating_ip_id" : "bf99c679-9f41-4dac-8513-9c9228e713e1",
    "port_id" : "9a469561-daac-4c94-88f5-39366e5ea193",
    "internal_service_port" : 993,
    "protocol" : "tcp",
    "external_service_port" : 242,
    "description" : "my dnat rule 01"
  }
}
```

## 响应示例<a name="section13263202342610"></a>

**状态码： 201**

创建DNAT规则成功。

```
{
  "dnat_rule" : {
    "floating_ip_id" : "bf99c679-9f41-4dac-8513-9c9228e713e1",
    "status" : "ACTIVE",
    "nat_gateway_id" : "cda3a125-2406-456c-a11f-598e10578541",
    "admin_state_up" : true,
    "port_id" : "9a469561-daac-4c94-88f5-39366e5ea193",
    "internal_service_port" : 993,
    "protocol" : "tcp",
    "tenant_id" : "d199ba7e0ba64899b2e81518104b1526d",
    "created_at" : "2019-11-15 15:44:42.595173",
    "id" : "79195d50-0271-41f1-bded-4c089b2502ff",
    "external_service_port" : 242,
    "floating_ip_address" : "5.21.11.226",
    "description" : "my dnat rule 01"
  }
}
```

## 状态码<a name="section162741223122613"></a>

<a name="zh-cn_topic_0297140302_status_code"></a>
<table><thead align="left"><tr id="row1317502311268"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p12275142312269"><a name="p12275142312269"></a><a name="p12275142312269"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p8275162318269"><a name="p8275162318269"></a><a name="p8275162318269"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1175923112614"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p14276823132614"><a name="p14276823132614"></a><a name="p14276823132614"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1627662315263"><a name="p1627662315263"></a><a name="p1627662315263"></a>创建DNAT规则成功。</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section1127716232260"></a>

请参见[错误码](错误码.md)。

