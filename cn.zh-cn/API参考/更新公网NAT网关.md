# 更新公网NAT网关<a name="UpdateNatGateway"></a>

## 功能介绍<a name="section12700122017467"></a>

更新公网NAT网关实例。

## 接口约束<a name="section1570162015460"></a>

在admin\_state\_up = True & status = ACTIVE时允许更新，支持更新名称、描述、规格。

## 调试<a name="section18702820184615"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=nat&api=UpdateNatGateway)中调试该接口。

## URI<a name="section18703220184614"></a>

PUT /v2/\{project\_id\}/nat\_gateways/\{nat\_gateway\_id\}

**表 1**  路径参数

<a name="table1770514209468"></a>
<table><thead align="left"><tr id="row127043205461"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p17064200464"><a name="p17064200464"></a><a name="p17064200464"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p15706182015468"><a name="p15706182015468"></a><a name="p15706182015468"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p137071020114620"><a name="p137071020114620"></a><a name="p137071020114620"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p8708162074613"><a name="p8708162074613"></a><a name="p8708162074613"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1670472084613"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1070852024612"><a name="p1070852024612"></a><a name="p1070852024612"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p770911201466"><a name="p770911201466"></a><a name="p770911201466"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p770952054613"><a name="p770952054613"></a><a name="p770952054613"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p871014209466"><a name="p871014209466"></a><a name="p871014209466"></a>项目的ID。</p>
<p id="p16710152020463"><a name="p16710152020463"></a><a name="p16710152020463"></a>最小长度：<strong id="b971032019464"><a name="b971032019464"></a><a name="b971032019464"></a>1</strong></p>
<p id="p147117209465"><a name="p147117209465"></a><a name="p147117209465"></a>最大长度：<strong id="b77113204469"><a name="b77113204469"></a><a name="b77113204469"></a>36</strong></p>
<p id="p2562026131319"><a name="p2562026131319"></a><a name="p2562026131319"></a>获取方法详见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row3704152015461"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p3711120154613"><a name="p3711120154613"></a><a name="p3711120154613"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1471213207463"><a name="p1471213207463"></a><a name="p1471213207463"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p117124207463"><a name="p117124207463"></a><a name="p117124207463"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p16713132017469"><a name="p16713132017469"></a><a name="p16713132017469"></a>公网NAT网关实例的ID。</p>
<p id="p7713182064620"><a name="p7713182064620"></a><a name="p7713182064620"></a>长度：<strong id="b871311208467"><a name="b871311208467"></a><a name="b871311208467"></a>36</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section3714202015461"></a>

**表 2**  请求Header参数

<a name="zh-cn_topic_0297140334_HeaderParameter"></a>
<table><thead align="left"><tr id="row371414205461"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p67168205462"><a name="p67168205462"></a><a name="p67168205462"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p15716420104612"><a name="p15716420104612"></a><a name="p15716420104612"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p2722192024610"><a name="p2722192024610"></a><a name="p2722192024610"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p18723720154617"><a name="p18723720154617"></a><a name="p18723720154617"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row137155203465"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p2723172054611"><a name="p2723172054611"></a><a name="p2723172054611"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p16724152034610"><a name="p16724152034610"></a><a name="p16724152034610"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p17724132012466"><a name="p17724132012466"></a><a name="p17724132012466"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p97247205461"><a name="p97247205461"></a><a name="p97247205461"></a>用户Token。用户Token也就是调用获取用户Token获取请求认证接口的响应值，该接口是唯一不需要认证的接口。请求响应成功后在响应消息头中包含的“X-Subject-Token”的值即为Token值。</p>
<p id="p20725102010462"><a name="p20725102010462"></a><a name="p20725102010462"></a>最小长度：<strong id="b12725820194611"><a name="b12725820194611"></a><a name="b12725820194611"></a>1</strong></p>
<p id="p472515209466"><a name="p472515209466"></a><a name="p472515209466"></a>最大长度：<strong id="b872542019467"><a name="b872542019467"></a><a name="b872542019467"></a>10240</strong></p>
</td>
</tr>
</tbody>
</table>

**表 3**  请求Body参数

<a name="zh-cn_topic_0297140334_requestParameter"></a>
<table><thead align="left"><tr id="row17726192013460"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1572622014460"><a name="p1572622014460"></a><a name="p1572622014460"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p872722034614"><a name="p872722034614"></a><a name="p872722034614"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p107271020194613"><a name="p107271020194613"></a><a name="p107271020194613"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p197282206466"><a name="p197282206466"></a><a name="p197282206466"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row14726142010464"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p167281820114611"><a name="p167281820114611"></a><a name="p167281820114611"></a>nat_gateway</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p57281020114617"><a name="p57281020114617"></a><a name="p57281020114617"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p372972054615"><a name="p372972054615"></a><a name="p372972054615"></a><a href="#zh-cn_topic_0297140334_request_UpdateNatGatewayOption">UpdateNatGatewayOption</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1772911207462"><a name="p1772911207462"></a><a name="p1772911207462"></a>更新公网NAT网关实例的请求体。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  UpdateNatGatewayOption

