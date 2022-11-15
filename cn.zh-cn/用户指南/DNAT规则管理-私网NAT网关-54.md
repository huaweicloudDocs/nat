# 支持的监控指标<a name="nat_ces_0002"></a>

## 功能说明<a name="zh-cn_topic_0201532915_section352319314226"></a>

本节定义了NAT网关上报云监控的监控指标的命名空间，监控指标列表和维度定义，用户可以通过云监控提供的管理控制台或API接口来检索NAT网关产生的监控指标。

## 命名空间<a name="zh-cn_topic_0201532915_section48641254172217"></a>

SYS.NAT

## 监控指标<a name="zh-cn_topic_0201532915_section1954874112249"></a>

**表 1** 公网NAT网关支持的监控指标

<a name="zh-cn_topic_0201532915_table6740854112515"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201532915_row663435514257"><th class="cellrowborder" valign="top" width="18.4%" id="mcps1.2.7.1.1"><p id="zh-cn_topic_0201532915_p863413556254"><a name="zh-cn_topic_0201532915_p863413556254"></a><a name="zh-cn_topic_0201532915_p863413556254"></a><strong id="zh-cn_topic_0201532915_b166621242151617"><a name="zh-cn_topic_0201532915_b166621242151617"></a><a name="zh-cn_topic_0201532915_b166621242151617"></a>指标ID</strong></p>
</th>
<th class="cellrowborder" valign="top" width="11.59%" id="mcps1.2.7.1.2"><p id="zh-cn_topic_0201532915_p56349551253"><a name="zh-cn_topic_0201532915_p56349551253"></a><a name="zh-cn_topic_0201532915_p56349551253"></a><strong id="zh-cn_topic_0201532915_b06647421164"><a name="zh-cn_topic_0201532915_b06647421164"></a><a name="zh-cn_topic_0201532915_b06647421164"></a>指标名称</strong></p>
</th>
<th class="cellrowborder" valign="top" width="28.77%" id="mcps1.2.7.1.3"><p id="zh-cn_topic_0201532915_p663485512519"><a name="zh-cn_topic_0201532915_p663485512519"></a><a name="zh-cn_topic_0201532915_p663485512519"></a><strong id="zh-cn_topic_0201532915_b166668423168"><a name="zh-cn_topic_0201532915_b166668423168"></a><a name="zh-cn_topic_0201532915_b166668423168"></a>指标含义</strong></p>
</th>
<th class="cellrowborder" valign="top" width="9.44%" id="mcps1.2.7.1.4"><p id="zh-cn_topic_0201532915_p16634165514250"><a name="zh-cn_topic_0201532915_p16634165514250"></a><a name="zh-cn_topic_0201532915_p16634165514250"></a><strong id="zh-cn_topic_0201532915_b176671642131618"><a name="zh-cn_topic_0201532915_b176671642131618"></a><a name="zh-cn_topic_0201532915_b176671642131618"></a>取值范围</strong></p>
</th>
<th class="cellrowborder" valign="top" width="16.77%" id="mcps1.2.7.1.5"><p id="zh-cn_topic_0201532915_p8634185517258"><a name="zh-cn_topic_0201532915_p8634185517258"></a><a name="zh-cn_topic_0201532915_p8634185517258"></a><strong id="zh-cn_topic_0201532915_b06691042111617"><a name="zh-cn_topic_0201532915_b06691042111617"></a><a name="zh-cn_topic_0201532915_b06691042111617"></a>测量对象</strong></p>
</th>
<th class="cellrowborder" valign="top" width="15.03%" id="mcps1.2.7.1.6"><p id="zh-cn_topic_0201532915_p1563455532511"><a name="zh-cn_topic_0201532915_p1563455532511"></a><a name="zh-cn_topic_0201532915_p1563455532511"></a><strong id="zh-cn_topic_0201532915_b067124231616"><a name="zh-cn_topic_0201532915_b067124231616"></a><a name="zh-cn_topic_0201532915_b067124231616"></a>监控周期（原始指标）</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201532915_row11634125514251"><td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.7.1.1 "><p id="zh-cn_topic_0201532915_p116341655142512"><a name="zh-cn_topic_0201532915_p116341655142512"></a><a name="zh-cn_topic_0201532915_p116341655142512"></a>snat_connection</p>
</td>
<td class="cellrowborder" valign="top" width="11.59%" headers="mcps1.2.7.1.2 "><p id="zh-cn_topic_0201532915_p16343558256"><a name="zh-cn_topic_0201532915_p16343558256"></a><a name="zh-cn_topic_0201532915_p16343558256"></a>SNAT连接数</p>
</td>
<td class="cellrowborder" valign="top" width="28.77%" headers="mcps1.2.7.1.3 "><p id="zh-cn_topic_0201532915_p6635255102513"><a name="zh-cn_topic_0201532915_p6635255102513"></a><a name="zh-cn_topic_0201532915_p6635255102513"></a>该指标用于统计测量对象的SNAT连接数。</p>
<p id="zh-cn_topic_0201532915_p363510554255"><a name="zh-cn_topic_0201532915_p363510554255"></a><a name="zh-cn_topic_0201532915_p363510554255"></a>单位：个</p>
</td>
<td class="cellrowborder" valign="top" width="9.44%" headers="mcps1.2.7.1.4 "><p id="zh-cn_topic_0201532915_p16351155112516"><a name="zh-cn_topic_0201532915_p16351155112516"></a><a name="zh-cn_topic_0201532915_p16351155112516"></a>≥ 0 个</p>
</td>
<td class="cellrowborder" valign="top" width="16.77%" headers="mcps1.2.7.1.5 "><p id="zh-cn_topic_0201532915_p963515562513"><a name="zh-cn_topic_0201532915_p963515562513"></a><a name="zh-cn_topic_0201532915_p963515562513"></a><span id="ph419543120186"><a name="ph419543120186"></a><a name="ph419543120186"></a>公网NAT网关</span>实例</p>
</td>
<td class="cellrowborder" valign="top" width="15.03%" headers="mcps1.2.7.1.6 "><p id="zh-cn_topic_0201532915_p1963515510259"><a name="zh-cn_topic_0201532915_p1963515510259"></a><a name="zh-cn_topic_0201532915_p1963515510259"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0201532915_row463515562510"><td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.7.1.1 "><p id="zh-cn_topic_0201532915_p126351551258"><a name="zh-cn_topic_0201532915_p126351551258"></a><a name="zh-cn_topic_0201532915_p126351551258"></a>inbound_bandwidth</p>
</td>
<td class="cellrowborder" valign="top" width="11.59%" headers="mcps1.2.7.1.2 "><p id="zh-cn_topic_0201532915_p26351555162513"><a name="zh-cn_topic_0201532915_p26351555162513"></a><a name="zh-cn_topic_0201532915_p26351555162513"></a>入方向带宽</p>
</td>
<td class="cellrowborder" valign="top" width="28.77%" headers="mcps1.2.7.1.3 "><p id="zh-cn_topic_0201532915_p263518551255"><a name="zh-cn_topic_0201532915_p263518551255"></a><a name="zh-cn_topic_0201532915_p263518551255"></a>该指标用于统计入方向带宽。</p>
<p id="zh-cn_topic_0201532915_p16351558259"><a name="zh-cn_topic_0201532915_p16351558259"></a><a name="zh-cn_topic_0201532915_p16351558259"></a>单位：比特/秒</p>
</td>
<td class="cellrowborder" valign="top" width="9.44%" headers="mcps1.2.7.1.4 "><p id="zh-cn_topic_0201532915_p1635175510252"><a name="zh-cn_topic_0201532915_p1635175510252"></a><a name="zh-cn_topic_0201532915_p1635175510252"></a>≥0</p>
<p id="zh-cn_topic_0201532915_p16856133111520"><a name="zh-cn_topic_0201532915_p16856133111520"></a><a name="zh-cn_topic_0201532915_p16856133111520"></a>bit/s</p>
</td>
<td class="cellrowborder" valign="top" width="16.77%" headers="mcps1.2.7.1.5 "><p id="zh-cn_topic_0201532915_p063665513259"><a name="zh-cn_topic_0201532915_p063665513259"></a><a name="zh-cn_topic_0201532915_p063665513259"></a><span id="ph108993361453"><a name="ph108993361453"></a><a name="ph108993361453"></a>公网NAT网关</span>实例</p>
</td>
<td class="cellrowborder" valign="top" width="15.03%" headers="mcps1.2.7.1.6 "><p id="zh-cn_topic_0201532915_p1263620558252"><a name="zh-cn_topic_0201532915_p1263620558252"></a><a name="zh-cn_topic_0201532915_p1263620558252"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0201532915_row66361255132514"><td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.7.1.1 "><p id="zh-cn_topic_0201532915_p76361955132513"><a name="zh-cn_topic_0201532915_p76361955132513"></a><a name="zh-cn_topic_0201532915_p76361955132513"></a>outbound_bandwidth</p>
</td>
<td class="cellrowborder" valign="top" width="11.59%" headers="mcps1.2.7.1.2 "><p id="zh-cn_topic_0201532915_p86361255182513"><a name="zh-cn_topic_0201532915_p86361255182513"></a><a name="zh-cn_topic_0201532915_p86361255182513"></a>出方向带宽</p>
</td>
<td class="cellrowborder" valign="top" width="28.77%" headers="mcps1.2.7.1.3 "><p id="zh-cn_topic_0201532915_p7636185511257"><a name="zh-cn_topic_0201532915_p7636185511257"></a><a name="zh-cn_topic_0201532915_p7636185511257"></a>该指标用于统计SNAT出方向带宽。</p>
<p id="zh-cn_topic_0201532915_p17636105510259"><a name="zh-cn_topic_0201532915_p17636105510259"></a><a name="zh-cn_topic_0201532915_p17636105510259"></a>单位：比特/秒</p>
</td>
<td class="cellrowborder" valign="top" width="9.44%" headers="mcps1.2.7.1.4 "><p id="zh-cn_topic_0201532915_p1636165542514"><a name="zh-cn_topic_0201532915_p1636165542514"></a><a name="zh-cn_topic_0201532915_p1636165542514"></a>≥0</p>
<p id="zh-cn_topic_0201532915_p13227357313"><a name="zh-cn_topic_0201532915_p13227357313"></a><a name="zh-cn_topic_0201532915_p13227357313"></a>bit/s</p>
</td>
<td class="cellrowborder" valign="top" width="16.77%" headers="mcps1.2.7.1.5 "><p id="zh-cn_topic_0201532915_p1663615551251"><a name="zh-cn_topic_0201532915_p1663615551251"></a><a name="zh-cn_topic_0201532915_p1663615551251"></a><span id="ph2088684710515"><a name="ph2088684710515"></a><a name="ph2088684710515"></a>公网NAT网关</span>实例</p>
</td>
<td class="cellrowborder" valign="top" width="15.03%" headers="mcps1.2.7.1.6 "><p id="zh-cn_topic_0201532915_p063725532517"><a name="zh-cn_topic_0201532915_p063725532517"></a><a name="zh-cn_topic_0201532915_p063725532517"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0201532915_row563710558259"><td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.7.1.1 "><p id="zh-cn_topic_0201532915_p1063715513256"><a name="zh-cn_topic_0201532915_p1063715513256"></a><a name="zh-cn_topic_0201532915_p1063715513256"></a>inbound_pps</p>
</td>
<td class="cellrowborder" valign="top" width="11.59%" headers="mcps1.2.7.1.2 "><p id="zh-cn_topic_0201532915_p963765592516"><a name="zh-cn_topic_0201532915_p963765592516"></a><a name="zh-cn_topic_0201532915_p963765592516"></a>入方向PPS</p>
</td>
<td class="cellrowborder" valign="top" width="28.77%" headers="mcps1.2.7.1.3 "><p id="zh-cn_topic_0201532915_p11637355122513"><a name="zh-cn_topic_0201532915_p11637355122513"></a><a name="zh-cn_topic_0201532915_p11637355122513"></a>该指标用于统计SNAT入方向PPS。</p>
<p id="zh-cn_topic_0201532915_p18637175522519"><a name="zh-cn_topic_0201532915_p18637175522519"></a><a name="zh-cn_topic_0201532915_p18637175522519"></a>单位：个</p>
</td>
<td class="cellrowborder" valign="top" width="9.44%" headers="mcps1.2.7.1.4 "><p id="zh-cn_topic_0201532915_p963725502517"><a name="zh-cn_topic_0201532915_p963725502517"></a><a name="zh-cn_topic_0201532915_p963725502517"></a>≥0个</p>
</td>
<td class="cellrowborder" valign="top" width="16.77%" headers="mcps1.2.7.1.5 "><p id="zh-cn_topic_0201532915_p663775572511"><a name="zh-cn_topic_0201532915_p663775572511"></a><a name="zh-cn_topic_0201532915_p663775572511"></a><span id="ph4563105519516"><a name="ph4563105519516"></a><a name="ph4563105519516"></a>公网NAT网关</span>实例</p>
</td>
<td class="cellrowborder" valign="top" width="15.03%" headers="mcps1.2.7.1.6 "><p id="zh-cn_topic_0201532915_p26374554252"><a name="zh-cn_topic_0201532915_p26374554252"></a><a name="zh-cn_topic_0201532915_p26374554252"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0201532915_row46388559258"><td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.7.1.1 "><p id="zh-cn_topic_0201532915_p46382555253"><a name="zh-cn_topic_0201532915_p46382555253"></a><a name="zh-cn_topic_0201532915_p46382555253"></a>outbound_pps</p>
</td>
<td class="cellrowborder" valign="top" width="11.59%" headers="mcps1.2.7.1.2 "><p id="zh-cn_topic_0201532915_p7638105518252"><a name="zh-cn_topic_0201532915_p7638105518252"></a><a name="zh-cn_topic_0201532915_p7638105518252"></a>出方向PPS</p>
</td>
<td class="cellrowborder" valign="top" width="28.77%" headers="mcps1.2.7.1.3 "><p id="zh-cn_topic_0201532915_p5638175532513"><a name="zh-cn_topic_0201532915_p5638175532513"></a><a name="zh-cn_topic_0201532915_p5638175532513"></a>该指标用于统计SNAT出方向PPS。</p>
<p id="zh-cn_topic_0201532915_p563875515256"><a name="zh-cn_topic_0201532915_p563875515256"></a><a name="zh-cn_topic_0201532915_p563875515256"></a>单位：个</p>
</td>
<td class="cellrowborder" valign="top" width="9.44%" headers="mcps1.2.7.1.4 "><p id="zh-cn_topic_0201532915_p136381255162512"><a name="zh-cn_topic_0201532915_p136381255162512"></a><a name="zh-cn_topic_0201532915_p136381255162512"></a>≥0个</p>
</td>
<td class="cellrowborder" valign="top" width="16.77%" headers="mcps1.2.7.1.5 "><p id="zh-cn_topic_0201532915_p063835542515"><a name="zh-cn_topic_0201532915_p063835542515"></a><a name="zh-cn_topic_0201532915_p063835542515"></a><span id="ph169363511611"><a name="ph169363511611"></a><a name="ph169363511611"></a>公网NAT网关</span>实例</p>
</td>
<td class="cellrowborder" valign="top" width="15.03%" headers="mcps1.2.7.1.6 "><p id="zh-cn_topic_0201532915_p11638135562510"><a name="zh-cn_topic_0201532915_p11638135562510"></a><a name="zh-cn_topic_0201532915_p11638135562510"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0201532915_row2638105513256"><td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.7.1.1 "><p id="zh-cn_topic_0201532915_p18638165562514"><a name="zh-cn_topic_0201532915_p18638165562514"></a><a name="zh-cn_topic_0201532915_p18638165562514"></a>inbound_traffic</p>
</td>
<td class="cellrowborder" valign="top" width="11.59%" headers="mcps1.2.7.1.2 "><p id="zh-cn_topic_0201532915_p206381155202510"><a name="zh-cn_topic_0201532915_p206381155202510"></a><a name="zh-cn_topic_0201532915_p206381155202510"></a>入方向流量</p>
</td>
<td class="cellrowborder" valign="top" width="28.77%" headers="mcps1.2.7.1.3 "><p id="zh-cn_topic_0201532915_p8638205517258"><a name="zh-cn_topic_0201532915_p8638205517258"></a><a name="zh-cn_topic_0201532915_p8638205517258"></a>该指标用于统计SNAT入方向流量。</p>
<p id="zh-cn_topic_0201532915_p1463845516256"><a name="zh-cn_topic_0201532915_p1463845516256"></a><a name="zh-cn_topic_0201532915_p1463845516256"></a>单位：字节</p>
</td>
<td class="cellrowborder" valign="top" width="9.44%" headers="mcps1.2.7.1.4 "><p id="zh-cn_topic_0201532915_p1563815516251"><a name="zh-cn_topic_0201532915_p1563815516251"></a><a name="zh-cn_topic_0201532915_p1563815516251"></a>≥0 bytes</p>
</td>
<td class="cellrowborder" valign="top" width="16.77%" headers="mcps1.2.7.1.5 "><p id="zh-cn_topic_0201532915_p663895517254"><a name="zh-cn_topic_0201532915_p663895517254"></a><a name="zh-cn_topic_0201532915_p663895517254"></a><span id="ph193118134617"><a name="ph193118134617"></a><a name="ph193118134617"></a>公网NAT网关</span>实例</p>
</td>
<td class="cellrowborder" valign="top" width="15.03%" headers="mcps1.2.7.1.6 "><p id="zh-cn_topic_0201532915_p1063925510257"><a name="zh-cn_topic_0201532915_p1063925510257"></a><a name="zh-cn_topic_0201532915_p1063925510257"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0201532915_row106391155172519"><td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.7.1.1 "><p id="zh-cn_topic_0201532915_p20639135512511"><a name="zh-cn_topic_0201532915_p20639135512511"></a><a name="zh-cn_topic_0201532915_p20639135512511"></a>outbound_traffic</p>
</td>
<td class="cellrowborder" valign="top" width="11.59%" headers="mcps1.2.7.1.2 "><p id="zh-cn_topic_0201532915_p19639155122512"><a name="zh-cn_topic_0201532915_p19639155122512"></a><a name="zh-cn_topic_0201532915_p19639155122512"></a>出方向流量</p>
</td>
<td class="cellrowborder" valign="top" width="28.77%" headers="mcps1.2.7.1.3 "><p id="zh-cn_topic_0201532915_p12639205552515"><a name="zh-cn_topic_0201532915_p12639205552515"></a><a name="zh-cn_topic_0201532915_p12639205552515"></a>该指标用于统计SNAT出方向流量。</p>
<p id="zh-cn_topic_0201532915_p76391855162519"><a name="zh-cn_topic_0201532915_p76391855162519"></a><a name="zh-cn_topic_0201532915_p76391855162519"></a>单位：字节</p>
</td>
<td class="cellrowborder" valign="top" width="9.44%" headers="mcps1.2.7.1.4 "><p id="zh-cn_topic_0201532915_p1063945502511"><a name="zh-cn_topic_0201532915_p1063945502511"></a><a name="zh-cn_topic_0201532915_p1063945502511"></a>≥0 bytes</p>
</td>
<td class="cellrowborder" valign="top" width="16.77%" headers="mcps1.2.7.1.5 "><p id="zh-cn_topic_0201532915_p663985522514"><a name="zh-cn_topic_0201532915_p663985522514"></a><a name="zh-cn_topic_0201532915_p663985522514"></a><span id="ph1911662210612"><a name="ph1911662210612"></a><a name="ph1911662210612"></a>公网NAT网关</span>实例</p>
</td>
<td class="cellrowborder" valign="top" width="15.03%" headers="mcps1.2.7.1.6 "><p id="zh-cn_topic_0201532915_p86393555251"><a name="zh-cn_topic_0201532915_p86393555251"></a><a name="zh-cn_topic_0201532915_p86393555251"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0201532915_row116251587280"><td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.7.1.1 "><p id="zh-cn_topic_0201532915_p12626195817281"><a name="zh-cn_topic_0201532915_p12626195817281"></a><a name="zh-cn_topic_0201532915_p12626195817281"></a>snat_connection_ratio</p>
</td>
<td class="cellrowborder" valign="top" width="11.59%" headers="mcps1.2.7.1.2 "><p id="zh-cn_topic_0201532915_p136269582283"><a name="zh-cn_topic_0201532915_p136269582283"></a><a name="zh-cn_topic_0201532915_p136269582283"></a>SNAT连接数使用率</p>
</td>
<td class="cellrowborder" valign="top" width="28.77%" headers="mcps1.2.7.1.3 "><p id="zh-cn_topic_0201532915_p13271162326"><a name="zh-cn_topic_0201532915_p13271162326"></a><a name="zh-cn_topic_0201532915_p13271162326"></a>该指标用于统计测量对象的SNAT连接数使用率。连接数最大为规格限制的连接数。详情可查看<a href="https://support.huaweicloud.com/productdesc-natgateway/zh-cn_topic_0086739763.html" target="_blank" rel="noopener noreferrer">产品规格</a>。</p>
<p id="zh-cn_topic_0201532915_p962635811282"><a name="zh-cn_topic_0201532915_p962635811282"></a><a name="zh-cn_topic_0201532915_p962635811282"></a>单位：百分比</p>
</td>
<td class="cellrowborder" valign="top" width="9.44%" headers="mcps1.2.7.1.4 "><p id="zh-cn_topic_0201532915_p5626558172810"><a name="zh-cn_topic_0201532915_p5626558172810"></a><a name="zh-cn_topic_0201532915_p5626558172810"></a>≥0</p>
</td>
<td class="cellrowborder" valign="top" width="16.77%" headers="mcps1.2.7.1.5 "><p id="zh-cn_topic_0201532915_p14146105216322"><a name="zh-cn_topic_0201532915_p14146105216322"></a><a name="zh-cn_topic_0201532915_p14146105216322"></a><span id="ph34632311168"><a name="ph34632311168"></a><a name="ph34632311168"></a>公网NAT网关</span>实例</p>
</td>
<td class="cellrowborder" valign="top" width="15.03%" headers="mcps1.2.7.1.6 "><p id="zh-cn_topic_0201532915_p1762745818288"><a name="zh-cn_topic_0201532915_p1762745818288"></a><a name="zh-cn_topic_0201532915_p1762745818288"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0201532915_row378433617354"><td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.7.1.1 "><p id="zh-cn_topic_0201532915_p1178416364351"><a name="zh-cn_topic_0201532915_p1178416364351"></a><a name="zh-cn_topic_0201532915_p1178416364351"></a>inbound_bandwidth_ratio</p>
</td>
<td class="cellrowborder" valign="top" width="11.59%" headers="mcps1.2.7.1.2 "><p id="zh-cn_topic_0201532915_p27844364355"><a name="zh-cn_topic_0201532915_p27844364355"></a><a name="zh-cn_topic_0201532915_p27844364355"></a>入方向带宽使用率</p>
</td>
<td class="cellrowborder" valign="top" width="28.77%" headers="mcps1.2.7.1.3 "><p id="zh-cn_topic_0201532915_p19296183916364"><a name="zh-cn_topic_0201532915_p19296183916364"></a><a name="zh-cn_topic_0201532915_p19296183916364"></a>该指标用于统计SNAT入方向带宽使用率，公网NAT实例最大带宽20Gbit/s。</p>
<p id="zh-cn_topic_0201532915_p1778463653513"><a name="zh-cn_topic_0201532915_p1778463653513"></a><a name="zh-cn_topic_0201532915_p1778463653513"></a>单位：百分比</p>
</td>
<td class="cellrowborder" valign="top" width="9.44%" headers="mcps1.2.7.1.4 "><p id="zh-cn_topic_0201532915_p167841836113517"><a name="zh-cn_topic_0201532915_p167841836113517"></a><a name="zh-cn_topic_0201532915_p167841836113517"></a>≥0</p>
</td>
<td class="cellrowborder" valign="top" width="16.77%" headers="mcps1.2.7.1.5 "><p id="zh-cn_topic_0201532915_p1434175812411"><a name="zh-cn_topic_0201532915_p1434175812411"></a><a name="zh-cn_topic_0201532915_p1434175812411"></a><span id="ph33624376611"><a name="ph33624376611"></a><a name="ph33624376611"></a>公网NAT网关</span>实例</p>
</td>
<td class="cellrowborder" valign="top" width="15.03%" headers="mcps1.2.7.1.6 "><p id="zh-cn_topic_0201532915_p1178433633517"><a name="zh-cn_topic_0201532915_p1178433633517"></a><a name="zh-cn_topic_0201532915_p1178433633517"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0201532915_row47851936133514"><td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.7.1.1 "><p id="zh-cn_topic_0201532915_p278563693515"><a name="zh-cn_topic_0201532915_p278563693515"></a><a name="zh-cn_topic_0201532915_p278563693515"></a>outbound_bandwidth_ratio</p>
</td>
<td class="cellrowborder" valign="top" width="11.59%" headers="mcps1.2.7.1.2 "><p id="zh-cn_topic_0201532915_p177859362358"><a name="zh-cn_topic_0201532915_p177859362358"></a><a name="zh-cn_topic_0201532915_p177859362358"></a>出方向带宽使用率</p>
</td>
<td class="cellrowborder" valign="top" width="28.77%" headers="mcps1.2.7.1.3 "><p id="zh-cn_topic_0201532915_p55177243316"><a name="zh-cn_topic_0201532915_p55177243316"></a><a name="zh-cn_topic_0201532915_p55177243316"></a>该指标用于统计SNAT出方向带宽使用率。</p>
<p id="zh-cn_topic_0201532915_p24641556437"><a name="zh-cn_topic_0201532915_p24641556437"></a><a name="zh-cn_topic_0201532915_p24641556437"></a>公网NAT实例的最大带宽为20Gbit/s，则出方向带宽使用率为：<strong id="zh-cn_topic_0201532915_b7753155315595"><a name="zh-cn_topic_0201532915_b7753155315595"></a><a name="zh-cn_topic_0201532915_b7753155315595"></a>实际使用带宽</strong>/<strong id="zh-cn_topic_0201532915_b11743116314"><a name="zh-cn_topic_0201532915_b11743116314"></a><a name="zh-cn_topic_0201532915_b11743116314"></a>公网NAT实例最大带宽</strong>*100%。</p>
<p id="zh-cn_topic_0201532915_p37856364355"><a name="zh-cn_topic_0201532915_p37856364355"></a><a name="zh-cn_topic_0201532915_p37856364355"></a>单位：百分比</p>
<div class="note" id="zh-cn_topic_0201532915_note118011155513"><a name="zh-cn_topic_0201532915_note118011155513"></a><a name="zh-cn_topic_0201532915_note118011155513"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0201532915_p69838348541"><a name="zh-cn_topic_0201532915_p69838348541"></a><a name="zh-cn_topic_0201532915_p69838348541"></a>该监控项为针对公网NAT实例性能的监控而不是针对EIP带宽的监控。</p>
</div></div>
</td>
<td class="cellrowborder" valign="top" width="9.44%" headers="mcps1.2.7.1.4 "><p id="zh-cn_topic_0201532915_p18785193614352"><a name="zh-cn_topic_0201532915_p18785193614352"></a><a name="zh-cn_topic_0201532915_p18785193614352"></a>≥0</p>
</td>
<td class="cellrowborder" valign="top" width="16.77%" headers="mcps1.2.7.1.5 "><p id="zh-cn_topic_0201532915_p8456135950"><a name="zh-cn_topic_0201532915_p8456135950"></a><a name="zh-cn_topic_0201532915_p8456135950"></a><span id="ph14564114318611"><a name="ph14564114318611"></a><a name="ph14564114318611"></a>公网NAT网关</span>实例</p>
</td>
<td class="cellrowborder" valign="top" width="15.03%" headers="mcps1.2.7.1.6 "><p id="zh-cn_topic_0201532915_p27851236173513"><a name="zh-cn_topic_0201532915_p27851236173513"></a><a name="zh-cn_topic_0201532915_p27851236173513"></a>1分钟</p>
</td>
</tr>
</tbody>
</table>

