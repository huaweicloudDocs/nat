# 批量创建DNAT规则<a name="BatchCreateNatGatewayDnatRules"></a>

## 功能介绍<a name="section2093918124274"></a>

批量创建DNAT规则。

## 接口约束<a name="section194920123277"></a>

-   批量创建规则时，要求网关状态status = ACTIVE，要求网关管理员状态admin\_state\_up = True。
-   port\_id和private\_ip不能同时生效。
-   对于all port类型的规则，要求internal\_service\_port = 0，external\_service\_port = 0，protocol = ANY。

## 调试<a name="section49591012122717"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=nat&api=BatchCreateNatGatewayDnatRules)中调试该接口。

## URI<a name="section79721912182717"></a>

POST /v2/\{project\_id\}/dnat\_rules/batch

**表 1**  路径参数

<a name="table1798519122278"></a>
<table><thead align="left"><tr id="row19982121218272"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p18990812172718"><a name="p18990812172718"></a><a name="p18990812172718"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p11994812172715"><a name="p11994812172715"></a><a name="p11994812172715"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1199971252711"><a name="p1199971252711"></a><a name="p1199971252711"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p9461342712"><a name="p9461342712"></a><a name="p9461342712"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row10982111213272"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1491513182717"><a name="p1491513182717"></a><a name="p1491513182717"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1413131316275"><a name="p1413131316275"></a><a name="p1413131316275"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p10188133273"><a name="p10188133273"></a><a name="p10188133273"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1223191352713"><a name="p1223191352713"></a><a name="p1223191352713"></a>项目的ID。</p>
<p id="p2562026131319"><a name="p2562026131319"></a><a name="p2562026131319"></a>获取方法详见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section228013102719"></a>

**表 2**  请求Header参数

<a name="zh-cn_topic_0297140303_HeaderParameter"></a>
<table><thead align="left"><tr id="row2347139279"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1740181332717"><a name="p1740181332717"></a><a name="p1740181332717"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p744121372714"><a name="p744121372714"></a><a name="p744121372714"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p174912135275"><a name="p174912135275"></a><a name="p174912135275"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p15554130279"><a name="p15554130279"></a><a name="p15554130279"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row163451313270"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p2591413112717"><a name="p2591413112717"></a><a name="p2591413112717"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1565613152712"><a name="p1565613152712"></a><a name="p1565613152712"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p069913142716"><a name="p069913142716"></a><a name="p069913142716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p137451311273"><a name="p137451311273"></a><a name="p137451311273"></a>用户Token。用户Token也就是调用获取用户Token获取请求认证接口的响应值，该接口是唯一不需要认证的接口。请求响应成功后在响应消息头中包含的“X-Subject-Token”的值即为Token值。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  请求Body参数

<a name="requestParameter"></a>
<table><thead align="left"><tr id="row6540182412916"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p10541192411914"><a name="p10541192411914"></a><a name="p10541192411914"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p75429249916"><a name="p75429249916"></a><a name="p75429249916"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1654211241194"><a name="p1654211241194"></a><a name="p1654211241194"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p854316241594"><a name="p854316241594"></a><a name="p854316241594"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row135401224695"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p2543124591"><a name="p2543124591"></a><a name="p2543124591"></a>dnat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p12544124999"><a name="p12544124999"></a><a name="p12544124999"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p175461624397"><a name="p175461624397"></a><a name="p175461624397"></a>Array of <a href="#request_CreateNatGatewayDnatOption">CreateNatGatewayDnatOption</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p854719248920"><a name="p854719248920"></a><a name="p854719248920"></a>DNAT规则批量创建对象的请求体。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  CreateNatGatewayDnatOption

