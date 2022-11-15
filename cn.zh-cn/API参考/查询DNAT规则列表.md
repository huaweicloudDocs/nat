# 查询DNAT规则列表<a name="ListNatGatewayDnatRules"></a>

## 功能介绍<a name="section17811811192619"></a>

查询DNAT规则列表。

## 接口约束<a name="section8812111113263"></a>

可以在URI后面用'?'和'&'添加不同的查询条件组合，支持参数说明中所有非必选参数过滤，请参考请求样例。

## 调试<a name="section08131211162617"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=nat&api=ListNatGatewayDnatRules)中调试该接口。

## URI<a name="section13814111112611"></a>

GET /v2/\{project\_id\}/dnat\_rules

**表 1**  路径参数

<a name="table2821131162612"></a>
<table><thead align="left"><tr id="row1981951111260"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p482391182615"><a name="p482391182615"></a><a name="p482391182615"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p1982411112268"><a name="p1982411112268"></a><a name="p1982411112268"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p6825171114264"><a name="p6825171114264"></a><a name="p6825171114264"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p1982511112262"><a name="p1982511112262"></a><a name="p1982511112262"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row7819151172619"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p178265114267"><a name="p178265114267"></a><a name="p178265114267"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p0826121114262"><a name="p0826121114262"></a><a name="p0826121114262"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1382771118268"><a name="p1382771118268"></a><a name="p1382771118268"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p168274114265"><a name="p168274114265"></a><a name="p168274114265"></a>项目的ID。</p>
<p id="p0827161122618"><a name="p0827161122618"></a><a name="p0827161122618"></a>最小长度：<strong id="b4828191112614"><a name="b4828191112614"></a><a name="b4828191112614"></a>1</strong></p>
<p id="p482816116262"><a name="p482816116262"></a><a name="p482816116262"></a>最大长度：<strong id="b1828611202619"><a name="b1828611202619"></a><a name="b1828611202619"></a>36</strong></p>
<p id="p2562026131319"><a name="p2562026131319"></a><a name="p2562026131319"></a>获取方法详见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  Query参数

