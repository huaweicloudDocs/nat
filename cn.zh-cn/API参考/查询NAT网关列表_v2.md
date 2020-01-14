# 查询NAT网关列表<a name="nat_apiv2_0006"></a>

## 功能介绍<a name="zh-cn_topic_0168797269_section21650537"></a>

查询NAT网关列表。如无特殊说明，匹配规则为精确匹配。

## URI<a name="zh-cn_topic_0168797269_section60637113"></a>

GET /v2/\{project\_id\}/nat\_gateways

>![](public_sys-resources/icon-note.gif) **说明：**   
>可以在URI后面用‘?’和‘&’添加不同的查询条件组合。支持参数说明中所有非必选参数过滤，请参考请求样例。  

**表 1**  参数说明

<a name="zh-cn_topic_0168797269_table18558131224111"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797269_row1808612184118"><th class="cellrowborder" valign="top" width="21.35213521352135%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797269_p780881214411"><a name="zh-cn_topic_0168797269_p780881214411"></a><a name="zh-cn_topic_0168797269_p780881214411"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.08080808080808%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797269_p201221240122514"><a name="zh-cn_topic_0168797269_p201221240122514"></a><a name="zh-cn_topic_0168797269_p201221240122514"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.711671167116712%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797269_p380881220414"><a name="zh-cn_topic_0168797269_p380881220414"></a><a name="zh-cn_topic_0168797269_p380881220414"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="53.855385538553854%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797269_p1880841274119"><a name="zh-cn_topic_0168797269_p1880841274119"></a><a name="zh-cn_topic_0168797269_p1880841274119"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797269_row2505168143116"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797269_p665515149312"><a name="zh-cn_topic_0168797269_p665515149312"></a><a name="zh-cn_topic_0168797269_p665515149312"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797269_p7122114022511"><a name="zh-cn_topic_0168797269_p7122114022511"></a><a name="zh-cn_topic_0168797269_p7122114022511"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797269_p76551414173114"><a name="zh-cn_topic_0168797269_p76551414173114"></a><a name="zh-cn_topic_0168797269_p76551414173114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797269_p1665541413318"><a name="zh-cn_topic_0168797269_p1665541413318"></a><a name="zh-cn_topic_0168797269_p1665541413318"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row5186181911174"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797269_p1383522411718"><a name="zh-cn_topic_0168797269_p1383522411718"></a><a name="zh-cn_topic_0168797269_p1383522411718"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797269_p1512224014255"><a name="zh-cn_topic_0168797269_p1512224014255"></a><a name="zh-cn_topic_0168797269_p1512224014255"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797269_p7836142471712"><a name="zh-cn_topic_0168797269_p7836142471712"></a><a name="zh-cn_topic_0168797269_p7836142471712"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797269_p11836102411710"><a name="zh-cn_topic_0168797269_p11836102411710"></a><a name="zh-cn_topic_0168797269_p11836102411710"></a>每页返回的个数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row28088123418"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797269_p480891218412"><a name="zh-cn_topic_0168797269_p480891218412"></a><a name="zh-cn_topic_0168797269_p480891218412"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797269_p712312405258"><a name="zh-cn_topic_0168797269_p712312405258"></a><a name="zh-cn_topic_0168797269_p712312405258"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797269_p0808181217416"><a name="zh-cn_topic_0168797269_p0808181217416"></a><a name="zh-cn_topic_0168797269_p0808181217416"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797269_p7808141219418"><a name="zh-cn_topic_0168797269_p7808141219418"></a><a name="zh-cn_topic_0168797269_p7808141219418"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row080891254119"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797269_p1880851212411"><a name="zh-cn_topic_0168797269_p1880851212411"></a><a name="zh-cn_topic_0168797269_p1880851212411"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797269_p212314092510"><a name="zh-cn_topic_0168797269_p212314092510"></a><a name="zh-cn_topic_0168797269_p212314092510"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797269_p198084127419"><a name="zh-cn_topic_0168797269_p198084127419"></a><a name="zh-cn_topic_0168797269_p198084127419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797269_p1080810121412"><a name="zh-cn_topic_0168797269_p1080810121412"></a><a name="zh-cn_topic_0168797269_p1080810121412"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row11808111284110"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797269_p1808191244110"><a name="zh-cn_topic_0168797269_p1808191244110"></a><a name="zh-cn_topic_0168797269_p1808191244110"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797269_p8123104015254"><a name="zh-cn_topic_0168797269_p8123104015254"></a><a name="zh-cn_topic_0168797269_p8123104015254"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797269_p2080861264119"><a name="zh-cn_topic_0168797269_p2080861264119"></a><a name="zh-cn_topic_0168797269_p2080861264119"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797269_p2808112174112"><a name="zh-cn_topic_0168797269_p2808112174112"></a><a name="zh-cn_topic_0168797269_p2808112174112"></a>NAT网关的名字。</p>
<p id="zh-cn_topic_0168797269_p138082126416"><a name="zh-cn_topic_0168797269_p138082126416"></a><a name="zh-cn_topic_0168797269_p138082126416"></a>NAT网关的名字仅支持数字、字母、_（下划线）、-（中划线）、中文。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row6808712144114"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797269_p08087126419"><a name="zh-cn_topic_0168797269_p08087126419"></a><a name="zh-cn_topic_0168797269_p08087126419"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797269_p2123114017259"><a name="zh-cn_topic_0168797269_p2123114017259"></a><a name="zh-cn_topic_0168797269_p2123114017259"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797269_p180811212410"><a name="zh-cn_topic_0168797269_p180811212410"></a><a name="zh-cn_topic_0168797269_p180811212410"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797269_p780817129410"><a name="zh-cn_topic_0168797269_p780817129410"></a><a name="zh-cn_topic_0168797269_p780817129410"></a>NAT网关的描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row16808171215417"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797269_p118081612194112"><a name="zh-cn_topic_0168797269_p118081612194112"></a><a name="zh-cn_topic_0168797269_p118081612194112"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797269_p131231940132515"><a name="zh-cn_topic_0168797269_p131231940132515"></a><a name="zh-cn_topic_0168797269_p131231940132515"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797269_p2080820126416"><a name="zh-cn_topic_0168797269_p2080820126416"></a><a name="zh-cn_topic_0168797269_p2080820126416"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797269_p198081612114114"><a name="zh-cn_topic_0168797269_p198081612114114"></a><a name="zh-cn_topic_0168797269_p198081612114114"></a>NAT网关的规格。</p>
<p id="zh-cn_topic_0168797269_p138081012184115"><a name="zh-cn_topic_0168797269_p138081012184115"></a><a name="zh-cn_topic_0168797269_p138081012184115"></a>取值为：</p>
<a name="zh-cn_topic_0168797269_ul108080122414"></a><a name="zh-cn_topic_0168797269_ul108080122414"></a><ul id="zh-cn_topic_0168797269_ul108080122414"><li>“1”：小型，SNAT最大连接数10000</li><li>“2”：中型，SNAT最大连接数50000</li><li>“3”：大型，SNAT最大连接数200000</li><li>“4”：超大型，SNAT最大连接数1000000</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row178085121417"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797269_p7808181224114"><a name="zh-cn_topic_0168797269_p7808181224114"></a><a name="zh-cn_topic_0168797269_p7808181224114"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797269_p1312314082511"><a name="zh-cn_topic_0168797269_p1312314082511"></a><a name="zh-cn_topic_0168797269_p1312314082511"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797269_p12808121264118"><a name="zh-cn_topic_0168797269_p12808121264118"></a><a name="zh-cn_topic_0168797269_p12808121264118"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797269_p108081912194120"><a name="zh-cn_topic_0168797269_p108081912194120"></a><a name="zh-cn_topic_0168797269_p108081912194120"></a>路由器的UUID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row18808151274111"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797269_p5808141224118"><a name="zh-cn_topic_0168797269_p5808141224118"></a><a name="zh-cn_topic_0168797269_p5808141224118"></a>internal_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797269_p17123174011251"><a name="zh-cn_topic_0168797269_p17123174011251"></a><a name="zh-cn_topic_0168797269_p17123174011251"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797269_p10808212124113"><a name="zh-cn_topic_0168797269_p10808212124113"></a><a name="zh-cn_topic_0168797269_p10808212124113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797269_p4808171224115"><a name="zh-cn_topic_0168797269_p4808171224115"></a><a name="zh-cn_topic_0168797269_p4808171224115"></a>NAT网关下行口（DVR的下一跳）所属的network id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row16808412104117"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797269_p1380821214116"><a name="zh-cn_topic_0168797269_p1380821214116"></a><a name="zh-cn_topic_0168797269_p1380821214116"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797269_p19123104052517"><a name="zh-cn_topic_0168797269_p19123104052517"></a><a name="zh-cn_topic_0168797269_p19123104052517"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797269_p6808181284110"><a name="zh-cn_topic_0168797269_p6808181284110"></a><a name="zh-cn_topic_0168797269_p6808181284110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0168797269_ul68084129415"></a><a name="zh-cn_topic_0168797269_ul68084129415"></a><ul id="zh-cn_topic_0168797269_ul68084129415"><li>功能说明：NAT网关的状态。</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row18808141244119"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797269_p1780816122417"><a name="zh-cn_topic_0168797269_p1780816122417"></a><a name="zh-cn_topic_0168797269_p1780816122417"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797269_p15123174010257"><a name="zh-cn_topic_0168797269_p15123174010257"></a><a name="zh-cn_topic_0168797269_p15123174010257"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797269_p136891348122217"><a name="zh-cn_topic_0168797269_p136891348122217"></a><a name="zh-cn_topic_0168797269_p136891348122217"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0168797269_ul71858556358"></a><a name="zh-cn_topic_0168797269_ul71858556358"></a><ul id="zh-cn_topic_0168797269_ul71858556358"><li>解冻/冻结状态。</li><li>取值范围：<a name="zh-cn_topic_0168797269_ul11838172814409"></a><a name="zh-cn_topic_0168797269_ul11838172814409"></a><ul id="zh-cn_topic_0168797269_ul11838172814409"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row138088125411"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797269_p1680831254112"><a name="zh-cn_topic_0168797269_p1680831254112"></a><a name="zh-cn_topic_0168797269_p1680831254112"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797269_p91239405258"><a name="zh-cn_topic_0168797269_p91239405258"></a><a name="zh-cn_topic_0168797269_p91239405258"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797269_p1180818124411"><a name="zh-cn_topic_0168797269_p1180818124411"></a><a name="zh-cn_topic_0168797269_p1180818124411"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0168797269_ul88088126418"></a><a name="zh-cn_topic_0168797269_ul88088126418"></a><ul id="zh-cn_topic_0168797269_ul88088126418"><li>NAT网关的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row13871123337"><td class="cellrowborder" valign="top" width="21.35213521352135%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797269_p16762910173316"><a name="zh-cn_topic_0168797269_p16762910173316"></a><a name="zh-cn_topic_0168797269_p16762910173316"></a>enterprise_project_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08080808080808%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797269_p012315404251"><a name="zh-cn_topic_0168797269_p012315404251"></a><a name="zh-cn_topic_0168797269_p012315404251"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.711671167116712%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797269_p176291015339"><a name="zh-cn_topic_0168797269_p176291015339"></a><a name="zh-cn_topic_0168797269_p176291015339"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.855385538553854%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0168797269_ul188298501193"></a><a name="zh-cn_topic_0168797269_ul188298501193"></a><ul id="zh-cn_topic_0168797269_ul188298501193"><li>功能说明：企业项目ID。默认值：0，表示默认企业项目。</li><li>取值范围：最大长度36字节，带 “-”连字符的UUID格式，或者是字符串“0”。</li><li>说明：关于企业项目ID的获取及企业项目特性的详细信息，请参考<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0123692049.html" target="_blank" rel="noopener noreferrer">《企业管理用户指南》</a>。</li></ul>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0168797269_section12659140"></a>