<a name="request_CreateNatGatewayDnatOption"></a>
<table><thead align="left"><tr id="row25485241699"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p185502241099"><a name="p185502241099"></a><a name="p185502241099"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p185517241790"><a name="p185517241790"></a><a name="p185517241790"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p8551624192"><a name="p8551624192"></a><a name="p8551624192"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p1455216242098"><a name="p1455216242098"></a><a name="p1455216242098"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row454882411914"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p11553724198"><a name="p11553724198"></a><a name="p11553724198"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p145542024097"><a name="p145542024097"></a><a name="p145542024097"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p655442417915"><a name="p655442417915"></a><a name="p655442417915"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p145553248917"><a name="p145553248917"></a><a name="p145553248917"></a>DNAT规则的描述，长度限制为255。</p>
<p id="p16555224198"><a name="p16555224198"></a><a name="p16555224198"></a>最大长度：<strong id="b125555241594"><a name="b125555241594"></a><a name="b125555241594"></a>255</strong></p>
</td>
</tr>
<tr id="row15488248918"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p755617241595"><a name="p755617241595"></a><a name="p755617241595"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p135561924997"><a name="p135561924997"></a><a name="p135561924997"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1557122412912"><a name="p1557122412912"></a><a name="p1557122412912"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p15577241391"><a name="p15577241391"></a><a name="p15577241391"></a>虚拟机或者裸机的Port ID，对应虚拟私有云场景，与private_ip参数二选一。</p>
<p id="p1155892416911"><a name="p1155892416911"></a><a name="p1155892416911"></a>长度：<strong id="b1355862416913"><a name="b1355862416913"></a><a name="b1355862416913"></a>36</strong></p>
</td>
</tr>
<tr id="row1254842418910"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p15559192411914"><a name="p15559192411914"></a><a name="p15559192411914"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p14559142414912"><a name="p14559142414912"></a><a name="p14559142414912"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p15601224299"><a name="p15601224299"></a><a name="p15601224299"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1556111241491"><a name="p1556111241491"></a><a name="p1556111241491"></a>用户私有IP地址，对应专线、云连接场景，与port_id参数二选一。</p>
</td>
</tr>
<tr id="row354817241911"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1056311249911"><a name="p1056311249911"></a><a name="p1056311249911"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p18563182413913"><a name="p18563182413913"></a><a name="p18563182413913"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1456416241918"><a name="p1456416241918"></a><a name="p1456416241918"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p556513249915"><a name="p556513249915"></a><a name="p556513249915"></a>公网NAT网关实例的ID。</p>
<p id="p2565324492"><a name="p2565324492"></a><a name="p2565324492"></a>长度：<strong id="b155658241895"><a name="b155658241895"></a><a name="b155658241895"></a>36</strong></p>
</td>
</tr>
<tr id="row2054815241095"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p14566132415911"><a name="p14566132415911"></a><a name="p14566132415911"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p156752414916"><a name="p156752414916"></a><a name="p156752414916"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p12567152417917"><a name="p12567152417917"></a><a name="p12567152417917"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p2568724993"><a name="p2568724993"></a><a name="p2568724993"></a>虚拟机或者裸机对外提供服务的协议端口号。 取值范围：0~65535。</p>
<p id="p956822419917"><a name="p956822419917"></a><a name="p956822419917"></a>最小值：<strong id="b115681241194"><a name="b115681241194"></a><a name="b115681241194"></a>0</strong></p>
<p id="p55691424198"><a name="p55691424198"></a><a name="p55691424198"></a>最大值：<strong id="b195693248912"><a name="b195693248912"></a><a name="b195693248912"></a>65535</strong></p>
</td>
</tr>
<tr id="row85492249913"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p35693241190"><a name="p35693241190"></a><a name="p35693241190"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p115706247916"><a name="p115706247916"></a><a name="p115706247916"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p185701324596"><a name="p185701324596"></a><a name="p185701324596"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1457182413915"><a name="p1457182413915"></a><a name="p1457182413915"></a>弹性公网IP的id。</p>
</td>
</tr>
<tr id="row19549122413916"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p357110241299"><a name="p357110241299"></a><a name="p357110241299"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p55711524992"><a name="p55711524992"></a><a name="p55711524992"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p14572142416916"><a name="p14572142416916"></a><a name="p14572142416916"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p157282414910"><a name="p157282414910"></a><a name="p157282414910"></a>Floatingip对外提供服务的端口号。 取值范围：0~65535。</p>
<p id="p1957311242914"><a name="p1957311242914"></a><a name="p1957311242914"></a>最小值：<strong id="b6573724191"><a name="b6573724191"></a><a name="b6573724191"></a>0</strong></p>
<p id="p257382416913"><a name="p257382416913"></a><a name="p257382416913"></a>最大值：<strong id="b155732247919"><a name="b155732247919"></a><a name="b155732247919"></a>65535</strong></p>
</td>
</tr>
<tr id="row954942418919"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p105741724793"><a name="p105741724793"></a><a name="p105741724793"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1157482417918"><a name="p1157482417918"></a><a name="p1157482417918"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p357592419916"><a name="p357592419916"></a><a name="p357592419916"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p65758246918"><a name="p65758246918"></a><a name="p65758246918"></a>协议类型，目前支持TCP/tcp、UDP/udp、ANY/any。 对应协议号6、17、0。</p>
</td>
</tr>
<tr id="row185494247918"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1457692419916"><a name="p1457692419916"></a><a name="p1457692419916"></a>internal_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p2057710241892"><a name="p2057710241892"></a><a name="p2057710241892"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1157717245916"><a name="p1157717245916"></a><a name="p1157717245916"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1236631891712"><a name="p1236631891712"></a><a name="p1236631891712"></a>虚拟机或者裸机对外提供服务的协议端口号范围。</p>
<p id="p1060992514176"><a name="p1060992514176"></a><a name="p1060992514176"></a>功能说明：该端口范围与external _service_port_range按顺序实现1:1映射。</p>
<p id="p19382332201710"><a name="p19382332201710"></a><a name="p19382332201710"></a>取值范围：1~65535。</p>
<p id="p657811241796"><a name="p657811241796"></a><a name="p657811241796"></a>约束：只能以’-’字符连接端口范围。</p>
</td>
</tr>
<tr id="row11549142416914"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p557932413920"><a name="p557932413920"></a><a name="p557932413920"></a>external_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p195807240920"><a name="p195807240920"></a><a name="p195807240920"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1158052420911"><a name="p1158052420911"></a><a name="p1158052420911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p5476754101717"><a name="p5476754101717"></a><a name="p5476754101717"></a>Floatingip对外提供服务的端口号范围。</p>
<p id="p11162409187"><a name="p11162409187"></a><a name="p11162409187"></a>功能说明：该端口范围与internal _service_port_range按顺序实现1:1映射。</p>
<p id="p19253181310187"><a name="p19253181310187"></a><a name="p19253181310187"></a>取值范围：1~65535。</p>
<p id="p1458122418910"><a name="p1458122418910"></a><a name="p1458122418910"></a>约束：只能以’-’字符连接端口范围。</p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section1779513142715"></a>