**表 2**  私网NAT网关支持的监控指标

<a name="zh-cn_topic_0201532915_table1567213720595"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201532915_row167610375590"><th class="cellrowborder" valign="top" width="25.214957008598276%" id="mcps1.2.7.1.1"><p id="zh-cn_topic_0201532915_p247511271010"><a name="zh-cn_topic_0201532915_p247511271010"></a><a name="zh-cn_topic_0201532915_p247511271010"></a><strong id="zh-cn_topic_0201532915_b20185352191614"><a name="zh-cn_topic_0201532915_b20185352191614"></a><a name="zh-cn_topic_0201532915_b20185352191614"></a>指标ID</strong></p>
</th>
<th class="cellrowborder" valign="top" width="14.107178564287143%" id="mcps1.2.7.1.2"><p id="zh-cn_topic_0201532915_p174751427403"><a name="zh-cn_topic_0201532915_p174751427403"></a><a name="zh-cn_topic_0201532915_p174751427403"></a><strong id="zh-cn_topic_0201532915_b12189185211166"><a name="zh-cn_topic_0201532915_b12189185211166"></a><a name="zh-cn_topic_0201532915_b12189185211166"></a>指标名称</strong></p>
</th>
<th class="cellrowborder" valign="top" width="16.286742651469705%" id="mcps1.2.7.1.3"><p id="zh-cn_topic_0201532915_p18475527706"><a name="zh-cn_topic_0201532915_p18475527706"></a><a name="zh-cn_topic_0201532915_p18475527706"></a><strong id="zh-cn_topic_0201532915_b10194185211162"><a name="zh-cn_topic_0201532915_b10194185211162"></a><a name="zh-cn_topic_0201532915_b10194185211162"></a>指标含义</strong></p>
</th>
<th class="cellrowborder" valign="top" width="11.057788442311537%" id="mcps1.2.7.1.4"><p id="zh-cn_topic_0201532915_p0475327202"><a name="zh-cn_topic_0201532915_p0475327202"></a><a name="zh-cn_topic_0201532915_p0475327202"></a><strong id="zh-cn_topic_0201532915_b1419510528162"><a name="zh-cn_topic_0201532915_b1419510528162"></a><a name="zh-cn_topic_0201532915_b1419510528162"></a>取值范围</strong></p>
</th>
<th class="cellrowborder" valign="top" width="19.28614277144571%" id="mcps1.2.7.1.5"><p id="zh-cn_topic_0201532915_p347572716014"><a name="zh-cn_topic_0201532915_p347572716014"></a><a name="zh-cn_topic_0201532915_p347572716014"></a><strong id="zh-cn_topic_0201532915_b15196155221611"><a name="zh-cn_topic_0201532915_b15196155221611"></a><a name="zh-cn_topic_0201532915_b15196155221611"></a>测量对象</strong></p>
</th>
<th class="cellrowborder" valign="top" width="14.047190561887623%" id="mcps1.2.7.1.6"><p id="zh-cn_topic_0201532915_p1289313411217"><a name="zh-cn_topic_0201532915_p1289313411217"></a><a name="zh-cn_topic_0201532915_p1289313411217"></a><strong id="zh-cn_topic_0201532915_b819855211611"><a name="zh-cn_topic_0201532915_b819855211611"></a><a name="zh-cn_topic_0201532915_b819855211611"></a>监控周期（原始指标）</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201532915_row767717379593"><td class="cellrowborder" valign="top" width="25.214957008598276%" headers="mcps1.2.7.1.1 "><p id="zh-cn_topic_0201532915_p16515107417"><a name="zh-cn_topic_0201532915_p16515107417"></a><a name="zh-cn_topic_0201532915_p16515107417"></a>snat_connection</p>
</td>
<td class="cellrowborder" valign="top" width="14.107178564287143%" headers="mcps1.2.7.1.2 "><p id="zh-cn_topic_0201532915_p165151774118"><a name="zh-cn_topic_0201532915_p165151774118"></a><a name="zh-cn_topic_0201532915_p165151774118"></a>SNAT连接数</p>
</td>
<td class="cellrowborder" valign="top" width="16.286742651469705%" headers="mcps1.2.7.1.3 "><p id="zh-cn_topic_0201532915_p20515678113"><a name="zh-cn_topic_0201532915_p20515678113"></a><a name="zh-cn_topic_0201532915_p20515678113"></a>该指标用于统计测量对象的SNAT连接数。</p>
<p id="zh-cn_topic_0201532915_p451567312"><a name="zh-cn_topic_0201532915_p451567312"></a><a name="zh-cn_topic_0201532915_p451567312"></a>单位：个</p>
</td>
<td class="cellrowborder" valign="top" width="11.057788442311537%" headers="mcps1.2.7.1.4 "><p id="zh-cn_topic_0201532915_p15152079112"><a name="zh-cn_topic_0201532915_p15152079112"></a><a name="zh-cn_topic_0201532915_p15152079112"></a>≥ 0 个</p>
</td>
<td class="cellrowborder" valign="top" width="19.28614277144571%" headers="mcps1.2.7.1.5 "><p id="zh-cn_topic_0201532915_p12515675112"><a name="zh-cn_topic_0201532915_p12515675112"></a><a name="zh-cn_topic_0201532915_p12515675112"></a>私网NAT网关实例</p>
</td>
<td class="cellrowborder" valign="top" width="14.047190561887623%" headers="mcps1.2.7.1.6 "><p id="zh-cn_topic_0201532915_p55157714118"><a name="zh-cn_topic_0201532915_p55157714118"></a><a name="zh-cn_topic_0201532915_p55157714118"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0201532915_row7677123765916"><td class="cellrowborder" valign="top" width="25.214957008598276%" headers="mcps1.2.7.1.1 "><p id="zh-cn_topic_0201532915_p28463281216"><a name="zh-cn_topic_0201532915_p28463281216"></a><a name="zh-cn_topic_0201532915_p28463281216"></a>inbound_bandwidth</p>
</td>
<td class="cellrowborder" valign="top" width="14.107178564287143%" headers="mcps1.2.7.1.2 "><p id="zh-cn_topic_0201532915_p188466286115"><a name="zh-cn_topic_0201532915_p188466286115"></a><a name="zh-cn_topic_0201532915_p188466286115"></a>入方向带宽</p>
</td>
<td class="cellrowborder" valign="top" width="16.286742651469705%" headers="mcps1.2.7.1.3 "><p id="zh-cn_topic_0201532915_p16846628511"><a name="zh-cn_topic_0201532915_p16846628511"></a><a name="zh-cn_topic_0201532915_p16846628511"></a>该指标用于统计入方向带宽。</p>
<p id="zh-cn_topic_0201532915_p198464282011"><a name="zh-cn_topic_0201532915_p198464282011"></a><a name="zh-cn_topic_0201532915_p198464282011"></a>单位：比特/秒</p>
</td>
<td class="cellrowborder" valign="top" width="11.057788442311537%" headers="mcps1.2.7.1.4 "><p id="zh-cn_topic_0201532915_p198460281918"><a name="zh-cn_topic_0201532915_p198460281918"></a><a name="zh-cn_topic_0201532915_p198460281918"></a>≥0 bit/s</p>
</td>
<td class="cellrowborder" valign="top" width="19.28614277144571%" headers="mcps1.2.7.1.5 "><p id="zh-cn_topic_0201532915_p384602810115"><a name="zh-cn_topic_0201532915_p384602810115"></a><a name="zh-cn_topic_0201532915_p384602810115"></a>私网NAT网关实例</p>
</td>
<td class="cellrowborder" valign="top" width="14.047190561887623%" headers="mcps1.2.7.1.6 "><p id="zh-cn_topic_0201532915_p48462281219"><a name="zh-cn_topic_0201532915_p48462281219"></a><a name="zh-cn_topic_0201532915_p48462281219"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0201532915_row6677133735919"><td class="cellrowborder" valign="top" width="25.214957008598276%" headers="mcps1.2.7.1.1 "><p id="zh-cn_topic_0201532915_p19846128512"><a name="zh-cn_topic_0201532915_p19846128512"></a><a name="zh-cn_topic_0201532915_p19846128512"></a>outbound_bandwidth</p>
</td>
<td class="cellrowborder" valign="top" width="14.107178564287143%" headers="mcps1.2.7.1.2 "><p id="zh-cn_topic_0201532915_p684616281116"><a name="zh-cn_topic_0201532915_p684616281116"></a><a name="zh-cn_topic_0201532915_p684616281116"></a>出方向带宽</p>
</td>
<td class="cellrowborder" valign="top" width="16.286742651469705%" headers="mcps1.2.7.1.3 "><p id="zh-cn_topic_0201532915_p884620284113"><a name="zh-cn_topic_0201532915_p884620284113"></a><a name="zh-cn_topic_0201532915_p884620284113"></a>该指标用于统计出方向带宽。</p>
<p id="zh-cn_topic_0201532915_p15846152810117"><a name="zh-cn_topic_0201532915_p15846152810117"></a><a name="zh-cn_topic_0201532915_p15846152810117"></a>单位：比特/秒</p>
</td>
<td class="cellrowborder" valign="top" width="11.057788442311537%" headers="mcps1.2.7.1.4 "><p id="zh-cn_topic_0201532915_p16846328618"><a name="zh-cn_topic_0201532915_p16846328618"></a><a name="zh-cn_topic_0201532915_p16846328618"></a>≥0 bit/s</p>
</td>
<td class="cellrowborder" valign="top" width="19.28614277144571%" headers="mcps1.2.7.1.5 "><p id="zh-cn_topic_0201532915_p584612281113"><a name="zh-cn_topic_0201532915_p584612281113"></a><a name="zh-cn_topic_0201532915_p584612281113"></a>私网NAT网关实例</p>
</td>
<td class="cellrowborder" valign="top" width="14.047190561887623%" headers="mcps1.2.7.1.6 "><p id="zh-cn_topic_0201532915_p7846728419"><a name="zh-cn_topic_0201532915_p7846728419"></a><a name="zh-cn_topic_0201532915_p7846728419"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0201532915_row116781137145912"><td class="cellrowborder" valign="top" width="25.214957008598276%" headers="mcps1.2.7.1.1 "><p id="zh-cn_topic_0201532915_p17846828310"><a name="zh-cn_topic_0201532915_p17846828310"></a><a name="zh-cn_topic_0201532915_p17846828310"></a>inbound_pps</p>
</td>
<td class="cellrowborder" valign="top" width="14.107178564287143%" headers="mcps1.2.7.1.2 "><p id="zh-cn_topic_0201532915_p48467281916"><a name="zh-cn_topic_0201532915_p48467281916"></a><a name="zh-cn_topic_0201532915_p48467281916"></a>入方向PPS</p>
</td>
<td class="cellrowborder" valign="top" width="16.286742651469705%" headers="mcps1.2.7.1.3 "><p id="zh-cn_topic_0201532915_p884610281517"><a name="zh-cn_topic_0201532915_p884610281517"></a><a name="zh-cn_topic_0201532915_p884610281517"></a>该指标用于统计入方向PPS。</p>
<p id="zh-cn_topic_0201532915_p18846328611"><a name="zh-cn_topic_0201532915_p18846328611"></a><a name="zh-cn_topic_0201532915_p18846328611"></a>单位：个</p>
</td>
<td class="cellrowborder" valign="top" width="11.057788442311537%" headers="mcps1.2.7.1.4 "><p id="zh-cn_topic_0201532915_p10846628917"><a name="zh-cn_topic_0201532915_p10846628917"></a><a name="zh-cn_topic_0201532915_p10846628917"></a>≥0个</p>
</td>
<td class="cellrowborder" valign="top" width="19.28614277144571%" headers="mcps1.2.7.1.5 "><p id="zh-cn_topic_0201532915_p18846172815118"><a name="zh-cn_topic_0201532915_p18846172815118"></a><a name="zh-cn_topic_0201532915_p18846172815118"></a>私网NAT网关实例</p>
</td>
<td class="cellrowborder" valign="top" width="14.047190561887623%" headers="mcps1.2.7.1.6 "><p id="zh-cn_topic_0201532915_p198461628312"><a name="zh-cn_topic_0201532915_p198461628312"></a><a name="zh-cn_topic_0201532915_p198461628312"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0201532915_row56781537155912"><td class="cellrowborder" valign="top" width="25.214957008598276%" headers="mcps1.2.7.1.1 "><p id="zh-cn_topic_0201532915_p1497844916119"><a name="zh-cn_topic_0201532915_p1497844916119"></a><a name="zh-cn_topic_0201532915_p1497844916119"></a>outbound_pps</p>
</td>
<td class="cellrowborder" valign="top" width="14.107178564287143%" headers="mcps1.2.7.1.2 "><p id="zh-cn_topic_0201532915_p159787492012"><a name="zh-cn_topic_0201532915_p159787492012"></a><a name="zh-cn_topic_0201532915_p159787492012"></a>出方向PPS</p>
</td>
<td class="cellrowborder" valign="top" width="16.286742651469705%" headers="mcps1.2.7.1.3 "><p id="zh-cn_topic_0201532915_p1978949114"><a name="zh-cn_topic_0201532915_p1978949114"></a><a name="zh-cn_topic_0201532915_p1978949114"></a>该指标用于统计出方向PPS。</p>
<p id="zh-cn_topic_0201532915_p5978164912118"><a name="zh-cn_topic_0201532915_p5978164912118"></a><a name="zh-cn_topic_0201532915_p5978164912118"></a>单位：个</p>
</td>
<td class="cellrowborder" valign="top" width="11.057788442311537%" headers="mcps1.2.7.1.4 "><p id="zh-cn_topic_0201532915_p13978144911117"><a name="zh-cn_topic_0201532915_p13978144911117"></a><a name="zh-cn_topic_0201532915_p13978144911117"></a>≥0个</p>
</td>
<td class="cellrowborder" valign="top" width="19.28614277144571%" headers="mcps1.2.7.1.5 "><p id="zh-cn_topic_0201532915_p2978104919119"><a name="zh-cn_topic_0201532915_p2978104919119"></a><a name="zh-cn_topic_0201532915_p2978104919119"></a>私网NAT网关实例</p>
</td>
<td class="cellrowborder" valign="top" width="14.047190561887623%" headers="mcps1.2.7.1.6 "><p id="zh-cn_topic_0201532915_p1797816491617"><a name="zh-cn_topic_0201532915_p1797816491617"></a><a name="zh-cn_topic_0201532915_p1797816491617"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0201532915_row3678133715592"><td class="cellrowborder" valign="top" width="25.214957008598276%" headers="mcps1.2.7.1.1 "><p id="zh-cn_topic_0201532915_p89787494119"><a name="zh-cn_topic_0201532915_p89787494119"></a><a name="zh-cn_topic_0201532915_p89787494119"></a>inbound_traffic</p>
</td>
<td class="cellrowborder" valign="top" width="14.107178564287143%" headers="mcps1.2.7.1.2 "><p id="zh-cn_topic_0201532915_p497874910117"><a name="zh-cn_topic_0201532915_p497874910117"></a><a name="zh-cn_topic_0201532915_p497874910117"></a>入方向流量</p>
</td>
<td class="cellrowborder" valign="top" width="16.286742651469705%" headers="mcps1.2.7.1.3 "><p id="zh-cn_topic_0201532915_p59781849911"><a name="zh-cn_topic_0201532915_p59781849911"></a><a name="zh-cn_topic_0201532915_p59781849911"></a>该指标用于统计入方向流量。</p>
<p id="zh-cn_topic_0201532915_p1997894918113"><a name="zh-cn_topic_0201532915_p1997894918113"></a><a name="zh-cn_topic_0201532915_p1997894918113"></a>单位：字节</p>
</td>
<td class="cellrowborder" valign="top" width="11.057788442311537%" headers="mcps1.2.7.1.4 "><p id="zh-cn_topic_0201532915_p297813491619"><a name="zh-cn_topic_0201532915_p297813491619"></a><a name="zh-cn_topic_0201532915_p297813491619"></a>≥0 bytes</p>
</td>
<td class="cellrowborder" valign="top" width="19.28614277144571%" headers="mcps1.2.7.1.5 "><p id="zh-cn_topic_0201532915_p79781749412"><a name="zh-cn_topic_0201532915_p79781749412"></a><a name="zh-cn_topic_0201532915_p79781749412"></a>私网NAT网关实例</p>
</td>
<td class="cellrowborder" valign="top" width="14.047190561887623%" headers="mcps1.2.7.1.6 "><p id="zh-cn_topic_0201532915_p49788491119"><a name="zh-cn_topic_0201532915_p49788491119"></a><a name="zh-cn_topic_0201532915_p49788491119"></a>1分钟</p>
</td>
</tr>
<tr id="zh-cn_topic_0201532915_row467863711594"><td class="cellrowborder" valign="top" width="25.214957008598276%" headers="mcps1.2.7.1.1 "><p id="zh-cn_topic_0201532915_p897815491117"><a name="zh-cn_topic_0201532915_p897815491117"></a><a name="zh-cn_topic_0201532915_p897815491117"></a>outbound_traffic</p>
</td>
<td class="cellrowborder" valign="top" width="14.107178564287143%" headers="mcps1.2.7.1.2 "><p id="zh-cn_topic_0201532915_p9978149716"><a name="zh-cn_topic_0201532915_p9978149716"></a><a name="zh-cn_topic_0201532915_p9978149716"></a>出方向流量</p>
</td>
<td class="cellrowborder" valign="top" width="16.286742651469705%" headers="mcps1.2.7.1.3 "><p id="zh-cn_topic_0201532915_p17978154919118"><a name="zh-cn_topic_0201532915_p17978154919118"></a><a name="zh-cn_topic_0201532915_p17978154919118"></a>该指标用于统计出方向流量。</p>
<p id="zh-cn_topic_0201532915_p1297864911114"><a name="zh-cn_topic_0201532915_p1297864911114"></a><a name="zh-cn_topic_0201532915_p1297864911114"></a>单位：字节</p>
</td>
<td class="cellrowborder" valign="top" width="11.057788442311537%" headers="mcps1.2.7.1.4 "><p id="zh-cn_topic_0201532915_p1897816491518"><a name="zh-cn_topic_0201532915_p1897816491518"></a><a name="zh-cn_topic_0201532915_p1897816491518"></a>≥0 bytes</p>
</td>
<td class="cellrowborder" valign="top" width="19.28614277144571%" headers="mcps1.2.7.1.5 "><p id="zh-cn_topic_0201532915_p1997884911118"><a name="zh-cn_topic_0201532915_p1997884911118"></a><a name="zh-cn_topic_0201532915_p1997884911118"></a>私网NAT网关实例</p>
</td>
<td class="cellrowborder" valign="top" width="14.047190561887623%" headers="mcps1.2.7.1.6 "><p id="zh-cn_topic_0201532915_p1597814491115"><a name="zh-cn_topic_0201532915_p1597814491115"></a><a name="zh-cn_topic_0201532915_p1597814491115"></a>1分钟</p>
</td>
</tr>
</tbody>
</table>