<a name="table78311811152617"></a>
<table><thead align="left"><tr id="row1082910117263"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p18832611182619"><a name="p18832611182619"></a><a name="p18832611182619"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p188322011122615"><a name="p188322011122615"></a><a name="p188322011122615"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p6832711162612"><a name="p6832711162612"></a><a name="p6832711162612"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p1983371114260"><a name="p1983371114260"></a><a name="p1983371114260"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row178291811172615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p13834111192614"><a name="p13834111192614"></a><a name="p13834111192614"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p168341311142617"><a name="p168341311142617"></a><a name="p168341311142617"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1183511110269"><a name="p1183511110269"></a><a name="p1183511110269"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1197115016115"><a name="p1197115016115"></a><a name="p1197115016115"></a>解冻/冻结状态。取值范围：</p>
<p id="p155837921215"><a name="p155837921215"></a><a name="p155837921215"></a>"true"：解冻</p>
<p id="p17115154331114"><a name="p17115154331114"></a><a name="p17115154331114"></a>"false"：冻结</p>
</td>
</tr>
<tr id="row08291311112613"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1083671114265"><a name="p1083671114265"></a><a name="p1083671114265"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p483621182615"><a name="p483621182615"></a><a name="p483621182615"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p783771110263"><a name="p783771110263"></a><a name="p783771110263"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p583818110267"><a name="p583818110267"></a><a name="p583818110267"></a>Floatingip对外提供服务的端口号。取值范围：0~65535。</p>
<p id="p88384119260"><a name="p88384119260"></a><a name="p88384119260"></a>最小值：<strong id="b68388117267"><a name="b68388117267"></a><a name="b68388117267"></a>0</strong></p>
<p id="p5838611202614"><a name="p5838611202614"></a><a name="p5838611202614"></a>最大值：<strong id="b17839121142620"><a name="b17839121142620"></a><a name="b17839121142620"></a>65535</strong></p>
<p id="p17839911192610"><a name="p17839911192610"></a><a name="p17839911192610"></a>最小长度：<strong id="b10839121114260"><a name="b10839121114260"></a><a name="b10839121114260"></a>1</strong></p>
<p id="p1483918115266"><a name="p1483918115266"></a><a name="p1483918115266"></a>最大长度：<strong id="b1983981113265"><a name="b1983981113265"></a><a name="b1983981113265"></a>5</strong></p>
</td>
</tr>
<tr id="row682971115267"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p2839181119265"><a name="p2839181119265"></a><a name="p2839181119265"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p13840201110268"><a name="p13840201110268"></a><a name="p13840201110268"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p4841201112620"><a name="p4841201112620"></a><a name="p4841201112620"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p284151182617"><a name="p284151182617"></a><a name="p284151182617"></a>弹性公网的IP地址。</p>
<p id="p3842111132620"><a name="p3842111132620"></a><a name="p3842111132620"></a>最小长度：<strong id="b384251119260"><a name="b384251119260"></a><a name="b384251119260"></a>0</strong></p>
<p id="p284221115266"><a name="p284221115266"></a><a name="p284221115266"></a>最大长度：<strong id="b3842151112618"><a name="b3842151112618"></a><a name="b3842151112618"></a>1024</strong></p>
</td>
</tr>
<tr id="row182951122617"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p38425114263"><a name="p38425114263"></a><a name="p38425114263"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p8843131192615"><a name="p8843131192615"></a><a name="p8843131192615"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p684491142617"><a name="p684491142617"></a><a name="p684491142617"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p784401152613"><a name="p784401152613"></a><a name="p784401152613"></a>Dnat规则的状态。</p>
<p id="p18844101114266"><a name="p18844101114266"></a><a name="p18844101114266"></a>枚举值：</p>
<a name="ul1845911132619"></a><a name="ul1845911132619"></a><ul id="ul1845911132619"><li><strong id="b108451211102616"><a name="b108451211102616"></a><a name="b108451211102616"></a>ACTIVE</strong></li><li><strong id="b1984651192614"><a name="b1984651192614"></a><a name="b1984651192614"></a>PENDING_CREATE</strong></li><li><strong id="b20846211152616"><a name="b20846211152616"></a><a name="b20846211152616"></a>PENDING_UPDATE</strong></li><li><strong id="b2847141119262"><a name="b2847141119262"></a><a name="b2847141119262"></a>PENDING_DELETE</strong></li><li><strong id="b8847141119263"><a name="b8847141119263"></a><a name="b8847141119263"></a>EIP_FREEZED</strong></li><li><strong id="b17847611122616"><a name="b17847611122616"></a><a name="b17847611122616"></a>INACTIVE</strong></li></ul>
</td>
</tr>
<tr id="row1182971162620"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p5848201118265"><a name="p5848201118265"></a><a name="p5848201118265"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p284812117262"><a name="p284812117262"></a><a name="p284812117262"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1684910117262"><a name="p1684910117262"></a><a name="p1684910117262"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1184971119263"><a name="p1184971119263"></a><a name="p1184971119263"></a>弹性公网IP的id。</p>
<p id="p1884911112269"><a name="p1884911112269"></a><a name="p1884911112269"></a>长度：<strong id="b18502112261"><a name="b18502112261"></a><a name="b18502112261"></a>36</strong></p>
</td>
</tr>
<tr id="row118301011152619"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p12850141113267"><a name="p12850141113267"></a><a name="p12850141113267"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p5851151122619"><a name="p5851151122619"></a><a name="p5851151122619"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p4851611122613"><a name="p4851611122613"></a><a name="p4851611122613"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p19852141102611"><a name="p19852141102611"></a><a name="p19852141102611"></a>虚拟机或者裸机对外提供服务的协议端口号。取值范围：0~65535。</p>
<p id="p208528119266"><a name="p208528119266"></a><a name="p208528119266"></a>最小值：<strong id="b1285251152617"><a name="b1285251152617"></a><a name="b1285251152617"></a>0</strong></p>
<p id="p78538113267"><a name="p78538113267"></a><a name="p78538113267"></a>最大值：<strong id="b138532115261"><a name="b138532115261"></a><a name="b138532115261"></a>65535</strong></p>
<p id="p1985313117267"><a name="p1985313117267"></a><a name="p1985313117267"></a>最小长度：<strong id="b128531711172616"><a name="b128531711172616"></a><a name="b128531711172616"></a>1</strong></p>
<p id="p585381182618"><a name="p585381182618"></a><a name="p585381182618"></a>最大长度：<strong id="b485315118263"><a name="b485315118263"></a><a name="b485315118263"></a>5</strong></p>
</td>
</tr>
<tr id="row883016114268"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p8854191110266"><a name="p8854191110266"></a><a name="p8854191110266"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p685451192613"><a name="p685451192613"></a><a name="p685451192613"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p19855171116267"><a name="p19855171116267"></a><a name="p19855171116267"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p188568115262"><a name="p188568115262"></a><a name="p188568115262"></a>功能说明：每页返回的个数。取值范围：0~2000。默认值：2000。</p>
<p id="p188561114263"><a name="p188561114263"></a><a name="p188561114263"></a>最小值：<strong id="b1856611102615"><a name="b1856611102615"></a><a name="b1856611102615"></a>1</strong></p>
<p id="p168561311132620"><a name="p168561311132620"></a><a name="p168561311132620"></a>最大值：<strong id="b085791192614"><a name="b085791192614"></a><a name="b085791192614"></a>2000</strong></p>
<p id="p485720111269"><a name="p485720111269"></a><a name="p485720111269"></a>缺省值：<strong id="b885751172610"><a name="b885751172610"></a><a name="b885751172610"></a>2000</strong></p>
</td>
</tr>
<tr id="row3830201162617"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p785710111267"><a name="p785710111267"></a><a name="p785710111267"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p185841118268"><a name="p185841118268"></a><a name="p185841118268"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p12858171116262"><a name="p12858171116262"></a><a name="p12858171116262"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p285931116267"><a name="p285931116267"></a><a name="p285931116267"></a>DNAT规则的ID。</p>
<p id="p885917118266"><a name="p885917118266"></a><a name="p885917118266"></a>最小长度：<strong id="b78591111142615"><a name="b78591111142615"></a><a name="b78591111142615"></a>1</strong></p>
<p id="p1285941115266"><a name="p1285941115266"></a><a name="p1285941115266"></a>最大长度：<strong id="b785921112268"><a name="b785921112268"></a><a name="b785921112268"></a>36</strong></p>
</td>
</tr>
<tr id="row983011117263"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p386017119263"><a name="p386017119263"></a><a name="p386017119263"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p12860181132617"><a name="p12860181132617"></a><a name="p12860181132617"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p486011119264"><a name="p486011119264"></a><a name="p486011119264"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p9861171120265"><a name="p9861171120265"></a><a name="p9861171120265"></a>DNAT规则的描述，长度限制为255。</p>
<p id="p3861181115261"><a name="p3861181115261"></a><a name="p3861181115261"></a>最大长度：<strong id="b1862211122617"><a name="b1862211122617"></a><a name="b1862211122617"></a>255</strong></p>
</td>
</tr>
<tr id="row4830161162617"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p2862211192612"><a name="p2862211192612"></a><a name="p2862211192612"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p168637115264"><a name="p168637115264"></a><a name="p168637115264"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p38631411112618"><a name="p38631411112618"></a><a name="p38631411112618"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1586481110260"><a name="p1586481110260"></a><a name="p1586481110260"></a>DNAT规则的创建时间，遵循UTC时间，格式是yyyy-mm-ddThh:mm:ssZ。</p>
<p id="p118649113263"><a name="p118649113263"></a><a name="p118649113263"></a>最小长度：<strong id="b2086515113266"><a name="b2086515113266"></a><a name="b2086515113266"></a>1</strong></p>
<p id="p28651411152612"><a name="p28651411152612"></a><a name="p28651411152612"></a>最大长度：<strong id="b18651911102619"><a name="b18651911102619"></a><a name="b18651911102619"></a>36</strong></p>
</td>
</tr>
<tr id="row16830171162615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p15865141172610"><a name="p15865141172610"></a><a name="p15865141172610"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p2867711172614"><a name="p2867711172614"></a><a name="p2867711172614"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p88671711122614"><a name="p88671711122614"></a><a name="p88671711122614"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p886818115269"><a name="p886818115269"></a><a name="p886818115269"></a>公网NAT网关实例的ID。</p>
</td>
</tr>
<tr id="row1083021162618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p168681311162615"><a name="p168681311162615"></a><a name="p168681311162615"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p786931162615"><a name="p786931162615"></a><a name="p786931162615"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1186911113264"><a name="p1186911113264"></a><a name="p1186911113264"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p17870121192615"><a name="p17870121192615"></a><a name="p17870121192615"></a>虚拟机或者裸机的Port ID，与private_ip参数二选一。</p>
<p id="p138701211142612"><a name="p138701211142612"></a><a name="p138701211142612"></a>最小值：<strong id="b787013116265"><a name="b787013116265"></a><a name="b787013116265"></a>0</strong></p>
<p id="p987161116260"><a name="p987161116260"></a><a name="p987161116260"></a>最大值：<strong id="b887118119263"><a name="b887118119263"></a><a name="b887118119263"></a>36</strong></p>
</td>
</tr>
<tr id="row28309111268"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p3871101118268"><a name="p3871101118268"></a><a name="p3871101118268"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p12873131120261"><a name="p12873131120261"></a><a name="p12873131120261"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p68747119263"><a name="p68747119263"></a><a name="p68747119263"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p987591115262"><a name="p987591115262"></a><a name="p987591115262"></a>用户私有IP地址，例如专线连接的私有云地址，与port_id参数二选一。</p>
</td>
</tr>
<tr id="row6830141112618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p387514113263"><a name="p387514113263"></a><a name="p387514113263"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1187651115264"><a name="p1187651115264"></a><a name="p1187651115264"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p48769113263"><a name="p48769113263"></a><a name="p48769113263"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p2877711192613"><a name="p2877711192613"></a><a name="p2877711192613"></a>协议类型，目前支持TCP/tcp、UDP/udp、ANY/any。对应协议号6、17、0。</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section4878811182617"></a>

