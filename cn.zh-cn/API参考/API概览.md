# API概览<a name="zh-cn_topic_0083011468"></a>

通过使用NAT网关服务所提供的接口，您可以完整的使用NAT网关服务的所有功能。

## API v2<a name="section1858610519143"></a>

**表 1**  NAT网关v2接口类型

<a name="table618264141112"></a>
<table><thead align="left"><tr id="row151831417111"><th class="cellrowborder" valign="top" width="21.62%" id="mcps1.2.3.1.1"><p id="p818318418119"><a name="p818318418119"></a><a name="p818318418119"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="78.38000000000001%" id="mcps1.2.3.1.2"><p id="p718311481119"><a name="p718311481119"></a><a name="p718311481119"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row191837451117"><td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.2.3.1.1 "><p id="p14183154141113"><a name="p14183154141113"></a><a name="p14183154141113"></a><a href="NAT网关-0.md">NAT网关</a></p>
</td>
<td class="cellrowborder" valign="top" width="78.38000000000001%" headers="mcps1.2.3.1.2 "><p id="p918314415117"><a name="p918314415117"></a><a name="p918314415117"></a>支持对NAT网关进行创建、查询、更新、删除等操作，包括创建NAT网关、查询NAT网关列表、查询指定的NAT网关详情、更新NAT网关、删除NAT网关等接口。</p>
</td>
</tr>
<tr id="row171831415111"><td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.2.3.1.1 "><p id="p101832416112"><a name="p101832416112"></a><a name="p101832416112"></a><a href="SNAT规则-1.md">SNAT规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="78.38000000000001%" headers="mcps1.2.3.1.2 "><p id="p21838410115"><a name="p21838410115"></a><a name="p21838410115"></a>支持创建、查询、更新、删除SNAT规则，包括创建SNAT规则、查询SNAT规则列表、查询指定的SNAT规则详情、更新SNAT规则、删除SNAT规则等接口。</p>
</td>
</tr>
<tr id="row18183194131112"><td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.2.3.1.1 "><p id="p418314171116"><a name="p418314171116"></a><a name="p418314171116"></a><a href="DNAT规则-2.md">DNAT规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="78.38000000000001%" headers="mcps1.2.3.1.2 "><p id="p171838412119"><a name="p171838412119"></a><a name="p171838412119"></a>支持创建、查询、更新、删除DNAT规则，包括创建DNAT规则、批量创建DNAT规则、查询DNAT规则列表、查询指定的DNAT规则详情、更新DNAT规则、删除DNAT规则等接口。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  NAT网关v2接口说明