<a name="zh-cn_topic_0297140334_request_UpdateNatGatewayOption"></a>
<table><thead align="left"><tr id="row5731820134617"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p173242014468"><a name="p173242014468"></a><a name="p173242014468"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p873312054611"><a name="p873312054611"></a><a name="p873312054611"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p173352016468"><a name="p173352016468"></a><a name="p173352016468"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p273513203466"><a name="p273513203466"></a><a name="p273513203466"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row177311020174615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1873682034617"><a name="p1873682034617"></a><a name="p1873682034617"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p7736182018461"><a name="p7736182018461"></a><a name="p7736182018461"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p11737122012468"><a name="p11737122012468"></a><a name="p11737122012468"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p973812204464"><a name="p973812204464"></a><a name="p973812204464"></a>公网NAT网关实例的名字，长度限制为64。公网NAT网关实例的名字仅支持数字、字母、_（下划线）、-（中划线）、中文。</p>
<p id="p473882013460"><a name="p473882013460"></a><a name="p473882013460"></a>最小长度：<strong id="b6738112014464"><a name="b6738112014464"></a><a name="b6738112014464"></a>1</strong></p>
<p id="p1738520124612"><a name="p1738520124612"></a><a name="p1738520124612"></a>最大长度：<strong id="b1673816202460"><a name="b1673816202460"></a><a name="b1673816202460"></a>64</strong></p>
</td>
</tr>
<tr id="row57311520114617"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p57397200463"><a name="p57397200463"></a><a name="p57397200463"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p77391020164616"><a name="p77391020164616"></a><a name="p77391020164616"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p4740920124613"><a name="p4740920124613"></a><a name="p4740920124613"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1774062064612"><a name="p1774062064612"></a><a name="p1774062064612"></a>公网NAT网关的描述，长度限制为255。</p>
<p id="p974113209463"><a name="p974113209463"></a><a name="p974113209463"></a>最大长度：<strong id="b117411720164616"><a name="b117411720164616"></a><a name="b117411720164616"></a>255</strong></p>
</td>
</tr>
<tr id="row177311120174617"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p2742122084618"><a name="p2742122084618"></a><a name="p2742122084618"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p5743102018466"><a name="p5743102018466"></a><a name="p5743102018466"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p07431220174616"><a name="p07431220174616"></a><a name="p07431220174616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p15744162017469"><a name="p15744162017469"></a><a name="p15744162017469"></a>公网NAT网关的规格。取值为："1"：小型，SNAT最大连接数10000；"2"：中型，SNAT最大连接数50000；"3"：大型，SNAT最大连接数200000；"4"：超大型，SNAT最大连接数1000000</p>
<p id="p2074482010465"><a name="p2074482010465"></a><a name="p2074482010465"></a>枚举值：</p>
<a name="ul3745320104613"></a><a name="ul3745320104613"></a><ul id="ul3745320104613"><li><strong id="b9747182020461"><a name="b9747182020461"></a><a name="b9747182020461"></a>1</strong></li><li><strong id="b675462010469"><a name="b675462010469"></a><a name="b675462010469"></a>2</strong></li><li><strong id="b1275518206466"><a name="b1275518206466"></a><a name="b1275518206466"></a>3</strong></li><li><strong id="b1975510202465"><a name="b1975510202465"></a><a name="b1975510202465"></a>4</strong></li></ul>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section975612074610"></a>

**状态码： 200**

**表 5**  响应Body参数

<a name="zh-cn_topic_0297140334_responseParameter"></a>
<table><thead align="left"><tr id="row5757162004610"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p275892094610"><a name="p275892094610"></a><a name="p275892094610"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p075916204468"><a name="p075916204468"></a><a name="p075916204468"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1175942018467"><a name="p1175942018467"></a><a name="p1175942018467"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row275716201460"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p9759520134618"><a name="p9759520134618"></a><a name="p9759520134618"></a>nat_gateway</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p117602020174618"><a name="p117602020174618"></a><a name="p117602020174618"></a><a href="#zh-cn_topic_0297140334_response_NatGatewayResponseBody">NatGatewayResponseBody</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p476042013464"><a name="p476042013464"></a><a name="p476042013464"></a>公网NAT网关实例的响应体。</p>
</td>
</tr>
</tbody>
</table>