无

## 响应消息<a name="zh-cn_topic_0168797269_section46823401"></a>

响应参数如[表2](#zh-cn_topic_0168797269_table8843312114313)所示。

**表 2**  响应参数

<a name="zh-cn_topic_0168797269_table8843312114313"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797269_row10874912134313"><th class="cellrowborder" valign="top" width="20.200000000000003%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797269_p1887410126437"><a name="zh-cn_topic_0168797269_p1887410126437"></a><a name="zh-cn_topic_0168797269_p1887410126437"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="21.62%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797269_p188749126436"><a name="zh-cn_topic_0168797269_p188749126436"></a><a name="zh-cn_topic_0168797269_p188749126436"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.18%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797269_p14874111234319"><a name="zh-cn_topic_0168797269_p14874111234319"></a><a name="zh-cn_topic_0168797269_p14874111234319"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797269_row1787461216433"><td class="cellrowborder" valign="top" width="20.200000000000003%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797269_p48741812124312"><a name="zh-cn_topic_0168797269_p48741812124312"></a><a name="zh-cn_topic_0168797269_p48741812124312"></a>nat_gateways</p>
</td>
<td class="cellrowborder" valign="top" width="21.62%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797269_p14874512194313"><a name="zh-cn_topic_0168797269_p14874512194313"></a><a name="zh-cn_topic_0168797269_p14874512194313"></a>Array(Object)</p>
</td>
<td class="cellrowborder" valign="top" width="58.18%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797269_p129411120422"><a name="zh-cn_topic_0168797269_p129411120422"></a><a name="zh-cn_topic_0168797269_p129411120422"></a>nat_gateway对象列表。请参考<a href="#zh-cn_topic_0168797269_table1810691174217">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  nat\_gateway字段说明

<a name="zh-cn_topic_0168797269_table1810691174217"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797269_row15294131114425"><th class="cellrowborder" valign="top" width="20.23%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797269_p029451114211"><a name="zh-cn_topic_0168797269_p029451114211"></a><a name="zh-cn_topic_0168797269_p029451114211"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="21.18%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797269_p18294511134216"><a name="zh-cn_topic_0168797269_p18294511134216"></a><a name="zh-cn_topic_0168797269_p18294511134216"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.589999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797269_p102941011144211"><a name="zh-cn_topic_0168797269_p102941011144211"></a><a name="zh-cn_topic_0168797269_p102941011144211"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797269_row929451134215"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797269_p102941911114216"><a name="zh-cn_topic_0168797269_p102941911114216"></a><a name="zh-cn_topic_0168797269_p102941911114216"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797269_p629481118424"><a name="zh-cn_topic_0168797269_p629481118424"></a><a name="zh-cn_topic_0168797269_p629481118424"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797269_p1429411117423"><a name="zh-cn_topic_0168797269_p1429411117423"></a><a name="zh-cn_topic_0168797269_p1429411117423"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row1329471104211"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797269_p82941511164216"><a name="zh-cn_topic_0168797269_p82941511164216"></a><a name="zh-cn_topic_0168797269_p82941511164216"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797269_p17294011144211"><a name="zh-cn_topic_0168797269_p17294011144211"></a><a name="zh-cn_topic_0168797269_p17294011144211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797269_p19294181174214"><a name="zh-cn_topic_0168797269_p19294181174214"></a><a name="zh-cn_topic_0168797269_p19294181174214"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row8294151112421"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797269_p629441174214"><a name="zh-cn_topic_0168797269_p629441174214"></a><a name="zh-cn_topic_0168797269_p629441174214"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797269_p12294161110426"><a name="zh-cn_topic_0168797269_p12294161110426"></a><a name="zh-cn_topic_0168797269_p12294161110426"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797269_p1329414115428"><a name="zh-cn_topic_0168797269_p1329414115428"></a><a name="zh-cn_topic_0168797269_p1329414115428"></a>NAT网关的名字。</p>
<p id="zh-cn_topic_0168797269_p529420111420"><a name="zh-cn_topic_0168797269_p529420111420"></a><a name="zh-cn_topic_0168797269_p529420111420"></a>NAT网关的名字仅支持数字、字母、_（下划线）、-（中划线）、中文。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row229451119425"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797269_p17294411174218"><a name="zh-cn_topic_0168797269_p17294411174218"></a><a name="zh-cn_topic_0168797269_p17294411174218"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797269_p1629412114426"><a name="zh-cn_topic_0168797269_p1629412114426"></a><a name="zh-cn_topic_0168797269_p1629412114426"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797269_p142947116421"><a name="zh-cn_topic_0168797269_p142947116421"></a><a name="zh-cn_topic_0168797269_p142947116421"></a>NAT网关的描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row1829421134210"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797269_p13294121194215"><a name="zh-cn_topic_0168797269_p13294121194215"></a><a name="zh-cn_topic_0168797269_p13294121194215"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797269_p1629411118423"><a name="zh-cn_topic_0168797269_p1629411118423"></a><a name="zh-cn_topic_0168797269_p1629411118423"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797269_p1329410119429"><a name="zh-cn_topic_0168797269_p1329410119429"></a><a name="zh-cn_topic_0168797269_p1329410119429"></a>NAT网关的规格。</p>
<p id="zh-cn_topic_0168797269_p1429413113429"><a name="zh-cn_topic_0168797269_p1429413113429"></a><a name="zh-cn_topic_0168797269_p1429413113429"></a>取值为：</p>
<a name="zh-cn_topic_0168797269_ul3294191111427"></a><a name="zh-cn_topic_0168797269_ul3294191111427"></a><ul id="zh-cn_topic_0168797269_ul3294191111427"><li>“1”：小型，SNAT最大连接数10000</li><li>“2”：中型，SNAT最大连接数50000</li><li>“3”：大型，SNAT最大连接数200000</li><li>“4”：超大型，SNAT最大连接数1000000</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row1329416115424"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797269_p629416117428"><a name="zh-cn_topic_0168797269_p629416117428"></a><a name="zh-cn_topic_0168797269_p629416117428"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797269_p329418118427"><a name="zh-cn_topic_0168797269_p329418118427"></a><a name="zh-cn_topic_0168797269_p329418118427"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797269_p429410118427"><a name="zh-cn_topic_0168797269_p429410118427"></a><a name="zh-cn_topic_0168797269_p429410118427"></a>路由器的UUID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row9294151184215"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797269_p4294151104220"><a name="zh-cn_topic_0168797269_p4294151104220"></a><a name="zh-cn_topic_0168797269_p4294151104220"></a>internal_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797269_p6294121115424"><a name="zh-cn_topic_0168797269_p6294121115424"></a><a name="zh-cn_topic_0168797269_p6294121115424"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797269_p52948115428"><a name="zh-cn_topic_0168797269_p52948115428"></a><a name="zh-cn_topic_0168797269_p52948115428"></a>NAT网关下行口（DVR的下一跳）所属的network id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row182946117421"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797269_p172941011194220"><a name="zh-cn_topic_0168797269_p172941011194220"></a><a name="zh-cn_topic_0168797269_p172941011194220"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797269_p172942119421"><a name="zh-cn_topic_0168797269_p172942119421"></a><a name="zh-cn_topic_0168797269_p172942119421"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797269_ul8294181134219"></a><a name="zh-cn_topic_0168797269_ul8294181134219"></a><ul id="zh-cn_topic_0168797269_ul8294181134219"><li>功能说明：NAT网关的状态。</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row1629421184215"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797269_p2294171112421"><a name="zh-cn_topic_0168797269_p2294171112421"></a><a name="zh-cn_topic_0168797269_p2294171112421"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797269_p1929413118426"><a name="zh-cn_topic_0168797269_p1929413118426"></a><a name="zh-cn_topic_0168797269_p1929413118426"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797269_ul548018112009"></a><a name="zh-cn_topic_0168797269_ul548018112009"></a><ul id="zh-cn_topic_0168797269_ul548018112009"><li>解冻/冻结状态。</li><li>取值范围：<a name="zh-cn_topic_0168797269_ul048131119013"></a><a name="zh-cn_topic_0168797269_ul048131119013"></a><ul id="zh-cn_topic_0168797269_ul048131119013"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row19294121144218"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797269_p1529417112428"><a name="zh-cn_topic_0168797269_p1529417112428"></a><a name="zh-cn_topic_0168797269_p1529417112428"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797269_p0294151110422"><a name="zh-cn_topic_0168797269_p0294151110422"></a><a name="zh-cn_topic_0168797269_p0294151110422"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797269_p38576211214"><a name="zh-cn_topic_0168797269_p38576211214"></a><a name="zh-cn_topic_0168797269_p38576211214"></a>创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row152941111124212"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797269_p12294151110427"><a name="zh-cn_topic_0168797269_p12294151110427"></a><a name="zh-cn_topic_0168797269_p12294151110427"></a>dnat_rules_limit</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797269_p929491194218"><a name="zh-cn_topic_0168797269_p929491194218"></a><a name="zh-cn_topic_0168797269_p929491194218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797269_p16819115720205"><a name="zh-cn_topic_0168797269_p16819115720205"></a><a name="zh-cn_topic_0168797269_p16819115720205"></a>NAT网关的DNAT规则最多条数限制值</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row1629471104219"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797269_p529411184216"><a name="zh-cn_topic_0168797269_p529411184216"></a><a name="zh-cn_topic_0168797269_p529411184216"></a>snat_rule_public_ip_limit</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797269_p32942011124216"><a name="zh-cn_topic_0168797269_p32942011124216"></a><a name="zh-cn_topic_0168797269_p32942011124216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797269_p060155972015"><a name="zh-cn_topic_0168797269_p060155972015"></a><a name="zh-cn_topic_0168797269_p060155972015"></a>NAT网关的任意一条SNAT规则最多绑定的弹性公网IP的数量最大限制值。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row1177072318377"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797269_p63522326376"><a name="zh-cn_topic_0168797269_p63522326376"></a><a name="zh-cn_topic_0168797269_p63522326376"></a>billing_info</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797269_p14352203233711"><a name="zh-cn_topic_0168797269_p14352203233711"></a><a name="zh-cn_topic_0168797269_p14352203233711"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797269_p10491654182013"><a name="zh-cn_topic_0168797269_p10491654182013"></a><a name="zh-cn_topic_0168797269_p10491654182013"></a>包周期NAT网关订单关联信息，按需值为空字符串。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797269_row1677011095116"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797269_p123591695118"><a name="zh-cn_topic_0168797269_p123591695118"></a><a name="zh-cn_topic_0168797269_p123591695118"></a>enterprise_project_id</p>
</td>
<td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797269_p4235101685117"><a name="zh-cn_topic_0168797269_p4235101685117"></a><a name="zh-cn_topic_0168797269_p4235101685117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797269_ul12351016175112"></a><a name="zh-cn_topic_0168797269_ul12351016175112"></a><ul id="zh-cn_topic_0168797269_ul12351016175112"><li>功能说明：企业项目ID。默认值：0，表示默认企业项目。</li><li>取值范围：最大长度36字节，带 “-”连字符的UUID格式，或者是字符串“0”。</li><li>说明：关于企业项目ID的获取及企业项目特性的详细信息，请参考<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0123692049.html" target="_blank" rel="noopener noreferrer">《企业管理用户指南》</a>。</li></ul>
</td>
</tr>
</tbody>
</table>

## 示例<a name="zh-cn_topic_0168797269_section18757432"></a>

-   请求样例

    ```
    GET https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/nat_gateways?status=ACTIVE
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
                "name": "wj3",
                "dnat_rules_limit": "200",
                "snat_rule_public_ip_limit": "20",
                "enterprise_project_id=0aad99bc-f5f6-4f78-8404-c598d76b0ed2",
                "billing_info": ""
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
                "name": "lyl001",
                "dnat_rules_limit": "200",
                "snat_rule_public_ip_limit": "20",
                "enterprise_project_id=0aad99bc-f5f6-4f78-8404-c598d76b0ed2",
                "billing_info": ""
            } 
        ] 
    }
    ```


## 状态码<a name="zh-cn_topic_0168797269_section42956987"></a>

请参考[状态码](状态码.md)。