<a name="table11491174735917"></a>
<table><thead align="left"><tr id="row154912475592"><th class="cellrowborder" valign="top" width="21.529999999999998%" id="mcps1.2.4.1.1"><p id="p88518407412"><a name="p88518407412"></a><a name="p88518407412"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="32.23%" id="mcps1.2.4.1.2"><p id="p1049104710593"><a name="p1049104710593"></a><a name="p1049104710593"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="46.239999999999995%" id="mcps1.2.4.1.3"><p id="p74912475597"><a name="p74912475597"></a><a name="p74912475597"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1449124710592"><td class="cellrowborder" rowspan="5" valign="top" width="21.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p14369546611"><a name="p14369546611"></a><a name="p14369546611"></a><a href="NAT网关.md">NAT网关</a></p>
</td>
<td class="cellrowborder" valign="top" width="32.23%" headers="mcps1.2.4.1.2 "><p id="p1550485114115"><a name="p1550485114115"></a><a name="p1550485114115"></a><a href="创建NAT网关_v2.md">创建NAT网关</a></p>
</td>
<td class="cellrowborder" valign="top" width="46.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p57869722"><a name="p57869722"></a><a name="p57869722"></a>创建NAT网关实例。</p>
</td>
</tr>
<tr id="row1521981914118"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p021916191116"><a name="p021916191116"></a><a name="p021916191116"></a><a href="查询NAT网关列表_v2.md">查询NAT网关列表</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p53449151"><a name="p53449151"></a><a name="p53449151"></a>查询NAT网关列表。</p>
</td>
</tr>
<tr id="row1624919231514"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p6249172310114"><a name="p6249172310114"></a><a name="p6249172310114"></a><a href="查询指定的NAT网关详情_v2.md">查询指定的NAT网关详情</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p2249152317111"><a name="p2249152317111"></a><a name="p2249152317111"></a>查询指定的NAT网关详情。</p>
</td>
</tr>
<tr id="row12567426918"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p156718264116"><a name="p156718264116"></a><a name="p156718264116"></a><a href="更新NAT网关_v2.md">更新NAT网关</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p10315194"><a name="p10315194"></a><a name="p10315194"></a>更新NAT网关。</p>
</td>
</tr>
<tr id="row05686265114"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p135685261513"><a name="p135685261513"></a><a name="p135685261513"></a><a href="删除NAT网关_v2.md">删除NAT网关</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p57538383"><a name="p57538383"></a><a name="p57538383"></a>删除NAT网关。</p>
</td>
</tr>
<tr id="row7288113015117"><td class="cellrowborder" rowspan="5" valign="top" width="21.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p16585144913514"><a name="p16585144913514"></a><a name="p16585144913514"></a><a href="SNAT规则.md">SNAT规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="32.23%" headers="mcps1.2.4.1.2 "><p id="p142889301110"><a name="p142889301110"></a><a name="p142889301110"></a><a href="创建SNAT规则_v2.md">创建SNAT规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="46.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p8229815153013"><a name="p8229815153013"></a><a name="p8229815153013"></a>创建SNAT规则。</p>
</td>
</tr>
<tr id="row1528863020117"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p122885305116"><a name="p122885305116"></a><a name="p122885305116"></a><a href="查询SNAT规则列表_v2.md">查询SNAT规则列表</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p9288203011113"><a name="p9288203011113"></a><a name="p9288203011113"></a>查询SNAT规则列表。</p>
</td>
</tr>
<tr id="row128815301617"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p1628816301117"><a name="p1628816301117"></a><a name="p1628816301117"></a><a href="查询指定的SNAT规则详情_v2.md">查询指定的SNAT规则详情</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p6289123019113"><a name="p6289123019113"></a><a name="p6289123019113"></a>查询指定的SNAT规则详情。</p>
</td>
</tr>
<tr id="row12895301216"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p1828916303114"><a name="p1828916303114"></a><a name="p1828916303114"></a><a href="更新SNAT规则_v2.md">更新SNAT规则</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p1935815471264"><a name="p1935815471264"></a><a name="p1935815471264"></a>更新SNAT规则。</p>
</td>
</tr>
<tr id="row171191946414"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p911954611112"><a name="p911954611112"></a><a name="p911954611112"></a><a href="删除SNAT规则_v2.md">删除SNAT规则</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p59418700"><a name="p59418700"></a><a name="p59418700"></a>删除SNAT规则。</p>
</td>
</tr>
<tr id="row2011911461114"><td class="cellrowborder" rowspan="6" valign="top" width="21.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p1571123914812"><a name="p1571123914812"></a><a name="p1571123914812"></a><a href="DNAT规则.md">DNAT规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="32.23%" headers="mcps1.2.4.1.2 "><p id="p1611914461514"><a name="p1611914461514"></a><a name="p1611914461514"></a><a href="创建DNAT规则_v2.md">创建DNAT规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="46.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p558179021710"><a name="p558179021710"></a><a name="p558179021710"></a>创建DNAT规则。</p>
</td>
</tr>
<tr id="row9119246714"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p111911468117"><a name="p111911468117"></a><a name="p111911468117"></a><a href="批量创建DNAT规则_v2.md">批量创建DNAT规则</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p16119194617112"><a name="p16119194617112"></a><a name="p16119194617112"></a>批量创建DNAT规则。</p>
</td>
</tr>
<tr id="row4119194614113"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p011911461414"><a name="p011911461414"></a><a name="p011911461414"></a><a href="查询DNAT规则列表_v2.md">查询DNAT规则列表</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p11319755164149"><a name="p11319755164149"></a><a name="p11319755164149"></a>查询DNAT规则列表。</p>
</td>
</tr>
<tr id="row5119134617116"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p91197465119"><a name="p91197465119"></a><a name="p91197465119"></a><a href="查询指定的DNAT规则详情_v2.md">查询指定的DNAT规则详情</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p24472239165022"><a name="p24472239165022"></a><a name="p24472239165022"></a>查询指定的DNAT规则详情。</p>
</td>
</tr>
<tr id="row1511954620112"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p311964617114"><a name="p311964617114"></a><a name="p311964617114"></a><a href="更新DNAT规则_v2.md">更新DNAT规则</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p6744195611486"><a name="p6744195611486"></a><a name="p6744195611486"></a>更新DNAT规则。</p>
</td>
</tr>
<tr id="row6119646512"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p312013463118"><a name="p312013463118"></a><a name="p312013463118"></a><a href="删除DNAT规则_v2.md">删除DNAT规则</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p2980712017119"><a name="p2980712017119"></a><a name="p2980712017119"></a>删除DNAT规则。</p>
</td>
</tr>
</tbody>
</table>

