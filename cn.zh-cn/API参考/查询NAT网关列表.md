# 查询NAT网关列表<a name="nat_api_0002"></a>

## 功能介绍<a name="section21650537"></a>

查询NAT网关列表。如无特殊说明，匹配规则为精确匹配。

## URI<a name="section60637113"></a>

GET /v2.0/nat\_gateways

>![](public_sys-resources/icon-note.gif) **说明：**   
>可以在URI后面用‘?’和‘&’添加不同的查询条件组合。支持参数说明中所有非必选参数过滤，请参考请求样例。  

**表 1**  参数说明

<a name="table18558131224111"></a>
<table><thead align="left"><tr id="row1808612184118"><th class="cellrowborder" valign="top" width="21.35213521352135%" id="mcps1.2.5.1.1"><p id="p780881214411"><a name="p780881214411"></a><a name="p780881214411"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.08080808080808%" id="mcps1.2.5.1.2"><p id="p1558032915438"><a name="p1558032915438"></a><a name="p1558032915438"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.711671167116712%" id="mcps1.2.5.1.3"><p id="p380881220414"><a name="p380881220414"></a><a name="p380881220414"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="53.855385538553854%" id="mcps1.2.5.1.4"><p id="p1880841274119"><a name="p1880841274119"></a><a name="p1880841274119"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row28088123418"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="p480891218412"><a name="p480891218412"></a><a name="p480891218412"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="p2580182916436"><a name="p2580182916436"></a><a name="p2580182916436"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="p0808181217416"><a name="p0808181217416"></a><a name="p0808181217416"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><p id="p7808141219418"><a name="p7808141219418"></a><a name="p7808141219418"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="row121171254102416"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="p63722013254"><a name="p63722013254"></a><a name="p63722013254"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="p13764185294314"><a name="p13764185294314"></a><a name="p13764185294314"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="p1737212162518"><a name="p1737212162518"></a><a name="p1737212162518"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><p id="p237217110251"><a name="p237217110251"></a><a name="p237217110251"></a>每页返回的个数。</p>
</td>
</tr>
<tr id="row080891254119"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="p1880851212411"><a name="p1880851212411"></a><a name="p1880851212411"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="p18311175344318"><a name="p18311175344318"></a><a name="p18311175344318"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="p198084127419"><a name="p198084127419"></a><a name="p198084127419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><p id="p1080810121412"><a name="p1080810121412"></a><a name="p1080810121412"></a>项目的ID。</p>
</td>
</tr>
<tr id="row11808111284110"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="p1808191244110"><a name="p1808191244110"></a><a name="p1808191244110"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="p117981853124317"><a name="p117981853124317"></a><a name="p117981853124317"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="p2080861264119"><a name="p2080861264119"></a><a name="p2080861264119"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><p id="p2808112174112"><a name="p2808112174112"></a><a name="p2808112174112"></a>NAT网关的名字。</p>
<p id="p138082126416"><a name="p138082126416"></a><a name="p138082126416"></a>NAT网关的名字仅支持数字、字母、_（下划线）、-（中划线）、中文。</p>
</td>
</tr>
<tr id="row6808712144114"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="p08087126419"><a name="p08087126419"></a><a name="p08087126419"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="p170010548430"><a name="p170010548430"></a><a name="p170010548430"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="p180811212410"><a name="p180811212410"></a><a name="p180811212410"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><p id="p780817129410"><a name="p780817129410"></a><a name="p780817129410"></a>NAT网关的描述。</p>
</td>
</tr>
<tr id="row16808171215417"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="p118081612194112"><a name="p118081612194112"></a><a name="p118081612194112"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="p4212155518434"><a name="p4212155518434"></a><a name="p4212155518434"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="p2080820126416"><a name="p2080820126416"></a><a name="p2080820126416"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><p id="p198081612114114"><a name="p198081612114114"></a><a name="p198081612114114"></a>NAT网关的规格。</p>
<p id="p138081012184115"><a name="p138081012184115"></a><a name="p138081012184115"></a>取值为：</p>
<a name="ul108080122414"></a><a name="ul108080122414"></a><ul id="ul108080122414"><li>“1”：小型，SNAT最大连接数10000</li><li>“2”：中型，SNAT最大连接数50000</li><li>“3”：大型，SNAT最大连接数200000</li><li>“4”：超大型，SNAT最大连接数1000000</li></ul>
</td>
</tr>
<tr id="row178085121417"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="p7808181224114"><a name="p7808181224114"></a><a name="p7808181224114"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="p695725617435"><a name="p695725617435"></a><a name="p695725617435"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="p12808121264118"><a name="p12808121264118"></a><a name="p12808121264118"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><p id="p108081912194120"><a name="p108081912194120"></a><a name="p108081912194120"></a>路由器的UUID。</p>
</td>
</tr>
<tr id="row18808151274111"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="p5808141224118"><a name="p5808141224118"></a><a name="p5808141224118"></a>internal_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="p781614578434"><a name="p781614578434"></a><a name="p781614578434"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="p10808212124113"><a name="p10808212124113"></a><a name="p10808212124113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><p id="p4808171224115"><a name="p4808171224115"></a><a name="p4808171224115"></a>NAT网关下行口（DVR的下一跳）所属的network id。</p>
</td>
</tr>
<tr id="row16808412104117"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="p1380821214116"><a name="p1380821214116"></a><a name="p1380821214116"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="p203831458144310"><a name="p203831458144310"></a><a name="p203831458144310"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="p6808181284110"><a name="p6808181284110"></a><a name="p6808181284110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><a name="ul68084129415"></a><a name="ul68084129415"></a><ul id="ul68084129415"><li>功能说明：NAT网关的状态。</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="row18808141244119"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="p1780816122417"><a name="p1780816122417"></a><a name="p1780816122417"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="p646565974314"><a name="p646565974314"></a><a name="p646565974314"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="p1764614265487"><a name="p1764614265487"></a><a name="p1764614265487"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><a name="ul71858556358"></a><a name="ul71858556358"></a><ul id="ul71858556358"><li>解冻/冻结状态。</li><li>取值范围：<a name="ul11838172814409"></a><a name="ul11838172814409"></a><ul id="ul11838172814409"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="row138088125411"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="p1680831254112"><a name="p1680831254112"></a><a name="p1680831254112"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="p173616110445"><a name="p173616110445"></a><a name="p173616110445"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="p1180818124411"><a name="p1180818124411"></a><a name="p1180818124411"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><p id="p182375159231"><a name="p182375159231"></a><a name="p182375159231"></a>NAT网关的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section12659140"></a>