**表 6**  NatGatewayResponseBody

<a name="zh-cn_topic_0297140334_response_NatGatewayResponseBody"></a>
<table><thead align="left"><tr id="row15761172084617"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1676452014461"><a name="p1676452014461"></a><a name="p1676452014461"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p67654207467"><a name="p67654207467"></a><a name="p67654207467"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1776562016462"><a name="p1776562016462"></a><a name="p1776562016462"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row476192011466"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19766320104619"><a name="p19766320104619"></a><a name="p19766320104619"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p4766152016462"><a name="p4766152016462"></a><a name="p4766152016462"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p10767420204614"><a name="p10767420204614"></a><a name="p10767420204614"></a>公网NAT网关实例的ID。</p>
<p id="p8767720124617"><a name="p8767720124617"></a><a name="p8767720124617"></a>长度：<strong id="b47671120134619"><a name="b47671120134619"></a><a name="b47671120134619"></a>36</strong></p>
</td>
</tr>
<tr id="row14762220124615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11769142064610"><a name="p11769142064610"></a><a name="p11769142064610"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12769112044612"><a name="p12769112044612"></a><a name="p12769112044612"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p14770122094619"><a name="p14770122094619"></a><a name="p14770122094619"></a>项目的ID。</p>
</td>
</tr>
<tr id="row476252014612"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15774172014617"><a name="p15774172014617"></a><a name="p15774172014617"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p57751220134615"><a name="p57751220134615"></a><a name="p57751220134615"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1777512013462"><a name="p1777512013462"></a><a name="p1777512013462"></a>公网NAT网关实例的名字，长度限制为64。</p>
<p id="p277612054610"><a name="p277612054610"></a><a name="p277612054610"></a>最小长度：<strong id="b12776720104617"><a name="b12776720104617"></a><a name="b12776720104617"></a>1</strong></p>
<p id="p477752074619"><a name="p477752074619"></a><a name="p477752074619"></a>最大长度：<strong id="b187771120204617"><a name="b187771120204617"></a><a name="b187771120204617"></a>64</strong></p>
</td>
</tr>
<tr id="row57626207468"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p2777142064613"><a name="p2777142064613"></a><a name="p2777142064613"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p877872044614"><a name="p877872044614"></a><a name="p877872044614"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p107781620184615"><a name="p107781620184615"></a><a name="p107781620184615"></a>公网NAT网关实例的描述，长度限制为255。</p>
<p id="p157781420104610"><a name="p157781420104610"></a><a name="p157781420104610"></a>最大长度：<strong id="b177822011468"><a name="b177822011468"></a><a name="b177822011468"></a>255</strong></p>
</td>
</tr>
<tr id="row8762720104619"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p177912014461"><a name="p177912014461"></a><a name="p177912014461"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p377916207462"><a name="p377916207462"></a><a name="p377916207462"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p10780162011468"><a name="p10780162011468"></a><a name="p10780162011468"></a>公网NAT网关的规格。取值为： “1”：小型，SNAT最大连接数10000；“2”：中型，SNAT最大连接数50000；“3”：大型，SNAT最大连接数200000；“4”：超大型，SNAT最大连接数1000000</p>
<p id="p978012010468"><a name="p978012010468"></a><a name="p978012010468"></a>枚举值：</p>
<a name="ul13780172054612"></a><a name="ul13780172054612"></a><ul id="ul13780172054612"><li><strong id="b5781520154615"><a name="b5781520154615"></a><a name="b5781520154615"></a>1</strong></li><li><strong id="b197811620104610"><a name="b197811620104610"></a><a name="b197811620104610"></a>2</strong></li><li><strong id="b378219203461"><a name="b378219203461"></a><a name="b378219203461"></a>3</strong></li><li><strong id="b13782142012468"><a name="b13782142012468"></a><a name="b13782142012468"></a>4</strong></li></ul>
</td>
</tr>
<tr id="row376216209461"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1778382011464"><a name="p1778382011464"></a><a name="p1778382011464"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p778320200465"><a name="p778320200465"></a><a name="p778320200465"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1178411209461"><a name="p1178411209461"></a><a name="p1178411209461"></a>公网NAT网关实例的状态。</p>
<p id="p9784192015462"><a name="p9784192015462"></a><a name="p9784192015462"></a>枚举值：</p>
<a name="ul478452074615"></a><a name="ul478452074615"></a><ul id="ul478452074615"><li><strong id="b1978513205463"><a name="b1978513205463"></a><a name="b1978513205463"></a>ACTIVE</strong></li><li><strong id="b278515209461"><a name="b278515209461"></a><a name="b278515209461"></a>PENDING_CREATE</strong></li><li><strong id="b0785182014612"><a name="b0785182014612"></a><a name="b0785182014612"></a>PENDING_UPDATE</strong></li><li><strong id="b13786162014466"><a name="b13786162014466"></a><a name="b13786162014466"></a>PENDING_DELETE</strong></li><li><strong id="b47861220104614"><a name="b47861220104614"></a><a name="b47861220104614"></a>INACTIVE</strong></li></ul>
</td>
</tr>
<tr id="row107621520114612"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19786142024620"><a name="p19786142024620"></a><a name="p19786142024620"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p17871020204613"><a name="p17871020204613"></a><a name="p17871020204613"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1278712084612"><a name="p1278712084612"></a><a name="p1278712084612"></a>解冻/冻结状态。取值范围：</p>
<a name="ul1878752044614"></a><a name="ul1878752044614"></a><ul id="ul1878752044614"><li>"true"：解冻</li><li>"false"：冻结</li></ul>
</td>
</tr>
<tr id="row77621720124613"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p17789122084617"><a name="p17789122084617"></a><a name="p17789122084617"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p15790192024616"><a name="p15790192024616"></a><a name="p15790192024616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p127901320164617"><a name="p127901320164617"></a><a name="p127901320164617"></a>公网NAT网关实例的创建时间，遵循UTC时间，格式是yyyy-mm-ddThh:mm:ssZ。</p>
</td>
</tr>
<tr id="row1776232094618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p379117207465"><a name="p379117207465"></a><a name="p379117207465"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p279182094616"><a name="p279182094616"></a><a name="p279182094616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p27921820144612"><a name="p27921820144612"></a><a name="p27921820144612"></a>VPC的id。</p>
</td>
</tr>
<tr id="row107621620164612"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19792172044617"><a name="p19792172044617"></a><a name="p19792172044617"></a>internal_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p579312205469"><a name="p579312205469"></a><a name="p579312205469"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p57931120154619"><a name="p57931120154619"></a><a name="p57931120154619"></a>公网NAT网关下行口（DVR的下一跳）所属的network id。</p>
</td>
</tr>
<tr id="row117621820114616"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p3794112014610"><a name="p3794112014610"></a><a name="p3794112014610"></a>enterprise_project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1379472074616"><a name="p1379472074616"></a><a name="p1379472074616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1479582016463"><a name="p1479582016463"></a><a name="p1479582016463"></a>企业项目ID。创建公网NAT网关实例时，关联的企业项目ID。</p>
<p id="p17795192014617"><a name="p17795192014617"></a><a name="p17795192014617"></a>最大长度：<strong id="b479572044612"><a name="b479572044612"></a><a name="b479572044612"></a>36</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section3796720174610"></a>