## API v2.0<a name="section1271642212268"></a>

**表 3**  NAT网关v2.0接口类型

<a name="table277111483220"></a>
<table><thead align="left"><tr id="row27715144329"><th class="cellrowborder" valign="top" width="21.62%" id="mcps1.2.3.1.1"><p id="p4771614153213"><a name="p4771614153213"></a><a name="p4771614153213"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="78.38000000000001%" id="mcps1.2.3.1.2"><p id="p1577131493213"><a name="p1577131493213"></a><a name="p1577131493213"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row147791415320"><td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.2.3.1.1 "><p id="p1877101414323"><a name="p1877101414323"></a><a name="p1877101414323"></a><a href="NAT网关-0.md">NAT网关</a></p>
</td>
<td class="cellrowborder" valign="top" width="78.38000000000001%" headers="mcps1.2.3.1.2 "><p id="p137818148329"><a name="p137818148329"></a><a name="p137818148329"></a>支持对NAT网关进行创建、查询、更新、删除等操作，包括创建NAT网关、查询NAT网关列表、查询NAT网关、更新NAT网关、删除NAT网关等接口。</p>
</td>
</tr>
<tr id="row778151418321"><td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.2.3.1.1 "><p id="p1078101403214"><a name="p1078101403214"></a><a name="p1078101403214"></a><a href="SNAT规则-1.md">SNAT规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="78.38000000000001%" headers="mcps1.2.3.1.2 "><p id="p1878131463213"><a name="p1878131463213"></a><a name="p1878131463213"></a>支持创建、查询、删除SNAT规则，包括创建SNAT规则、查询SNAT规则列表、查询SNAT规则、删除SNAT规则等接口。</p>
</td>
</tr>
<tr id="row1078121443217"><td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.2.3.1.1 "><p id="p117841418329"><a name="p117841418329"></a><a name="p117841418329"></a><a href="DNAT规则-2.md">DNAT规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="78.38000000000001%" headers="mcps1.2.3.1.2 "><p id="p127816140326"><a name="p127816140326"></a><a name="p127816140326"></a>支持创建、查询、删除DNAT规则，包括创建DNAT规则、查询DNAT规则列表、查询DNAT规则、删除DNAT规则等接口。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  NAT网关v2.0接口说明