**表 3**  请求Header参数

<a name="zh-cn_topic_0297140328_HeaderParameter"></a>
<table><thead align="left"><tr id="row587991172619"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p18811911192619"><a name="p18811911192619"></a><a name="p18811911192619"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p088121172614"><a name="p088121172614"></a><a name="p088121172614"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p17882191112615"><a name="p17882191112615"></a><a name="p17882191112615"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p168835119267"><a name="p168835119267"></a><a name="p168835119267"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row4879711172617"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1188313110265"><a name="p1188313110265"></a><a name="p1188313110265"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p788401122610"><a name="p788401122610"></a><a name="p788401122610"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p148856115269"><a name="p148856115269"></a><a name="p148856115269"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p20885101119267"><a name="p20885101119267"></a><a name="p20885101119267"></a>用户Token。用户Token也就是调用获取用户Token获取请求认证接口的响应值，该接口是唯一不需要认证的接口。请求响应成功后在响应消息头中包含的“X-Subject-Token”的值即为Token值。</p>
<p id="p1788610112266"><a name="p1788610112266"></a><a name="p1788610112266"></a>最小长度：<strong id="b588671192610"><a name="b588671192610"></a><a name="b588671192610"></a>1</strong></p>
<p id="p1488691152616"><a name="p1488691152616"></a><a name="p1488691152616"></a>最大长度：<strong id="b128861211102611"><a name="b128861211102611"></a><a name="b128861211102611"></a>10240</strong></p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section788711110268"></a>