**状态码： 201**

**表 5**  响应Body参数

<a name="zh-cn_topic_0297140303_responseParameter"></a>
<table><thead align="left"><tr id="row13882135272"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p7931013122717"><a name="p7931013122717"></a><a name="p7931013122717"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p097113152710"><a name="p097113152710"></a><a name="p097113152710"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1410161392718"><a name="p1410161392718"></a><a name="p1410161392718"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1588161314277"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p910510130270"><a name="p910510130270"></a><a name="p910510130270"></a>dnat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p2011101322716"><a name="p2011101322716"></a><a name="p2011101322716"></a>Array of <a href="#zh-cn_topic_0297140303_response_NatGatewayDnatRuleResponseBody">NatGatewayDnatRuleResponseBody</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p61181613122716"><a name="p61181613122716"></a><a name="p61181613122716"></a>DNAT规则批量创建对象的响应体。</p>
</td>
</tr>
</tbody>
</table>

**表 6**  NatGatewayDnatRuleResponseBody

<a name="zh-cn_topic_0297140303_response_NatGatewayDnatRuleResponseBody"></a>
<table><thead align="left"><tr id="row11122181312715"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1212851382716"><a name="p1212851382716"></a><a name="p1212851382716"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p713481320277"><a name="p713481320277"></a><a name="p713481320277"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p213811382719"><a name="p213811382719"></a><a name="p213811382719"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1512211311275"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1714211137274"><a name="p1714211137274"></a><a name="p1714211137274"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p714631312715"><a name="p714631312715"></a><a name="p714631312715"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p0152213142717"><a name="p0152213142717"></a><a name="p0152213142717"></a>DNAT规则的ID。</p>
<p id="p5156131302712"><a name="p5156131302712"></a><a name="p5156131302712"></a>长度：<strong id="b20157813172710"><a name="b20157813172710"></a><a name="b20157813172710"></a>36</strong></p>
</td>
</tr>
<tr id="row13122151372715"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p13164111392716"><a name="p13164111392716"></a><a name="p13164111392716"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p116891332718"><a name="p116891332718"></a><a name="p116891332718"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5174191316278"><a name="p5174191316278"></a><a name="p5174191316278"></a>项目的ID。</p>
</td>
</tr>
<tr id="row15122171317274"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p51793135279"><a name="p51793135279"></a><a name="p51793135279"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p718321316277"><a name="p718321316277"></a><a name="p718321316277"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p16188191317275"><a name="p16188191317275"></a><a name="p16188191317275"></a>DNAT规则的描述。长度限制为255。</p>
<p id="p15193141382717"><a name="p15193141382717"></a><a name="p15193141382717"></a>最大长度：<strong id="b1919581318274"><a name="b1919581318274"></a><a name="b1919581318274"></a>255</strong></p>
</td>
</tr>
<tr id="row12122313172713"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19198141392712"><a name="p19198141392712"></a><a name="p19198141392712"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p520218134275"><a name="p520218134275"></a><a name="p520218134275"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p820871342718"><a name="p820871342718"></a><a name="p820871342718"></a>虚拟机或者裸机的Port ID，对应虚拟私有云场景，与private_ip参数二选一。</p>
<p id="p11212513132718"><a name="p11212513132718"></a><a name="p11212513132718"></a>长度：<strong id="b3213171313276"><a name="b3213171313276"></a><a name="b3213171313276"></a>36</strong></p>
</td>
</tr>
<tr id="row6122151352719"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p13222161310272"><a name="p13222161310272"></a><a name="p13222161310272"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p7226513172717"><a name="p7226513172717"></a><a name="p7226513172717"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p02312131270"><a name="p02312131270"></a><a name="p02312131270"></a>用户私有IP地址，对应专线、云连接场景，与port_id参数二选一。</p>
</td>
</tr>
<tr id="row7122181352712"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p423681318278"><a name="p423681318278"></a><a name="p423681318278"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p02431613172719"><a name="p02431613172719"></a><a name="p02431613172719"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p132493133274"><a name="p132493133274"></a><a name="p132493133274"></a>虚拟机或者裸机对外提供服务的协议端口号。取值范围：0~65535。</p>
<p id="p725341382714"><a name="p725341382714"></a><a name="p725341382714"></a>最小值：<strong id="b5256151352716"><a name="b5256151352716"></a><a name="b5256151352716"></a>0</strong></p>
<p id="p6259161319273"><a name="p6259161319273"></a><a name="p6259161319273"></a>最大值：<strong id="b1526191316273"><a name="b1526191316273"></a><a name="b1526191316273"></a>65535</strong></p>
<p id="p8264151315274"><a name="p8264151315274"></a><a name="p8264151315274"></a>最小长度：<strong id="b152651713202710"><a name="b152651713202710"></a><a name="b152651713202710"></a>1</strong></p>
<p id="p122681613172717"><a name="p122681613172717"></a><a name="p122681613172717"></a>最大长度：<strong id="b102691313112718"><a name="b102691313112718"></a><a name="b102691313112718"></a>5</strong></p>
</td>
</tr>
<tr id="row1712231392716"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p127231372716"><a name="p127231372716"></a><a name="p127231372716"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p17278111311274"><a name="p17278111311274"></a><a name="p17278111311274"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17284171322711"><a name="p17284171322711"></a><a name="p17284171322711"></a>公网NAT网关实例的ID。</p>
<p id="p182891913142718"><a name="p182891913142718"></a><a name="p182891913142718"></a>最小长度：<strong id="b42911413122719"><a name="b42911413122719"></a><a name="b42911413122719"></a>1</strong></p>
<p id="p529521332720"><a name="p529521332720"></a><a name="p529521332720"></a>最大长度：<strong id="b429611136271"><a name="b429611136271"></a><a name="b429611136271"></a>36</strong></p>
</td>
</tr>
<tr id="row19122113112712"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p329920131276"><a name="p329920131276"></a><a name="p329920131276"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p3304131316271"><a name="p3304131316271"></a><a name="p3304131316271"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p8309101362717"><a name="p8309101362717"></a><a name="p8309101362717"></a>弹性公网IP的id。</p>
<p id="p731331342718"><a name="p731331342718"></a><a name="p731331342718"></a>最小长度：<strong id="b431561332716"><a name="b431561332716"></a><a name="b431561332716"></a>1</strong></p>
<p id="p1331819133272"><a name="p1331819133272"></a><a name="p1331819133272"></a>最大长度：<strong id="b1431911319274"><a name="b1431911319274"></a><a name="b1431911319274"></a>36</strong></p>
</td>
</tr>
<tr id="row1712361352720"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p2322191310272"><a name="p2322191310272"></a><a name="p2322191310272"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p432820137273"><a name="p432820137273"></a><a name="p432820137273"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1533441392715"><a name="p1533441392715"></a><a name="p1533441392715"></a>弹性公网IP的IP地址。</p>
</td>
</tr>
<tr id="row19123113202713"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1334021332715"><a name="p1334021332715"></a><a name="p1334021332715"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p334491372717"><a name="p334491372717"></a><a name="p334491372717"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p16349191322711"><a name="p16349191322711"></a><a name="p16349191322711"></a>Floatingip对外提供服务的端口号。取值范围：0~65535。</p>
</td>
</tr>
<tr id="row812381382714"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p035321312277"><a name="p035321312277"></a><a name="p035321312277"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p93571313122718"><a name="p93571313122718"></a><a name="p93571313122718"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1236661313275"><a name="p1236661313275"></a><a name="p1236661313275"></a>功能说明：DNAT规则的状态。</p>
<p id="p937061372718"><a name="p937061372718"></a><a name="p937061372718"></a>枚举值：</p>
<a name="ul12376213112713"></a><a name="ul12376213112713"></a><ul id="ul12376213112713"><li><strong id="b738181312717"><a name="b738181312717"></a><a name="b738181312717"></a>ACTIVE</strong></li><li><strong id="b1387213182720"><a name="b1387213182720"></a><a name="b1387213182720"></a>PENDING_CREATE</strong></li><li><strong id="b9392151382710"><a name="b9392151382710"></a><a name="b9392151382710"></a>PENDING_UPDATE</strong></li><li><strong id="b2398913112714"><a name="b2398913112714"></a><a name="b2398913112714"></a>PENDING_DELETE</strong></li><li><strong id="b14404201310276"><a name="b14404201310276"></a><a name="b14404201310276"></a>EIP_FREEZED</strong></li><li><strong id="b11410181313278"><a name="b11410181313278"></a><a name="b11410181313278"></a>INACTIVE</strong></li></ul>
</td>
</tr>
<tr id="row131231913162715"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p154149132275"><a name="p154149132275"></a><a name="p154149132275"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p14420111313276"><a name="p14420111313276"></a><a name="p14420111313276"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p104261213162711"><a name="p104261213162711"></a><a name="p104261213162711"></a>解冻/冻结状态。取值范围：</p>
<a name="ul195721758266"></a><a name="ul195721758266"></a><ul id="ul195721758266"><li>"true"： 解冻</li><li>"false"： 冻结</li></ul>
</td>
</tr>
<tr id="row412319136274"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4431131312271"><a name="p4431131312271"></a><a name="p4431131312271"></a>internal_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p6436191392714"><a name="p6436191392714"></a><a name="p6436191392714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p18441191382713"><a name="p18441191382713"></a><a name="p18441191382713"></a>虚拟机或者裸机对外提供服务的协议端口号范围。功能说明：该端口范围与external _service_port_range按顺序实现1:1映射。取值范围：1~65535。约束：只能以’-’字符连接端口范围。</p>
</td>
</tr>
<tr id="row1712371314271"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8446161318276"><a name="p8446161318276"></a><a name="p8446161318276"></a>external_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p245011310278"><a name="p245011310278"></a><a name="p245011310278"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1745471352719"><a name="p1745471352719"></a><a name="p1745471352719"></a>Floatingip对外提供服务的端口号范围。功能说明：该端口范围与internal _service_port_range按顺序实现1:1映射。取值范围：1~65535。约束：只能以’-’字符连接端口范围</p>
</td>
</tr>
<tr id="row14123111317272"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p5459121316277"><a name="p5459121316277"></a><a name="p5459121316277"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1546311315270"><a name="p1546311315270"></a><a name="p1546311315270"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12469141332713"><a name="p12469141332713"></a><a name="p12469141332713"></a>协议类型，目前支持TCP/tcp、UDP/udp、ANY/any。对应协议号6、17、0。</p>
<p id="p1847471392715"><a name="p1847471392715"></a><a name="p1847471392715"></a>最小长度：<strong id="b2047510139275"><a name="b2047510139275"></a><a name="b2047510139275"></a>1</strong></p>
<p id="p1947841352713"><a name="p1947841352713"></a><a name="p1947841352713"></a>最大长度：<strong id="b1948051315277"><a name="b1948051315277"></a><a name="b1948051315277"></a>3</strong></p>
<p id="p1148251372719"><a name="p1148251372719"></a><a name="p1148251372719"></a>枚举值：</p>
<a name="ul13486141310271"></a><a name="ul13486141310271"></a><ul id="ul13486141310271"><li><strong id="b449011313274"><a name="b449011313274"></a><a name="b449011313274"></a>tcp</strong></li><li><strong id="b54941413132719"><a name="b54941413132719"></a><a name="b54941413132719"></a>udp</strong></li><li><strong id="b1949811352713"><a name="b1949811352713"></a><a name="b1949811352713"></a>any</strong></li></ul>
</td>
</tr>
<tr id="row91231130279"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11501181311273"><a name="p11501181311273"></a><a name="p11501181311273"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p35051113122712"><a name="p35051113122712"></a><a name="p35051113122712"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p751021312715"><a name="p751021312715"></a><a name="p751021312715"></a>DNAT规则的创建时间，遵循UTC时间，格式是yyyy-mm-ddThh:mm:ssZ。</p>
<p id="p11514151310278"><a name="p11514151310278"></a><a name="p11514151310278"></a>最小长度：<strong id="b751731382716"><a name="b751731382716"></a><a name="b751731382716"></a>1</strong></p>
<p id="p352111132273"><a name="p352111132273"></a><a name="p352111132273"></a>最大长度：<strong id="b55227131279"><a name="b55227131279"></a><a name="b55227131279"></a>36</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section2052615138273"></a>