<a name="table201951814131620"></a>
<table><thead align="left"><tr id="row019514144168"><th class="cellrowborder" valign="top" width="21.529999999999998%" id="mcps1.2.4.1.1"><p id="p11951514131618"><a name="p11951514131618"></a><a name="p11951514131618"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="32.23%" id="mcps1.2.4.1.2"><p id="p16195101413164"><a name="p16195101413164"></a><a name="p16195101413164"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="46.239999999999995%" id="mcps1.2.4.1.3"><p id="p8195614171615"><a name="p8195614171615"></a><a name="p8195614171615"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row131951714191620"><td class="cellrowborder" rowspan="5" valign="top" width="21.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p612893941620"><a name="p612893941620"></a><a name="p612893941620"></a><a href="NAT网关-0.md">NAT网关</a></p>
</td>
<td class="cellrowborder" valign="top" width="32.23%" headers="mcps1.2.4.1.2 "><p id="p912783913162"><a name="p912783913162"></a><a name="p912783913162"></a><a href="创建NAT网关.md">创建NAT网关</a></p>
</td>
<td class="cellrowborder" valign="top" width="46.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p41261339141617"><a name="p41261339141617"></a><a name="p41261339141617"></a>创建NAT网关实例。</p>
</td>
</tr>
<tr id="row419551416161"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p0126183910164"><a name="p0126183910164"></a><a name="p0126183910164"></a><a href="查询NAT网关列表.md">查询NAT网关列表</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p151251439151618"><a name="p151251439151618"></a><a name="p151251439151618"></a>查询NAT网关列表。</p>
</td>
</tr>
<tr id="row13195714131614"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p61246391162"><a name="p61246391162"></a><a name="p61246391162"></a><a href="查询指定的NAT网关详情.md">查询指定的NAT网关详情</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p17123173991618"><a name="p17123173991618"></a><a name="p17123173991618"></a>查询指定的NAT网关详情。</p>
</td>
</tr>
<tr id="row1419581481616"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p201238393166"><a name="p201238393166"></a><a name="p201238393166"></a><a href="更新NAT网关.md">更新NAT网关</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p9122103911162"><a name="p9122103911162"></a><a name="p9122103911162"></a>更新NAT网关。</p>
</td>
</tr>
<tr id="row119551451619"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p612215395166"><a name="p612215395166"></a><a name="p612215395166"></a><a href="删除NAT网关.md">删除NAT网关</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p14121123991611"><a name="p14121123991611"></a><a name="p14121123991611"></a>删除NAT网关。</p>
</td>
</tr>
<tr id="row20196191418169"><td class="cellrowborder" rowspan="4" valign="top" width="21.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p1312143991613"><a name="p1312143991613"></a><a name="p1312143991613"></a><a href="SNAT规则-1.md">SNAT规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="32.23%" headers="mcps1.2.4.1.2 "><p id="p5120139111618"><a name="p5120139111618"></a><a name="p5120139111618"></a><a href="创建SNAT规则.md">创建SNAT规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="46.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p13630721105118"><a name="p13630721105118"></a><a name="p13630721105118"></a>创建SNAT规则。</p>
</td>
</tr>
<tr id="row91968149166"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p191191439121611"><a name="p191191439121611"></a><a name="p191191439121611"></a><a href="查询SNAT规则列表.md">查询SNAT规则列表</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p21184395161"><a name="p21184395161"></a><a name="p21184395161"></a>查询SNAT规则列表。</p>
</td>
</tr>
<tr id="row1519651414162"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p1111853951617"><a name="p1111853951617"></a><a name="p1111853951617"></a><a href="查询指定的SNAT规则详情.md">查询指定的SNAT规则详情</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p13117139101611"><a name="p13117139101611"></a><a name="p13117139101611"></a>查询指定的SNAT规则详情。</p>
</td>
</tr>
<tr id="row919651413169"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p411653921619"><a name="p411653921619"></a><a name="p411653921619"></a><a href="删除SNAT规则.md">删除SNAT规则</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p3116153919168"><a name="p3116153919168"></a><a name="p3116153919168"></a>删除SNAT规则。</p>
</td>
</tr>
<tr id="row31961514151615"><td class="cellrowborder" rowspan="4" valign="top" width="21.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p411412399165"><a name="p411412399165"></a><a name="p411412399165"></a><a href="DNAT规则-2.md">DNAT规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="32.23%" headers="mcps1.2.4.1.2 "><p id="p1211318398163"><a name="p1211318398163"></a><a name="p1211318398163"></a><a href="创建DNAT规则.md">创建DNAT规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="46.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p8591194814516"><a name="p8591194814516"></a><a name="p8591194814516"></a>创建DNAT规则</p>
</td>
</tr>
<tr id="row1119641417169"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p1611211399169"><a name="p1611211399169"></a><a name="p1611211399169"></a><a href="查询DNAT规则列表.md">查询DNAT规则列表</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p18112839181613"><a name="p18112839181613"></a><a name="p18112839181613"></a>查询DNAT规则列表。</p>
</td>
</tr>
<tr id="row61962014121616"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p91111398161"><a name="p91111398161"></a><a name="p91111398161"></a><a href="查询指定的DNAT规则详情.md">查询指定的DNAT规则详情</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p2110193931618"><a name="p2110193931618"></a><a name="p2110193931618"></a>查询指定的DNAT规则详情。</p>
</td>
</tr>
<tr id="row119615145167"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p181091039191616"><a name="p181091039191616"></a><a name="p181091039191616"></a><a href="删除DNAT规则.md">删除DNAT规则</a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p6108839181614"><a name="p6108839181614"></a><a name="p6108839181614"></a>删除DNAT规则。</p>
</td>
</tr>
</tbody>
</table>