## 维度<a name="zh-cn_topic_0201532915_section11173113215254"></a>

<a name="zh-cn_topic_0201532915_zh-cn_topic_0102475743_table13291038182217"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201532915_zh-cn_topic_0102475743_row13292153862219"><th class="cellrowborder" valign="top" width="40.400000000000006%" id="mcps1.1.3.1.1"><p id="zh-cn_topic_0201532915_zh-cn_topic_0102475743_p17292638192211"><a name="zh-cn_topic_0201532915_zh-cn_topic_0102475743_p17292638192211"></a><a name="zh-cn_topic_0201532915_zh-cn_topic_0102475743_p17292638192211"></a><strong id="zh-cn_topic_0201532915_b530316586167"><a name="zh-cn_topic_0201532915_b530316586167"></a><a name="zh-cn_topic_0201532915_b530316586167"></a>Key</strong></p>
</th>
<th class="cellrowborder" valign="top" width="59.599999999999994%" id="mcps1.1.3.1.2"><p id="zh-cn_topic_0201532915_zh-cn_topic_0102475743_p92938385226"><a name="zh-cn_topic_0201532915_zh-cn_topic_0102475743_p92938385226"></a><a name="zh-cn_topic_0201532915_zh-cn_topic_0102475743_p92938385226"></a><strong id="zh-cn_topic_0201532915_b1730655814161"><a name="zh-cn_topic_0201532915_b1730655814161"></a><a name="zh-cn_topic_0201532915_b1730655814161"></a>Value</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201532915_zh-cn_topic_0102475743_row1429373812228"><td class="cellrowborder" valign="top" width="40.400000000000006%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0201532915_zh-cn_topic_0102475743_p11777171991217"><a name="zh-cn_topic_0201532915_zh-cn_topic_0102475743_p11777171991217"></a><a name="zh-cn_topic_0201532915_zh-cn_topic_0102475743_p11777171991217"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="59.599999999999994%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0201532915_zh-cn_topic_0102475743_p11777101931217"><a name="zh-cn_topic_0201532915_zh-cn_topic_0102475743_p11777101931217"></a><a name="zh-cn_topic_0201532915_zh-cn_topic_0102475743_p11777101931217"></a><span id="ph16958171412217"><a name="ph16958171412217"></a><a name="ph16958171412217"></a>公网NAT网关</span>实例标识</p>
</td>
</tr>
<tr id="zh-cn_topic_0201532915_row20140137192511"><td class="cellrowborder" valign="top" width="40.400000000000006%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0201532915_p13141123782513"><a name="zh-cn_topic_0201532915_p13141123782513"></a><a name="zh-cn_topic_0201532915_p13141123782513"></a>vpc_nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="59.599999999999994%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0201532915_p014183716255"><a name="zh-cn_topic_0201532915_p014183716255"></a><a name="zh-cn_topic_0201532915_p014183716255"></a>私网NAT实例标识</p>
</td>
</tr>
</tbody>
</table>