批量创建规则\(第一条为指定端口的规则，第二条为all port类型的规则\)。

```
POST https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/dnat_rules/batch

{
  "dnat_rules" : [ {
    "floating_ip_id" : "bf99c679-9f41-4dac-8513-9c9228e713e1",
    "nat_gateway_id" : "cda3a125-2406-456c-a11f-598e10578541",
    "port_id" : "9a469561-daac-4c94-88f5-39366e5ea193",
    "internal_service_port" : 993,
    "protocol" : "tcp",
    "external_service_port" : 242,
    "description" : "my dnat rule 01"
  }, {
    "floating_ip_id" : "cf99c679-9f41-4dac-8513-9c9228e713e1",
    "nat_gateway_id" : "dda3a125-2406-456c-a11f-598e10578541",
    "private_ip" : "192.168.1.100",
    "internal_service_port" : 0,
    "protocol" : "any",
    "external_service_port" : 0,
    "description" : "my dnat rule 01"
  } ]
}
```

## 响应示例<a name="section15630151372710"></a>

**状态码： 201**

POST操作正常返回。

```
{
  "dnat_rules" : [ {
    "floating_ip_id" : "bf99c679-9f41-4dac-8513-9c9228e713e1",
    "status" : "ACTIVE",
    "nat_gateway_id" : "cda3a125-2406-456c-a11f-598e10578541",
    "admin_state_up" : true,
    "port_id" : "9a469561-daac-4c94-88f5-39366e5ea193",
    "private_ip" : "",
    "internal_service_port" : 993,
    "protocol" : "tcp",
    "tenant_id" : "d199ba7e0ba64899b2e81518104b1526",
    "created_at" : "2019-11-15 15:44:42.595173",
    "id" : "79195d50-0271-41f1-bded-4c089b2502ff",
    "floating_ip_address" : "5.21.11.226",
    "external_service_port" : 242,
    "description" : "my dnat rule 01"
  }, {
    "floating_ip_id" : "cf99c679-9f41-4dac-8513-9c9228e713e1",
    "status" : "ACTIVE",
    "nat_gateway_id" : "dda3a125-2406-456c-a11f-598e10578541",
    "admin_state_up" : true,
    "port_id" : "",
    "private_ip" : "192.168.1.100",
    "internal_service_port" : 0,
    "protocol" : "any",
    "tenant_id" : "d199ba7e0ba64899b2e81518104b1526",
    "created_at" : "2019-11-15 15:44:42.595173",
    "id" : "79195d50-0271-41f1-bded-4c089c2502ff",
    "floating_ip_address" : "5.21.11.227",
    "external_service_port" : 0,
    "description" : "my dnat rule 01"
  } ]
}
```

## 状态码<a name="section14786121382713"></a>

<a name="zh-cn_topic_0297140303_status_code"></a>
<table><thead align="left"><tr id="row279151332719"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p17795201332716"><a name="p17795201332716"></a><a name="p17795201332716"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p1480061352710"><a name="p1480061352710"></a><a name="p1480061352710"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row179141310277"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p180501392717"><a name="p180501392717"></a><a name="p180501392717"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1981014137275"><a name="p1981014137275"></a><a name="p1981014137275"></a>POST操作正常返回。</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section20814111342711"></a>

请参见[错误码](错误码.md)。