**状态码： 200**

**表 4**  响应Body参数

<a name="zh-cn_topic_0297140328_responseParameter"></a>
<table><thead align="left"><tr id="row3888191119265"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p188891011132614"><a name="p188891011132614"></a><a name="p188891011132614"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1688991111265"><a name="p1688991111265"></a><a name="p1688991111265"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p789018118266"><a name="p789018118266"></a><a name="p789018118266"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row988831132614"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p16890141117269"><a name="p16890141117269"></a><a name="p16890141117269"></a>dnat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p5891111202611"><a name="p5891111202611"></a><a name="p5891111202611"></a>Array of <a href="#zh-cn_topic_0297140328_response_NatGatewayDnatRuleResponseBody">NatGatewayDnatRuleResponseBody</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p089216119269"><a name="p089216119269"></a><a name="p089216119269"></a>查询DNAT规则列表的响应体。</p>
</td>
</tr>
</tbody>
</table>

**表 5**  NatGatewayDnatRuleResponseBody

<a name="zh-cn_topic_0297140328_response_NatGatewayDnatRuleResponseBody"></a>
<table><thead align="left"><tr id="row1989319113268"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1589681117267"><a name="p1589681117267"></a><a name="p1589681117267"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p48967112264"><a name="p48967112264"></a><a name="p48967112264"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p789712113267"><a name="p789712113267"></a><a name="p789712113267"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row15893161119263"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p148981711112612"><a name="p148981711112612"></a><a name="p148981711112612"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p118981711102613"><a name="p118981711102613"></a><a name="p118981711102613"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p128998116268"><a name="p128998116268"></a><a name="p128998116268"></a>DNAT规则的ID。</p>
<p id="p2900131119263"><a name="p2900131119263"></a><a name="p2900131119263"></a>长度：<strong id="b1590031110264"><a name="b1590031110264"></a><a name="b1590031110264"></a>36</strong></p>
</td>
</tr>
<tr id="row10893151112268"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p89001711162617"><a name="p89001711162617"></a><a name="p89001711162617"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p69018119266"><a name="p69018119266"></a><a name="p69018119266"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p129011311172615"><a name="p129011311172615"></a><a name="p129011311172615"></a>项目的ID。</p>
</td>
</tr>
<tr id="row18893211142615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p690213113269"><a name="p690213113269"></a><a name="p690213113269"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p10902131122619"><a name="p10902131122619"></a><a name="p10902131122619"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1190312112265"><a name="p1190312112265"></a><a name="p1190312112265"></a>DNAT规则的描述。长度限制为255。</p>
<p id="p990314115260"><a name="p990314115260"></a><a name="p990314115260"></a>最大长度：<strong id="b2903311132620"><a name="b2903311132620"></a><a name="b2903311132620"></a>255</strong></p>
</td>
</tr>
<tr id="row10893011112616"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p16904171115262"><a name="p16904171115262"></a><a name="p16904171115262"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p3904121110269"><a name="p3904121110269"></a><a name="p3904121110269"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1905141192620"><a name="p1905141192620"></a><a name="p1905141192620"></a>虚拟机或者裸机的Port ID，与private_ip参数二选一。</p>
<p id="p10906711192617"><a name="p10906711192617"></a><a name="p10906711192617"></a>长度：<strong id="b129061811112616"><a name="b129061811112616"></a><a name="b129061811112616"></a>36</strong></p>
</td>
</tr>
<tr id="row6894131192618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p9907161182610"><a name="p9907161182610"></a><a name="p9907161182610"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12907111112614"><a name="p12907111112614"></a><a name="p12907111112614"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p790710110263"><a name="p790710110263"></a><a name="p790710110263"></a>用户私有IP地址，例如专线连接的私有云地址，与port_id参数二选一。</p>
</td>
</tr>
<tr id="row14894711202611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p99081011182614"><a name="p99081011182614"></a><a name="p99081011182614"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p5908141182612"><a name="p5908141182612"></a><a name="p5908141182612"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12909181132617"><a name="p12909181132617"></a><a name="p12909181132617"></a>虚拟机或者裸机对外提供服务的协议端口号。取值范围：0~65535。</p>
<p id="p13910611102612"><a name="p13910611102612"></a><a name="p13910611102612"></a>最小值：<strong id="b15910151118263"><a name="b15910151118263"></a><a name="b15910151118263"></a>0</strong></p>
<p id="p89102119261"><a name="p89102119261"></a><a name="p89102119261"></a>最大值：<strong id="b9910181162612"><a name="b9910181162612"></a><a name="b9910181162612"></a>65535</strong></p>
<p id="p391061112269"><a name="p391061112269"></a><a name="p391061112269"></a>最小长度：<strong id="b109101411152617"><a name="b109101411152617"></a><a name="b109101411152617"></a>1</strong></p>
<p id="p16911141113263"><a name="p16911141113263"></a><a name="p16911141113263"></a>最大长度：<strong id="b17911131132614"><a name="b17911131132614"></a><a name="b17911131132614"></a>5</strong></p>
</td>
</tr>
<tr id="row16894611122611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p0911131112263"><a name="p0911131112263"></a><a name="p0911131112263"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1691201112266"><a name="p1691201112266"></a><a name="p1691201112266"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2912131116264"><a name="p2912131116264"></a><a name="p2912131116264"></a>公网NAT网关实例的ID。</p>
<p id="p9913511112614"><a name="p9913511112614"></a><a name="p9913511112614"></a>最小长度：<strong id="b11913181102614"><a name="b11913181102614"></a><a name="b11913181102614"></a>1</strong></p>
<p id="p179132118262"><a name="p179132118262"></a><a name="p179132118262"></a>最大长度：<strong id="b5914181112613"><a name="b5914181112613"></a><a name="b5914181112613"></a>36</strong></p>
</td>
</tr>
<tr id="row1289471192615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1091471132618"><a name="p1091471132618"></a><a name="p1091471132618"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12914201142616"><a name="p12914201142616"></a><a name="p12914201142616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p159151811152617"><a name="p159151811152617"></a><a name="p159151811152617"></a>弹性公网IP的id。</p>
<p id="p1391551152618"><a name="p1391551152618"></a><a name="p1391551152618"></a>最小长度：<strong id="b109153112264"><a name="b109153112264"></a><a name="b109153112264"></a>1</strong></p>
<p id="p179161311102612"><a name="p179161311102612"></a><a name="p179161311102612"></a>最大长度：<strong id="b3916511152615"><a name="b3916511152615"></a><a name="b3916511152615"></a>36</strong></p>
</td>
</tr>
<tr id="row589411116267"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p179169113268"><a name="p179169113268"></a><a name="p179169113268"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p149171811152616"><a name="p149171811152616"></a><a name="p149171811152616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p119179115260"><a name="p119179115260"></a><a name="p119179115260"></a>弹性公网IP的IP地址。</p>
</td>
</tr>
<tr id="row28941711122611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p10918111152613"><a name="p10918111152613"></a><a name="p10918111152613"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p14919131132614"><a name="p14919131132614"></a><a name="p14919131132614"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p4919161111269"><a name="p4919161111269"></a><a name="p4919161111269"></a>Floatingip对外提供服务的端口号。取值范围：0~65535。</p>
</td>
</tr>
<tr id="row38941311162619"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11920171152614"><a name="p11920171152614"></a><a name="p11920171152614"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p5920191115263"><a name="p5920191115263"></a><a name="p5920191115263"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p19921111152620"><a name="p19921111152620"></a><a name="p19921111152620"></a>功能说明：DNAT规则的状态。</p>
<p id="p12921111182616"><a name="p12921111182616"></a><a name="p12921111182616"></a>枚举值：</p>
<a name="ul199212011192618"></a><a name="ul199212011192618"></a><ul id="ul199212011192618"><li><strong id="b792271132617"><a name="b792271132617"></a><a name="b792271132617"></a>ACTIVE</strong></li><li><strong id="b39231411102612"><a name="b39231411102612"></a><a name="b39231411102612"></a>PENDING_CREATE</strong></li><li><strong id="b169235110261"><a name="b169235110261"></a><a name="b169235110261"></a>PENDING_UPDATE</strong></li><li><strong id="b2092461116262"><a name="b2092461116262"></a><a name="b2092461116262"></a>PENDING_DELETE</strong></li><li><strong id="b1092441142610"><a name="b1092441142610"></a><a name="b1092441142610"></a>EIP_FREEZED</strong></li><li><strong id="b109241411172613"><a name="b109241411172613"></a><a name="b109241411172613"></a>INACTIVE</strong></li></ul>
</td>
</tr>
<tr id="row2894211172615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4925101111269"><a name="p4925101111269"></a><a name="p4925101111269"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p189262114267"><a name="p189262114267"></a><a name="p189262114267"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p0926141132616"><a name="p0926141132616"></a><a name="p0926141132616"></a>解冻/冻结状态。取值范围： − “true”： 解冻 − “false”： 冻结</p>
</td>
</tr>
<tr id="row188947112266"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p2927131113262"><a name="p2927131113262"></a><a name="p2927131113262"></a>internal_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p8927111112619"><a name="p8927111112619"></a><a name="p8927111112619"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1928141119267"><a name="p1928141119267"></a><a name="p1928141119267"></a>虚拟机或者裸机对外提供服务的协议端口号范围。功能说明：该端口范围与external _service_port_range按顺序实现1:1映射。取值范围：1~65535。约束：只能以’-’字符连接端口范围。</p>
</td>
</tr>
<tr id="row28941111102612"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1492871132619"><a name="p1492871132619"></a><a name="p1492871132619"></a>external_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p0314127269"><a name="p0314127269"></a><a name="p0314127269"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p143291218262"><a name="p143291218262"></a><a name="p143291218262"></a>Floatingip对外提供服务的端口号范围。功能说明：该端口范围与internal _service_port_range按顺序实现1:1映射。取值范围：1~65535。约束：只能以’-’字符连接端口范围</p>
</td>
</tr>
<tr id="row10894211162612"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p173271219265"><a name="p173271219265"></a><a name="p173271219265"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p183211252611"><a name="p183211252611"></a><a name="p183211252611"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1032161212616"><a name="p1032161212616"></a><a name="p1032161212616"></a>协议类型，目前支持TCP/tcp、UDP/udp、ANY/any。对应协议号6、17、0。</p>
<p id="p73211121268"><a name="p73211121268"></a><a name="p73211121268"></a>最小长度：<strong id="b732612192611"><a name="b732612192611"></a><a name="b732612192611"></a>1</strong></p>
<p id="p933161211264"><a name="p933161211264"></a><a name="p933161211264"></a>最大长度：<strong id="b16331412132619"><a name="b16331412132619"></a><a name="b16331412132619"></a>3</strong></p>
<p id="p03311212617"><a name="p03311212617"></a><a name="p03311212617"></a>枚举值：</p>
<a name="ul173381219267"></a><a name="ul173381219267"></a><ul id="ul173381219267"><li><strong id="b1333181218269"><a name="b1333181218269"></a><a name="b1333181218269"></a>tcp</strong></li><li><strong id="b1633112112611"><a name="b1633112112611"></a><a name="b1633112112611"></a>udp</strong></li><li><strong id="b193451215269"><a name="b193451215269"></a><a name="b193451215269"></a>any</strong></li></ul>
</td>
</tr>
<tr id="row089421118262"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p63451222620"><a name="p63451222620"></a><a name="p63451222620"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1234121218264"><a name="p1234121218264"></a><a name="p1234121218264"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p334121214261"><a name="p334121214261"></a><a name="p334121214261"></a>DNAT规则的创建时间，遵循UTC时间，格式是yyyy-mm-ddThh:mm:ssZ。</p>
<p id="p1334712192615"><a name="p1334712192615"></a><a name="p1334712192615"></a>最小长度：<strong id="b183471216269"><a name="b183471216269"></a><a name="b183471216269"></a>1</strong></p>
<p id="p634161272620"><a name="p634161272620"></a><a name="p634161272620"></a>最大长度：<strong id="b103421217266"><a name="b103421217266"></a><a name="b103421217266"></a>36</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section534612122612"></a>

