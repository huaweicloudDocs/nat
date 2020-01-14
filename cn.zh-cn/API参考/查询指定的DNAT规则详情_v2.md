# 查询指定的DNAT规则详情<a name="nat_apiv2_0020"></a>

## 功能介绍<a name="zh-cn_topic_0168797271_section242916116504"></a>

查询指定的DNAT规则详情。

## URI<a name="zh-cn_topic_0168797271_section55252672165026"></a>

GET /v2/\{project\_id\}/dnat\_rules/\{dnat\_rule\_id\}

**表 1**  参数说明

<a name="zh-cn_topic_0168797271_table41603310017"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797271_row323012314017"><th class="cellrowborder" valign="top" width="28.687131286871313%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797271_p1023043508"><a name="zh-cn_topic_0168797271_p1023043508"></a><a name="zh-cn_topic_0168797271_p1023043508"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="9.369063093690631%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797271_p52301036011"><a name="zh-cn_topic_0168797271_p52301036011"></a><a name="zh-cn_topic_0168797271_p52301036011"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.238176182381764%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797271_p1328082133316"><a name="zh-cn_topic_0168797271_p1328082133316"></a><a name="zh-cn_topic_0168797271_p1328082133316"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="43.705629437056295%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797271_p7230330014"><a name="zh-cn_topic_0168797271_p7230330014"></a><a name="zh-cn_topic_0168797271_p7230330014"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797271_row97760911571"><td class="cellrowborder" valign="top" width="28.687131286871313%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797271_p61255241574"><a name="zh-cn_topic_0168797271_p61255241574"></a><a name="zh-cn_topic_0168797271_p61255241574"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="9.369063093690631%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797271_p1712512485715"><a name="zh-cn_topic_0168797271_p1712512485715"></a><a name="zh-cn_topic_0168797271_p1712512485715"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.238176182381764%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797271_p6280182110334"><a name="zh-cn_topic_0168797271_p6280182110334"></a><a name="zh-cn_topic_0168797271_p6280182110334"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.705629437056295%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797271_p10125122455714"><a name="zh-cn_topic_0168797271_p10125122455714"></a><a name="zh-cn_topic_0168797271_p10125122455714"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797271_row9230031106"><td class="cellrowborder" valign="top" width="28.687131286871313%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797271_p1823033907"><a name="zh-cn_topic_0168797271_p1823033907"></a><a name="zh-cn_topic_0168797271_p1823033907"></a>dnat_rule_id</p>
</td>
<td class="cellrowborder" valign="top" width="9.369063093690631%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797271_p623013311018"><a name="zh-cn_topic_0168797271_p623013311018"></a><a name="zh-cn_topic_0168797271_p623013311018"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.238176182381764%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797271_p12445175215452"><a name="zh-cn_topic_0168797271_p12445175215452"></a><a name="zh-cn_topic_0168797271_p12445175215452"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.705629437056295%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797271_p5230735019"><a name="zh-cn_topic_0168797271_p5230735019"></a><a name="zh-cn_topic_0168797271_p5230735019"></a>DNAT规则的id。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0168797271_section30445355165052"></a>

无

## 响应消息<a name="zh-cn_topic_0168797271_section1412948816517"></a>