```
PUT https://{Endpoint}/v2/70505c941b9b4dfd82fd351932328a2f/nat_gateways/14338426-6afe-4019-996b-3a9525296e11 

{
  "nat_gateway" : {
    "name" : "new_name",
    "description" : "new description",
    "spec" : "1"
  }
}
```

## 响应示例<a name="section28011520104610"></a>

**状态码： 200**

更新公网NAT网关实例成功。

```
{
  "nat_gateway" : {
    "id" : "14338426-6afe-4019-996b-3a9525296e11",
    "name" : "new_name",
    "description" : "new description",
    "spec" : "1",
    "tenant_id" : "70505c941b9b4dfd82fd351932328a2f",
    "enterprise_project_id" : "2759da7b-8015-404c-ae0a-a389007b0e2a",
    "status" : "ACTIVE",
    "created_at" : "2019-04-22T08:47:13",
    "internal_network_id" : "89d66639-aacb-4929-969d-07080b0f9fd9",
    "router_id" : "d84f345c-80a1-4fa2-a39c-d0d397c3f09a",
    "admin_state_up" : true
  }
}
```

## 状态码<a name="section10806112017467"></a>

<a name="zh-cn_topic_0297140334_status_code"></a>
<table><thead align="left"><tr id="row68061320154620"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p1680732084619"><a name="p1680732084619"></a><a name="p1680732084619"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p1281122044619"><a name="p1281122044619"></a><a name="p1281122044619"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row380612200469"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p158121320164615"><a name="p158121320164615"></a><a name="p158121320164615"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p12812820204611"><a name="p12812820204611"></a><a name="p12812820204611"></a>更新公网NAT网关实例成功。</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section9812112017460"></a>

请参见[错误码](错误码.md)。

