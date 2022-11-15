# 支持审计的关键操作列表<a name="nat_cts_0001"></a>

通过云审计服务，您可以记录与NAT网关相关的操作事件，便于日后的查询、审计和回溯。

云审计支持的公网NAT网关操作事件列表如[表1](#zh-cn_topic_0107344478_table1419082716297)所示。

云审计支持的私网NAT网关操作事件列表如[表2](#table18203355141715)所示。

**表 1**  云审计服务支持的公网NAT网关操作列表

<a name="zh-cn_topic_0107344478_table1419082716297"></a>
<table><thead align="left"><tr id="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_zh-cn_topic_0043877303_row20363337194626"><th class="cellrowborder" valign="top" width="31.630000000000003%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_zh-cn_topic_0043877303_p38817639194626"><a name="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_zh-cn_topic_0043877303_p38817639194626"></a><a name="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_zh-cn_topic_0043877303_p38817639194626"></a>操作名称</p>
</th>
<th class="cellrowborder" valign="top" width="28.57%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_zh-cn_topic_0043877303_p57221065194626"><a name="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_zh-cn_topic_0043877303_p57221065194626"></a><a name="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_zh-cn_topic_0043877303_p57221065194626"></a>资源类型</p>
</th>
<th class="cellrowborder" valign="top" width="39.800000000000004%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_zh-cn_topic_0043877303_p4394712194626"><a name="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_zh-cn_topic_0043877303_p4394712194626"></a><a name="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_zh-cn_topic_0043877303_p4394712194626"></a>事件名称</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_zh-cn_topic_0043877303_row20427387194626"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="p026775221616"><a name="p026775221616"></a><a name="p026775221616"></a>创建公网NAT网关</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p895145319197"><a name="p895145319197"></a><a name="p895145319197"></a>natgateway</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p4933516101716"><a name="p4933516101716"></a><a name="p4933516101716"></a>createNatGateway</p>
</td>
</tr>
<tr id="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_zh-cn_topic_0043877303_row34959088194626"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_p40002746102657"><a name="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_p40002746102657"></a><a name="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_p40002746102657"></a>修改公网NAT网关</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p79315341910"><a name="p79315341910"></a><a name="p79315341910"></a>natgateway</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p95406212013"><a name="p95406212013"></a><a name="p95406212013"></a>updateNatGateway</p>
</td>
</tr>
<tr id="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_zh-cn_topic_0043877303_row59839823194626"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_p36754893102657"><a name="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_p36754893102657"></a><a name="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_p36754893102657"></a>删除公网NAT网关</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p109255315193"><a name="p109255315193"></a><a name="p109255315193"></a>natgateway</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p38311019201"><a name="p38311019201"></a><a name="p38311019201"></a>deleteNatGateway</p>
</td>
</tr>
<tr id="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_zh-cn_topic_0043877303_row31578295194626"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_p17880695102657"><a name="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_p17880695102657"></a><a name="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_p17880695102657"></a>创建公网NAT网关DNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p9911533199"><a name="p9911533199"></a><a name="p9911533199"></a>dnatrule</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p927101822015"><a name="p927101822015"></a><a name="p927101822015"></a>createDnatRule</p>
</td>
</tr>
<tr id="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_zh-cn_topic_0043877303_row49694672194626"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="p20267115271615"><a name="p20267115271615"></a><a name="p20267115271615"></a>修改公网NAT网关DNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p15901653201912"><a name="p15901653201912"></a><a name="p15901653201912"></a>dnatrule</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p898219256202"><a name="p898219256202"></a><a name="p898219256202"></a>updateDnatRule</p>
</td>
</tr>
<tr id="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_zh-cn_topic_0043877303_row23432327194626"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="p1426745291618"><a name="p1426745291618"></a><a name="p1426745291618"></a>删除公网NAT网关DNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p688175311199"><a name="p688175311199"></a><a name="p688175311199"></a>dnatrule</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p44371733152015"><a name="p44371733152015"></a><a name="p44371733152015"></a>deleteDnatRule</p>
</td>
</tr>
<tr id="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_zh-cn_topic_0043877303_row66571733194626"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="p1226745211611"><a name="p1226745211611"></a><a name="p1226745211611"></a>创建公网NAT网关SNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p1287175331918"><a name="p1287175331918"></a><a name="p1287175331918"></a>snatrule</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p17374114072013"><a name="p17374114072013"></a><a name="p17374114072013"></a>createSnatRule</p>
</td>
</tr>
<tr id="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_zh-cn_topic_0043877303_row49521528194626"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="p112671752131612"><a name="p112671752131612"></a><a name="p112671752131612"></a>修改公网NAT网关SNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p1285165319195"><a name="p1285165319195"></a><a name="p1285165319195"></a>snatrule</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p118174507203"><a name="p118174507203"></a><a name="p118174507203"></a>updateSnatRule</p>
</td>
</tr>
<tr id="zh-cn_topic_0107344478_zh-cn_topic_0107211963_zh-cn_topic_0100273727_zh-cn_topic_0043877303_row3607478194626"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="p132679523167"><a name="p132679523167"></a><a name="p132679523167"></a>删除公网NAT网关SNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p127845381910"><a name="p127845381910"></a><a name="p127845381910"></a>snatrule</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p164421658112016"><a name="p164421658112016"></a><a name="p164421658112016"></a>deleteSnatRule</p>
</td>
</tr>
</tbody>
</table>

**表 2**  云审计服务支持的私网NAT网关操作列表

<a name="table18203355141715"></a>
<table><thead align="left"><tr id="row7203055121716"><th class="cellrowborder" valign="top" width="31.630000000000003%" id="mcps1.2.4.1.1"><p id="p11203125518175"><a name="p11203125518175"></a><a name="p11203125518175"></a>操作名称</p>
</th>
<th class="cellrowborder" valign="top" width="28.57%" id="mcps1.2.4.1.2"><p id="p12204955151713"><a name="p12204955151713"></a><a name="p12204955151713"></a>资源类型</p>
</th>
<th class="cellrowborder" valign="top" width="39.800000000000004%" id="mcps1.2.4.1.3"><p id="p18204055191713"><a name="p18204055191713"></a><a name="p18204055191713"></a>事件名称</p>
</th>
</tr>
</thead>
<tbody><tr id="row320416557179"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="p11204165518179"><a name="p11204165518179"></a><a name="p11204165518179"></a>创建私网NAT网关</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p12618105694610"><a name="p12618105694610"></a><a name="p12618105694610"></a>privateNat</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p176182563467"><a name="p176182563467"></a><a name="p176182563467"></a>createPrivateNat</p>
</td>
</tr>
<tr id="row12204555141716"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="p112043558178"><a name="p112043558178"></a><a name="p112043558178"></a>修改私网NAT网关</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p76181456154617"><a name="p76181456154617"></a><a name="p76181456154617"></a>privateNat</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p1561812569460"><a name="p1561812569460"></a><a name="p1561812569460"></a>updatePrivateNat</p>
</td>
</tr>
<tr id="row920585541718"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="p420517556176"><a name="p420517556176"></a><a name="p420517556176"></a>删除私网NAT网关</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p3618156164613"><a name="p3618156164613"></a><a name="p3618156164613"></a>privateNat</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p6618556164614"><a name="p6618556164614"></a><a name="p6618556164614"></a>deletePrivateNat</p>
</td>
</tr>
<tr id="row120514551176"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="p1220535514172"><a name="p1220535514172"></a><a name="p1220535514172"></a>创建私网NAT网关DNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p106191856134616"><a name="p106191856134616"></a><a name="p106191856134616"></a>privateDnatRule</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p1361935610469"><a name="p1361935610469"></a><a name="p1361935610469"></a>createPrivateDnatRule</p>
</td>
</tr>
<tr id="row62051655101710"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="p42051955141716"><a name="p42051955141716"></a><a name="p42051955141716"></a>修改私网NAT网关DNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p861910567463"><a name="p861910567463"></a><a name="p861910567463"></a>privateDnatRule</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p14619175644617"><a name="p14619175644617"></a><a name="p14619175644617"></a>updatePrivateDnatRule</p>
</td>
</tr>
<tr id="row18205455131710"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="p1720525511718"><a name="p1720525511718"></a><a name="p1720525511718"></a>删除私网NAT网关DNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p36191956174612"><a name="p36191956174612"></a><a name="p36191956174612"></a>privateDnatRule</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p126191556174615"><a name="p126191556174615"></a><a name="p126191556174615"></a>deletePrivateDnatRule</p>
</td>
</tr>
<tr id="row192051455181718"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="p2205195571716"><a name="p2205195571716"></a><a name="p2205195571716"></a>创建私网NAT网关SNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p1974254712478"><a name="p1974254712478"></a><a name="p1974254712478"></a>privateSnatRule</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p4742174724710"><a name="p4742174724710"></a><a name="p4742174724710"></a>createPrivateSnatRule</p>
</td>
</tr>
<tr id="row1620575511713"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="p32051455151711"><a name="p32051455151711"></a><a name="p32051455151711"></a>修改私网NAT网关SNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p1774214473472"><a name="p1774214473472"></a><a name="p1774214473472"></a>privateSnatRule</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p1674216476473"><a name="p1674216476473"></a><a name="p1674216476473"></a>updatePrivateSnatRule</p>
</td>
</tr>
<tr id="row1620575519176"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="p9205195531720"><a name="p9205195531720"></a><a name="p9205195531720"></a>删除私网NAT网关SNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p147421477477"><a name="p147421477477"></a><a name="p147421477477"></a>privateSnatRule</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p1743194712472"><a name="p1743194712472"></a><a name="p1743194712472"></a>deletePrivateSnatRule</p>
</td>
</tr>
<tr id="row16732591447"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="p667455934414"><a name="p667455934414"></a><a name="p667455934414"></a>创建中转子网</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p10619135694611"><a name="p10619135694611"></a><a name="p10619135694611"></a>transitSubnet</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p1561965611461"><a name="p1561965611461"></a><a name="p1561965611461"></a>createTransitSubnet</p>
</td>
</tr>
<tr id="row167415910448"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="p5674115994413"><a name="p5674115994413"></a><a name="p5674115994413"></a>修改中转子网</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p12619195613464"><a name="p12619195613464"></a><a name="p12619195613464"></a>transitSubnet</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p10619195616460"><a name="p10619195616460"></a><a name="p10619195616460"></a>updateTransitSubnet</p>
</td>
</tr>
<tr id="row16751259174418"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="p46751959174416"><a name="p46751959174416"></a><a name="p46751959174416"></a>删除中转子网</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p06191756164611"><a name="p06191756164611"></a><a name="p06191756164611"></a>transitSubnet</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p6619356194610"><a name="p6619356194610"></a><a name="p6619356194610"></a>deleteTransitSubnet</p>
</td>
</tr>
<tr id="row116751596441"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="p567615919447"><a name="p567615919447"></a><a name="p567615919447"></a>创建中转IP</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p061955684610"><a name="p061955684610"></a><a name="p061955684610"></a>transitIp</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p361945674620"><a name="p361945674620"></a><a name="p361945674620"></a>createTransitIp</p>
</td>
</tr>
<tr id="row13676125994418"><td class="cellrowborder" valign="top" width="31.630000000000003%" headers="mcps1.2.4.1.1 "><p id="p967665964415"><a name="p967665964415"></a><a name="p967665964415"></a>删除中转IP</p>
</td>
<td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p36191956154613"><a name="p36191956154613"></a><a name="p36191956154613"></a>transitip</p>
</td>
<td class="cellrowborder" valign="top" width="39.800000000000004%" headers="mcps1.2.4.1.3 "><p id="p1461955610465"><a name="p1461955610465"></a><a name="p1461955610465"></a>deleteTransitIp</p>
</td>
</tr>
</tbody>
</table>