响应参数如[表2](#zh-cn_topic_0168797271_table66411570165117)所示。

**表 2**  响应参数

<a name="zh-cn_topic_0168797271_table66411570165117"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797271_row43436947165117"><th class="cellrowborder" valign="top" width="28.000000000000004%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797271_p28731843165117"><a name="zh-cn_topic_0168797271_p28731843165117"></a><a name="zh-cn_topic_0168797271_p28731843165117"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="22.2%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797271_p45577964165117"><a name="zh-cn_topic_0168797271_p45577964165117"></a><a name="zh-cn_topic_0168797271_p45577964165117"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="49.8%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797271_p67033414165117"><a name="zh-cn_topic_0168797271_p67033414165117"></a><a name="zh-cn_topic_0168797271_p67033414165117"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797271_row60997448165117"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797271_p41846242165117"><a name="zh-cn_topic_0168797271_p41846242165117"></a><a name="zh-cn_topic_0168797271_p41846242165117"></a>dnat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="22.2%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797271_p34102461165117"><a name="zh-cn_topic_0168797271_p34102461165117"></a><a name="zh-cn_topic_0168797271_p34102461165117"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="49.8%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797271_p5298260165117"><a name="zh-cn_topic_0168797271_p5298260165117"></a><a name="zh-cn_topic_0168797271_p5298260165117"></a>dnat_rule对象。请参考<a href="#zh-cn_topic_0168797271_table9899152414719">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  dnat\_rule字段说明

<a name="zh-cn_topic_0168797271_table9899152414719"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797271_row198997241973"><th class="cellrowborder" valign="top" width="28.072807280728075%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797271_p3368163219712"><a name="zh-cn_topic_0168797271_p3368163219712"></a><a name="zh-cn_topic_0168797271_p3368163219712"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.57205720572057%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797271_p23681832770"><a name="zh-cn_topic_0168797271_p23681832770"></a><a name="zh-cn_topic_0168797271_p23681832770"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.35513551355135%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797271_p23681432671"><a name="zh-cn_topic_0168797271_p23681432671"></a><a name="zh-cn_topic_0168797271_p23681432671"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797271_row88993241676"><td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797271_p1136816321074"><a name="zh-cn_topic_0168797271_p1136816321074"></a><a name="zh-cn_topic_0168797271_p1136816321074"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20.57205720572057%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797271_p1236803212715"><a name="zh-cn_topic_0168797271_p1236803212715"></a><a name="zh-cn_topic_0168797271_p1236803212715"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.35513551355135%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797271_p636818322071"><a name="zh-cn_topic_0168797271_p636818322071"></a><a name="zh-cn_topic_0168797271_p636818322071"></a>DNAT规则的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797271_row198999241712"><td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797271_p15368632273"><a name="zh-cn_topic_0168797271_p15368632273"></a><a name="zh-cn_topic_0168797271_p15368632273"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.57205720572057%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797271_p6368132672"><a name="zh-cn_topic_0168797271_p6368132672"></a><a name="zh-cn_topic_0168797271_p6368132672"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.35513551355135%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797271_p4368193211713"><a name="zh-cn_topic_0168797271_p4368193211713"></a><a name="zh-cn_topic_0168797271_p4368193211713"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797271_row18993246715"><td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797271_p10368143213712"><a name="zh-cn_topic_0168797271_p10368143213712"></a><a name="zh-cn_topic_0168797271_p10368143213712"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.57205720572057%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797271_p03681132579"><a name="zh-cn_topic_0168797271_p03681132579"></a><a name="zh-cn_topic_0168797271_p03681132579"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.35513551355135%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797271_p0368163220715"><a name="zh-cn_topic_0168797271_p0368163220715"></a><a name="zh-cn_topic_0168797271_p0368163220715"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797271_row1899924074"><td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797271_p0368183220715"><a name="zh-cn_topic_0168797271_p0368183220715"></a><a name="zh-cn_topic_0168797271_p0368183220715"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.57205720572057%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797271_p12368932672"><a name="zh-cn_topic_0168797271_p12368932672"></a><a name="zh-cn_topic_0168797271_p12368932672"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.35513551355135%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797271_p3368132676"><a name="zh-cn_topic_0168797271_p3368132676"></a><a name="zh-cn_topic_0168797271_p3368132676"></a>虚拟机或者裸机的Port ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797271_row38991524672"><td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797271_p836823213715"><a name="zh-cn_topic_0168797271_p836823213715"></a><a name="zh-cn_topic_0168797271_p836823213715"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="20.57205720572057%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797271_p1636843210716"><a name="zh-cn_topic_0168797271_p1636843210716"></a><a name="zh-cn_topic_0168797271_p1636843210716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.35513551355135%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797271_p2036803210718"><a name="zh-cn_topic_0168797271_p2036803210718"></a><a name="zh-cn_topic_0168797271_p2036803210718"></a>用户私有IP地址，例如专线连接的私有云地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797271_row48998241373"><td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797271_p936811322076"><a name="zh-cn_topic_0168797271_p936811322076"></a><a name="zh-cn_topic_0168797271_p936811322076"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="20.57205720572057%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797271_p6368153211712"><a name="zh-cn_topic_0168797271_p6368153211712"></a><a name="zh-cn_topic_0168797271_p6368153211712"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="51.35513551355135%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797271_p15368123218715"><a name="zh-cn_topic_0168797271_p15368123218715"></a><a name="zh-cn_topic_0168797271_p15368123218715"></a>虚拟机或者裸机对外提供服务的协议端口号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797271_row1789914241878"><td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797271_p43681532970"><a name="zh-cn_topic_0168797271_p43681532970"></a><a name="zh-cn_topic_0168797271_p43681532970"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.57205720572057%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797271_p123684326717"><a name="zh-cn_topic_0168797271_p123684326717"></a><a name="zh-cn_topic_0168797271_p123684326717"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.35513551355135%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797271_p93683323710"><a name="zh-cn_topic_0168797271_p93683323710"></a><a name="zh-cn_topic_0168797271_p93683323710"></a>弹性公网IP的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797271_row7899102413716"><td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797271_p1336843213714"><a name="zh-cn_topic_0168797271_p1336843213714"></a><a name="zh-cn_topic_0168797271_p1336843213714"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="20.57205720572057%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797271_p536820321572"><a name="zh-cn_topic_0168797271_p536820321572"></a><a name="zh-cn_topic_0168797271_p536820321572"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.35513551355135%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797271_p193681532072"><a name="zh-cn_topic_0168797271_p193681532072"></a><a name="zh-cn_topic_0168797271_p193681532072"></a>弹性公网的IP地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797271_row889916241373"><td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797271_p73686321175"><a name="zh-cn_topic_0168797271_p73686321175"></a><a name="zh-cn_topic_0168797271_p73686321175"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="20.57205720572057%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797271_p1836813210719"><a name="zh-cn_topic_0168797271_p1836813210719"></a><a name="zh-cn_topic_0168797271_p1836813210719"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="51.35513551355135%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797271_p73683325711"><a name="zh-cn_topic_0168797271_p73683325711"></a><a name="zh-cn_topic_0168797271_p73683325711"></a>Floatingip对外提供服务的端口号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797271_row489932414710"><td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797271_p17368232474"><a name="zh-cn_topic_0168797271_p17368232474"></a><a name="zh-cn_topic_0168797271_p17368232474"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20.57205720572057%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797271_p163683321719"><a name="zh-cn_topic_0168797271_p163683321719"></a><a name="zh-cn_topic_0168797271_p163683321719"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.35513551355135%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797271_p336893219716"><a name="zh-cn_topic_0168797271_p336893219716"></a><a name="zh-cn_topic_0168797271_p336893219716"></a>协议类型，目前支持TCP、UDP、ANY。</p>
<p id="zh-cn_topic_0168797271_p9368432271"><a name="zh-cn_topic_0168797271_p9368432271"></a><a name="zh-cn_topic_0168797271_p9368432271"></a>对应协议号6、17、0。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797271_row1489917241174"><td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797271_p1936814325712"><a name="zh-cn_topic_0168797271_p1936814325712"></a><a name="zh-cn_topic_0168797271_p1936814325712"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20.57205720572057%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797271_p133681232279"><a name="zh-cn_topic_0168797271_p133681232279"></a><a name="zh-cn_topic_0168797271_p133681232279"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="51.35513551355135%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797271_p1536816321716"><a name="zh-cn_topic_0168797271_p1536816321716"></a><a name="zh-cn_topic_0168797271_p1536816321716"></a>DNAT规则的描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797271_row389917241879"><td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797271_p1736833215711"><a name="zh-cn_topic_0168797271_p1736833215711"></a><a name="zh-cn_topic_0168797271_p1736833215711"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20.57205720572057%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797271_p736853214714"><a name="zh-cn_topic_0168797271_p736853214714"></a><a name="zh-cn_topic_0168797271_p736853214714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.35513551355135%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797271_ul113681321476"></a><a name="zh-cn_topic_0168797271_ul113681321476"></a><ul id="zh-cn_topic_0168797271_ul113681321476"><li>功能说明：DNAT规则的状态。</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797271_row1589910244715"><td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797271_p1836883218715"><a name="zh-cn_topic_0168797271_p1836883218715"></a><a name="zh-cn_topic_0168797271_p1836883218715"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="20.57205720572057%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797271_p1501189281"><a name="zh-cn_topic_0168797271_p1501189281"></a><a name="zh-cn_topic_0168797271_p1501189281"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="51.35513551355135%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797271_ul71858556358"></a><a name="zh-cn_topic_0168797271_ul71858556358"></a><ul id="zh-cn_topic_0168797271_ul71858556358"><li>解冻/冻结状态。</li><li>取值范围：<a name="zh-cn_topic_0168797271_ul11838172814409"></a><a name="zh-cn_topic_0168797271_ul11838172814409"></a><ul id="zh-cn_topic_0168797271_ul11838172814409"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797271_row28997241277"><td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797271_p13368332977"><a name="zh-cn_topic_0168797271_p13368332977"></a><a name="zh-cn_topic_0168797271_p13368332977"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="20.57205720572057%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797271_p136853217716"><a name="zh-cn_topic_0168797271_p136853217716"></a><a name="zh-cn_topic_0168797271_p136853217716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.35513551355135%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797271_ul2036815321717"></a><a name="zh-cn_topic_0168797271_ul2036815321717"></a><ul id="zh-cn_topic_0168797271_ul2036815321717"><li>DNAT规则的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797271_row1945175314583"><td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797271_p111699547583"><a name="zh-cn_topic_0168797271_p111699547583"></a><a name="zh-cn_topic_0168797271_p111699547583"></a>internal_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="20.57205720572057%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797271_p516912543588"><a name="zh-cn_topic_0168797271_p516912543588"></a><a name="zh-cn_topic_0168797271_p516912543588"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.35513551355135%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797271_p2169115415815"><a name="zh-cn_topic_0168797271_p2169115415815"></a><a name="zh-cn_topic_0168797271_p2169115415815"></a>虚拟机或者裸机对外提供服务的协议端口号范围。</p>
<a name="zh-cn_topic_0168797271_ul1416965445810"></a><a name="zh-cn_topic_0168797271_ul1416965445810"></a><ul id="zh-cn_topic_0168797271_ul1416965445810"><li>功能说明：该端口范围与external _service_port_range按顺序实现1:1映射。</li><li>取值范围：1~65535。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797271_row104535385813"><td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797271_p17170135465812"><a name="zh-cn_topic_0168797271_p17170135465812"></a><a name="zh-cn_topic_0168797271_p17170135465812"></a>external_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="20.57205720572057%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797271_p18170654195811"><a name="zh-cn_topic_0168797271_p18170654195811"></a><a name="zh-cn_topic_0168797271_p18170654195811"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.35513551355135%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797271_p61706549584"><a name="zh-cn_topic_0168797271_p61706549584"></a><a name="zh-cn_topic_0168797271_p61706549584"></a>Floatingip对外提供服务的端口号范围。</p>
<a name="zh-cn_topic_0168797271_ul121701154175811"></a><a name="zh-cn_topic_0168797271_ul121701154175811"></a><ul id="zh-cn_topic_0168797271_ul121701154175811"><li>功能说明：该端口范围与internal _service_port_range按顺序实现1:1映射。</li><li>取值范围：1~65535。</li></ul>
</td>
</tr>
</tbody>
</table>

## 示例<a name="zh-cn_topic_0168797271_section24779297165121"></a>

-   请求样例

    ```
    GET https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526d/dnat_rules/5b95c675-69c2-4656-ba06-58ff72e1d338
    ```


-   响应样例

    ```
    {               
    　　　"dnat_rules": { 
    　　　　　　"floating_ip_id": "bf99c679-9f41-4dac-8513-9c9228e713e1", 
    　　　　　　"status": "ACTIVE", 
    　　　　　　"nat_gateway_id": "cda3a125-2406-456c-a11f-598e10578541",　
    　　　　　　"admin_state_up": true, 
    　　　　　　"port_id": "9a469561-daac-4c94-88f5-39366e5ea193", 
    　　　　　　"private_ip": "", 
    　　　　　　"internal_service_port": 993, 
    　　　　　　"protocol": "tcp", 
    　　　　　　"tenant_id": "d199ba7e0ba64899b2e81518104b1526d", 
    　　　　　　"created_at": "2017-11-15 15:44:42.595173", 
    　　　　　　"id": "5b95c675-69c2-4656-ba06-58ff72e1d338", 
    　　　　　　"floating_ip_address": "5.21.11.226", 
    　　　　　　"external_service_port": 242, 
    　　　　　　"description": "my dnat rule 01" 
       　 } 
     }
    ```


## 状态码<a name="zh-cn_topic_0168797271_section16249219165526"></a>

请参考[状态码](状态码.md)。