```
GET https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526d/dnat_rules?limit=2

    
```

## 响应示例<a name="section1535131216265"></a>

**状态码： 200**

查询DNAT规则列表成功。

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
    "tenant_id" : "d199ba7e0ba64899b2e81518104b1526d",
    "created_at" : "2017-11-15 15:44:42.595173",
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
    "tenant_id" : "d199ba7e0ba64899b2e81518104b1526d",
    "created_at" : "2017-11-16 15:44:42.595173",
    "id" : "89195d50-0271-41f1-bded-4c089b2502ff",
    "floating_ip_address" : "5.21.11.227",
    "external_service_port" : 0,
    "description" : "my dnat rule 01"
  } ]
}
```

## 状态码<a name="section338141210269"></a>

<a name="zh-cn_topic_0297140328_status_code"></a>
<table><thead align="left"><tr id="row494571152611"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p5391012182620"><a name="p5391012182620"></a><a name="p5391012182620"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p33931216266"><a name="p33931216266"></a><a name="p33931216266"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row794531182614"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p639812102616"><a name="p639812102616"></a><a name="p639812102616"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p13394121268"><a name="p13394121268"></a><a name="p13394121268"></a>查询DNAT规则列表成功。</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section143911123262"></a>

请参见[错误码](错误码.md)。