无

## 响应消息<a name="section46823401"></a>

响应参数如[表2](#table8843312114313)所示。

**表 2**  响应参数

<a name="table8843312114313"></a>
<table><thead align="left"><tr id="row10874912134313"><th class="cellrowborder" valign="top" width="20.200000000000003%" id="mcps1.2.4.1.1"><p id="p1887410126437"><a name="p1887410126437"></a><a name="p1887410126437"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="28.28%" id="mcps1.2.4.1.2"><p id="p188749126436"><a name="p188749126436"></a><a name="p188749126436"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.519999999999996%" id="mcps1.2.4.1.3"><p id="p14874111234319"><a name="p14874111234319"></a><a name="p14874111234319"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1787461216433"><td class="cellrowborder" valign="top" width="20.200000000000003%" headers="mcps1.2.4.1.1 "><p id="p48741812124312"><a name="p48741812124312"></a><a name="p48741812124312"></a>nat_gateways</p>
</td>
<td class="cellrowborder" valign="top" width="28.28%" headers="mcps1.2.4.1.2 "><p id="p14874512194313"><a name="p14874512194313"></a><a name="p14874512194313"></a>List(nat_gateway)</p>
</td>
<td class="cellrowborder" valign="top" width="51.519999999999996%" headers="mcps1.2.4.1.3 "><p id="p129411120422"><a name="p129411120422"></a><a name="p129411120422"></a>nat_gateway对象列表。详见<a href="#table1810691174217">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  nat\_gateway字段说明

<a name="table1810691174217"></a>
<table><thead align="left"><tr id="row15294131114425"><th class="cellrowborder" valign="top" width="20.14%" id="mcps1.2.4.1.1"><p id="p029451114211"><a name="p029451114211"></a><a name="p029451114211"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="27.810000000000002%" id="mcps1.2.4.1.2"><p id="p18294511134216"><a name="p18294511134216"></a><a name="p18294511134216"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="52.05%" id="mcps1.2.4.1.3"><p id="p102941011144211"><a name="p102941011144211"></a><a name="p102941011144211"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row929451134215"><td class="cellrowborder" valign="top" width="20.14%" headers="mcps1.2.4.1.1 "><p id="p102941911114216"><a name="p102941911114216"></a><a name="p102941911114216"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="27.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p629481118424"><a name="p629481118424"></a><a name="p629481118424"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.05%" headers="mcps1.2.4.1.3 "><p id="p1429411117423"><a name="p1429411117423"></a><a name="p1429411117423"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="row1329471104211"><td class="cellrowborder" valign="top" width="20.14%" headers="mcps1.2.4.1.1 "><p id="p82941511164216"><a name="p82941511164216"></a><a name="p82941511164216"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="27.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p17294011144211"><a name="p17294011144211"></a><a name="p17294011144211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.05%" headers="mcps1.2.4.1.3 "><p id="p19294181174214"><a name="p19294181174214"></a><a name="p19294181174214"></a>项目的ID。</p>
</td>
</tr>
<tr id="row8294151112421"><td class="cellrowborder" valign="top" width="20.14%" headers="mcps1.2.4.1.1 "><p id="p629441174214"><a name="p629441174214"></a><a name="p629441174214"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="27.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p12294161110426"><a name="p12294161110426"></a><a name="p12294161110426"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="52.05%" headers="mcps1.2.4.1.3 "><p id="p1329414115428"><a name="p1329414115428"></a><a name="p1329414115428"></a>NAT网关的名字。</p>
<p id="p529420111420"><a name="p529420111420"></a><a name="p529420111420"></a>NAT网关的名字仅支持数字、字母、_（下划线）、-（中划线）、中文。</p>
</td>
</tr>
<tr id="row229451119425"><td class="cellrowborder" valign="top" width="20.14%" headers="mcps1.2.4.1.1 "><p id="p17294411174218"><a name="p17294411174218"></a><a name="p17294411174218"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="27.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p1629412114426"><a name="p1629412114426"></a><a name="p1629412114426"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="52.05%" headers="mcps1.2.4.1.3 "><p id="p142947116421"><a name="p142947116421"></a><a name="p142947116421"></a>NAT网关的描述。</p>
</td>
</tr>
<tr id="row1829421134210"><td class="cellrowborder" valign="top" width="20.14%" headers="mcps1.2.4.1.1 "><p id="p13294121194215"><a name="p13294121194215"></a><a name="p13294121194215"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="27.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p1629411118423"><a name="p1629411118423"></a><a name="p1629411118423"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.05%" headers="mcps1.2.4.1.3 "><p id="p1329410119429"><a name="p1329410119429"></a><a name="p1329410119429"></a>NAT网关的规格。</p>
<p id="p1429413113429"><a name="p1429413113429"></a><a name="p1429413113429"></a>取值为：</p>
<a name="ul3294191111427"></a><a name="ul3294191111427"></a><ul id="ul3294191111427"><li>“1”：小型，SNAT最大连接数10000</li><li>“2”：中型，SNAT最大连接数50000</li><li>“3”：大型，SNAT最大连接数200000</li><li>“4”：超大型，SNAT最大连接数1000000</li></ul>
</td>
</tr>
<tr id="row1329416115424"><td class="cellrowborder" valign="top" width="20.14%" headers="mcps1.2.4.1.1 "><p id="p629416117428"><a name="p629416117428"></a><a name="p629416117428"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="27.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p329418118427"><a name="p329418118427"></a><a name="p329418118427"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.05%" headers="mcps1.2.4.1.3 "><p id="p429410118427"><a name="p429410118427"></a><a name="p429410118427"></a>路由器的UUID。</p>
</td>
</tr>
<tr id="row9294151184215"><td class="cellrowborder" valign="top" width="20.14%" headers="mcps1.2.4.1.1 "><p id="p4294151104220"><a name="p4294151104220"></a><a name="p4294151104220"></a>internal_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="27.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p6294121115424"><a name="p6294121115424"></a><a name="p6294121115424"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.05%" headers="mcps1.2.4.1.3 "><p id="p52948115428"><a name="p52948115428"></a><a name="p52948115428"></a>NAT网关下行口（DVR的下一跳）所属的network id。</p>
</td>
</tr>
<tr id="row182946117421"><td class="cellrowborder" valign="top" width="20.14%" headers="mcps1.2.4.1.1 "><p id="p172941011194220"><a name="p172941011194220"></a><a name="p172941011194220"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="27.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p172942119421"><a name="p172942119421"></a><a name="p172942119421"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.05%" headers="mcps1.2.4.1.3 "><a name="ul8294181134219"></a><a name="ul8294181134219"></a><ul id="ul8294181134219"><li>功能说明：NAT网关的状态。</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="row1629421184215"><td class="cellrowborder" valign="top" width="20.14%" headers="mcps1.2.4.1.1 "><p id="p2294171112421"><a name="p2294171112421"></a><a name="p2294171112421"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="27.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p159281825725"><a name="p159281825725"></a><a name="p159281825725"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="52.05%" headers="mcps1.2.4.1.3 "><a name="ul1238147165311"></a><a name="ul1238147165311"></a><ul id="ul1238147165311"><li>解冻/冻结状态。</li><li>取值范围：<a name="ul19394755315"></a><a name="ul19394755315"></a><ul id="ul19394755315"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="row19294121144218"><td class="cellrowborder" valign="top" width="20.14%" headers="mcps1.2.4.1.1 "><p id="p1529417112428"><a name="p1529417112428"></a><a name="p1529417112428"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="27.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p0294151110422"><a name="p0294151110422"></a><a name="p0294151110422"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.05%" headers="mcps1.2.4.1.3 "><p id="p14616181615910"><a name="p14616181615910"></a><a name="p14616181615910"></a>NAT网关的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section18757432"></a>

-   请求样例

    ```
    GET https://{Endpoint}/v2.0/nat_gateways?limit=10
    ```


-   响应样例

    ```
    {
         "nat_gateways": [ 
             { 
                 "router_id": "b1d81744-5165-48b8-916e-e56626feb88f", 
                 "status": "ACTIVE", 
                 "description": "", 
                 "admin_state_up": true, 
                 "tenant_id": "27e25061336f4af590faeabeb7fcd9a3", 
                 "created_at": "2017-11-15 14:50:39.505112", 
                 "spec": "2", 
                 "internal_network_id": "5930796a-6026-4d8b-8790-6c6bfc9f87e8", 
                 "id": "a253be25-ae7c-4013-978b-3c0785eccd63",
                 "name": "wj3" 
             }, 
             { 
                 "router_id": "305dc52f-13dd-429b-a2d4-444a1039ba0b", 
                 "status": "ACTIVE", 
                 "description": "", 
                 "admin_state_up": true, 
                 "tenant_id": "27e25061336f4af590faeabeb7fcd9a3", 
                 "created_at": "2017-11-17 07:41:07.538062", 
                 "spec": "2", 
                 "internal_network_id": "fc09463b-4ef8-4c7a-93c8-92d9ca6daf9d", 
                 "id": "e824f1b4-4290-4ebc-8322-cfff370dbd1e", 
                 "name": "lyl001" 
            }
        ]
    }
    ```


## 状态码<a name="section42956987"></a>

请参考[状态码](状态码.md)。

