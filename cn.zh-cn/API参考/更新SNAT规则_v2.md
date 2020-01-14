# 更新SNAT规则<a name="nat_apiv2_0014"></a>

## 功能介绍<a name="zh-cn_topic_0168797262_section4303471762"></a>

更新SNAT规则。

>![](public_sys-resources/icon-note.gif) **说明：**   
>更新弹性公网IP的地址或者更新描述时，要求SNAT规则状态status = "ACTIVE"，要求网关管理员状态admin\_state\_up = True。  

## URI<a name="zh-cn_topic_0168797262_section1130447561"></a>

PUT /v2/\{project\_id\}/snat\_rules/\{snat\_rule\_id\}

**表 1**  参数说明

<a name="zh-cn_topic_0168797262_table15301247966"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797262_row1935819471269"><th class="cellrowborder" valign="top" width="22.84%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797262_p1358347161"><a name="zh-cn_topic_0168797262_p1358347161"></a><a name="zh-cn_topic_0168797262_p1358347161"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="9.07%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797262_p335817471567"><a name="zh-cn_topic_0168797262_p335817471567"></a><a name="zh-cn_topic_0168797262_p335817471567"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.790000000000001%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797262_p167781145103713"><a name="zh-cn_topic_0168797262_p167781145103713"></a><a name="zh-cn_topic_0168797262_p167781145103713"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.300000000000004%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797262_p835812471666"><a name="zh-cn_topic_0168797262_p835812471666"></a><a name="zh-cn_topic_0168797262_p835812471666"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797262_row7358647263"><td class="cellrowborder" valign="top" width="22.84%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797262_p135815471961"><a name="zh-cn_topic_0168797262_p135815471961"></a><a name="zh-cn_topic_0168797262_p135815471961"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="9.07%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797262_p11358347365"><a name="zh-cn_topic_0168797262_p11358347365"></a><a name="zh-cn_topic_0168797262_p11358347365"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.790000000000001%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797262_p977814514375"><a name="zh-cn_topic_0168797262_p977814514375"></a><a name="zh-cn_topic_0168797262_p977814514375"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.300000000000004%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797262_p1035813478610"><a name="zh-cn_topic_0168797262_p1035813478610"></a><a name="zh-cn_topic_0168797262_p1035813478610"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797262_row435815471268"><td class="cellrowborder" valign="top" width="22.84%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797262_p535818471766"><a name="zh-cn_topic_0168797262_p535818471766"></a><a name="zh-cn_topic_0168797262_p535818471766"></a>snat_rule_id</p>
</td>
<td class="cellrowborder" valign="top" width="9.07%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797262_p1135844710613"><a name="zh-cn_topic_0168797262_p1135844710613"></a><a name="zh-cn_topic_0168797262_p1135844710613"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.790000000000001%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797262_p57785453379"><a name="zh-cn_topic_0168797262_p57785453379"></a><a name="zh-cn_topic_0168797262_p57785453379"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.300000000000004%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797262_p435812471368"><a name="zh-cn_topic_0168797262_p435812471368"></a><a name="zh-cn_topic_0168797262_p435812471368"></a>SNAT规则的id。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0168797262_section3451047365"></a>

请求参数如[表2](#zh-cn_topic_0168797262_table14822100163510)所示。

**表 2**  请求参数

<a name="zh-cn_topic_0168797262_table14822100163510"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797262_row168221301359"><th class="cellrowborder" valign="top" width="23.1%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797262_p237919923516"><a name="zh-cn_topic_0168797262_p237919923516"></a><a name="zh-cn_topic_0168797262_p237919923516"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="7.93%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797262_p15379209203517"><a name="zh-cn_topic_0168797262_p15379209203517"></a><a name="zh-cn_topic_0168797262_p15379209203517"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.79%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797262_p14379492357"><a name="zh-cn_topic_0168797262_p14379492357"></a><a name="zh-cn_topic_0168797262_p14379492357"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.17999999999999%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797262_p337929133520"><a name="zh-cn_topic_0168797262_p337929133520"></a><a name="zh-cn_topic_0168797262_p337929133520"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797262_row382214013510"><td class="cellrowborder" valign="top" width="23.1%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797262_p1838012933514"><a name="zh-cn_topic_0168797262_p1838012933514"></a><a name="zh-cn_topic_0168797262_p1838012933514"></a>snat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="7.93%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797262_p83805911358"><a name="zh-cn_topic_0168797262_p83805911358"></a><a name="zh-cn_topic_0168797262_p83805911358"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.79%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797262_p538019153510"><a name="zh-cn_topic_0168797262_p538019153510"></a><a name="zh-cn_topic_0168797262_p538019153510"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.17999999999999%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797262_p6380109143511"><a name="zh-cn_topic_0168797262_p6380109143511"></a><a name="zh-cn_topic_0168797262_p6380109143511"></a>snat_rule对象。请参考<a href="#zh-cn_topic_0168797262_table124514471766">表 snat_rule字段说明</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  snat\_rule字段说明

<a name="zh-cn_topic_0168797262_table124514471766"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797262_row153580471463"><th class="cellrowborder" valign="top" width="22.67%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797262_p18358154717620"><a name="zh-cn_topic_0168797262_p18358154717620"></a><a name="zh-cn_topic_0168797262_p18358154717620"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.309999999999999%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797262_p1235812471263"><a name="zh-cn_topic_0168797262_p1235812471263"></a><a name="zh-cn_topic_0168797262_p1235812471263"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.04%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797262_p235818472619"><a name="zh-cn_topic_0168797262_p235818472619"></a><a name="zh-cn_topic_0168797262_p235818472619"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.98%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797262_p1935820476613"><a name="zh-cn_topic_0168797262_p1935820476613"></a><a name="zh-cn_topic_0168797262_p1935820476613"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797262_row14358204719614"><td class="cellrowborder" valign="top" width="22.67%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797262_p1835874712617"><a name="zh-cn_topic_0168797262_p1835874712617"></a><a name="zh-cn_topic_0168797262_p1835874712617"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.309999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797262_p5358184712616"><a name="zh-cn_topic_0168797262_p5358184712616"></a><a name="zh-cn_topic_0168797262_p5358184712616"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.04%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797262_p183588476619"><a name="zh-cn_topic_0168797262_p183588476619"></a><a name="zh-cn_topic_0168797262_p183588476619"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.98%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797262_p1635844710611"><a name="zh-cn_topic_0168797262_p1635844710611"></a><a name="zh-cn_topic_0168797262_p1635844710611"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797262_row83581647169"><td class="cellrowborder" valign="top" width="22.67%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797262_p203581447165"><a name="zh-cn_topic_0168797262_p203581447165"></a><a name="zh-cn_topic_0168797262_p203581447165"></a>public_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="8.309999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797262_p1735819479613"><a name="zh-cn_topic_0168797262_p1735819479613"></a><a name="zh-cn_topic_0168797262_p1735819479613"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.04%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797262_p93581475612"><a name="zh-cn_topic_0168797262_p93581475612"></a><a name="zh-cn_topic_0168797262_p93581475612"></a>String(1024)</p>
</td>
<td class="cellrowborder" valign="top" width="54.98%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0168797262_ul1935812471663"></a><a name="zh-cn_topic_0168797262_ul1935812471663"></a><ul id="zh-cn_topic_0168797262_ul1935812471663"><li>功能说明：弹性公网IP，多个弹性公网IP使用逗号分隔。</li><li>取值范围：最大长度1024字节。</li><li>约束：弹性公网IP个数不能超过20个</li><li>获取弹性公网IP地址的方法请参考<a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090598.html" target="_blank" rel="noopener noreferrer">查询弹性公网IP列表</a>。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797262_row83582471861"><td class="cellrowborder" valign="top" width="22.67%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797262_p193581847161"><a name="zh-cn_topic_0168797262_p193581847161"></a><a name="zh-cn_topic_0168797262_p193581847161"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="8.309999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797262_p135814713612"><a name="zh-cn_topic_0168797262_p135814713612"></a><a name="zh-cn_topic_0168797262_p135814713612"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.04%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797262_p133589472063"><a name="zh-cn_topic_0168797262_p133589472063"></a><a name="zh-cn_topic_0168797262_p133589472063"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="54.98%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797262_p13581471663"><a name="zh-cn_topic_0168797262_p13581471663"></a><a name="zh-cn_topic_0168797262_p13581471663"></a>SNAT规则的描述。</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="zh-cn_topic_0168797262_section8618475619"></a>

响应参数如[表4](#zh-cn_topic_0168797262_table1774471665)所示。

**表 4**  响应参数

<a name="zh-cn_topic_0168797262_table1774471665"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797262_row14358124720612"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797262_p5358104711614"><a name="zh-cn_topic_0168797262_p5358104711614"></a><a name="zh-cn_topic_0168797262_p5358104711614"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="22.93%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797262_p7358154717618"><a name="zh-cn_topic_0168797262_p7358154717618"></a><a name="zh-cn_topic_0168797262_p7358154717618"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.07%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797262_p18358147964"><a name="zh-cn_topic_0168797262_p18358147964"></a><a name="zh-cn_topic_0168797262_p18358147964"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797262_row203586471566"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797262_p1835812472615"><a name="zh-cn_topic_0168797262_p1835812472615"></a><a name="zh-cn_topic_0168797262_p1835812472615"></a>snat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="22.93%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797262_p935814716614"><a name="zh-cn_topic_0168797262_p935814716614"></a><a name="zh-cn_topic_0168797262_p935814716614"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="57.07%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797262_p1835811477615"><a name="zh-cn_topic_0168797262_p1835811477615"></a><a name="zh-cn_topic_0168797262_p1835811477615"></a>snat_rule对象。</p>
</td>
</tr>
</tbody>
</table>

**表 5**  snat\_rule字段说明

<a name="zh-cn_topic_0168797262_table207724713612"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797262_row535884715611"><th class="cellrowborder" valign="top" width="23.23%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797262_p1735810478612"><a name="zh-cn_topic_0168797262_p1735810478612"></a><a name="zh-cn_topic_0168797262_p1735810478612"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.189999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797262_p83581947868"><a name="zh-cn_topic_0168797262_p83581947868"></a><a name="zh-cn_topic_0168797262_p83581947868"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797262_p835812471362"><a name="zh-cn_topic_0168797262_p835812471362"></a><a name="zh-cn_topic_0168797262_p835812471362"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797262_row13358174719613"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797262_p7358747560"><a name="zh-cn_topic_0168797262_p7358747560"></a><a name="zh-cn_topic_0168797262_p7358747560"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797262_p235819471868"><a name="zh-cn_topic_0168797262_p235819471868"></a><a name="zh-cn_topic_0168797262_p235819471868"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797262_p135884718617"><a name="zh-cn_topic_0168797262_p135884718617"></a><a name="zh-cn_topic_0168797262_p135884718617"></a>SNAT规则的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797262_row10358194711617"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797262_p635824712620"><a name="zh-cn_topic_0168797262_p635824712620"></a><a name="zh-cn_topic_0168797262_p635824712620"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797262_p19358104711616"><a name="zh-cn_topic_0168797262_p19358104711616"></a><a name="zh-cn_topic_0168797262_p19358104711616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797262_p835810478611"><a name="zh-cn_topic_0168797262_p835810478611"></a><a name="zh-cn_topic_0168797262_p835810478611"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797262_row13581447269"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797262_p9358144720614"><a name="zh-cn_topic_0168797262_p9358144720614"></a><a name="zh-cn_topic_0168797262_p9358144720614"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797262_p143588478612"><a name="zh-cn_topic_0168797262_p143588478612"></a><a name="zh-cn_topic_0168797262_p143588478612"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797262_p13358104710613"><a name="zh-cn_topic_0168797262_p13358104710613"></a><a name="zh-cn_topic_0168797262_p13358104710613"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797262_row0358114718615"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797262_p63588471566"><a name="zh-cn_topic_0168797262_p63588471566"></a><a name="zh-cn_topic_0168797262_p63588471566"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797262_p935814471161"><a name="zh-cn_topic_0168797262_p935814471161"></a><a name="zh-cn_topic_0168797262_p935814471161"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797262_p123588471167"><a name="zh-cn_topic_0168797262_p123588471167"></a><a name="zh-cn_topic_0168797262_p123588471167"></a>规则使用的网络id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797262_row935817473613"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797262_p635814472069"><a name="zh-cn_topic_0168797262_p635814472069"></a><a name="zh-cn_topic_0168797262_p635814472069"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797262_p4358104713617"><a name="zh-cn_topic_0168797262_p4358104713617"></a><a name="zh-cn_topic_0168797262_p4358104713617"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797262_p53584471467"><a name="zh-cn_topic_0168797262_p53584471467"></a><a name="zh-cn_topic_0168797262_p53584471467"></a>cidr，vpc 子网网段的子集或专线侧网段。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797262_row335864710618"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797262_p335811478613"><a name="zh-cn_topic_0168797262_p335811478613"></a><a name="zh-cn_topic_0168797262_p335811478613"></a>source_type</p>
</td>
<td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797262_p5841434155217"><a name="zh-cn_topic_0168797262_p5841434155217"></a><a name="zh-cn_topic_0168797262_p5841434155217"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797262_p63581474613"><a name="zh-cn_topic_0168797262_p63581474613"></a><a name="zh-cn_topic_0168797262_p63581474613"></a>0：VPC侧，可以指定network_id 或者cidr。</p>
<p id="zh-cn_topic_0168797262_p43588471617"><a name="zh-cn_topic_0168797262_p43588471617"></a><a name="zh-cn_topic_0168797262_p43588471617"></a>1：专线侧，只能指定cidr。</p>
<p id="zh-cn_topic_0168797262_p835815471666"><a name="zh-cn_topic_0168797262_p835815471666"></a><a name="zh-cn_topic_0168797262_p835815471666"></a>不输入默认为0（VPC）。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797262_row1835812473612"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797262_p10358647660"><a name="zh-cn_topic_0168797262_p10358647660"></a><a name="zh-cn_topic_0168797262_p10358647660"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797262_p43582479614"><a name="zh-cn_topic_0168797262_p43582479614"></a><a name="zh-cn_topic_0168797262_p43582479614"></a>String(4096)</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797262_ul1535894711615"></a><a name="zh-cn_topic_0168797262_ul1535894711615"></a><ul id="zh-cn_topic_0168797262_ul1535894711615"><li>功能说明：弹性公网IP的id，多个弹性公网IP使用逗号分隔。</li><li>取值范围：最大长度4096字节。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797262_row435814471767"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797262_p18358124712616"><a name="zh-cn_topic_0168797262_p18358124712616"></a><a name="zh-cn_topic_0168797262_p18358124712616"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797262_p11358747568"><a name="zh-cn_topic_0168797262_p11358747568"></a><a name="zh-cn_topic_0168797262_p11358747568"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797262_p103581847660"><a name="zh-cn_topic_0168797262_p103581847660"></a><a name="zh-cn_topic_0168797262_p103581847660"></a>SNAT规则的描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797262_row1735814713614"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797262_p143585471365"><a name="zh-cn_topic_0168797262_p143585471365"></a><a name="zh-cn_topic_0168797262_p143585471365"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797262_p1035812471763"><a name="zh-cn_topic_0168797262_p1035812471763"></a><a name="zh-cn_topic_0168797262_p1035812471763"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797262_ul173582047761"></a><a name="zh-cn_topic_0168797262_ul173582047761"></a><ul id="zh-cn_topic_0168797262_ul173582047761"><li>功能说明：SNAT规则的状态。</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797262_row1335834718618"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797262_p1635813471269"><a name="zh-cn_topic_0168797262_p1635813471269"></a><a name="zh-cn_topic_0168797262_p1635813471269"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797262_p13409122018276"><a name="zh-cn_topic_0168797262_p13409122018276"></a><a name="zh-cn_topic_0168797262_p13409122018276"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797262_ul71858556358"></a><a name="zh-cn_topic_0168797262_ul71858556358"></a><ul id="zh-cn_topic_0168797262_ul71858556358"><li>解冻/冻结状态。</li><li>取值范围：<a name="zh-cn_topic_0168797262_ul11838172814409"></a><a name="zh-cn_topic_0168797262_ul11838172814409"></a><ul id="zh-cn_topic_0168797262_ul11838172814409"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797262_row133583477612"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797262_p1335894716612"><a name="zh-cn_topic_0168797262_p1335894716612"></a><a name="zh-cn_topic_0168797262_p1335894716612"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797262_p135864711615"><a name="zh-cn_topic_0168797262_p135864711615"></a><a name="zh-cn_topic_0168797262_p135864711615"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797262_ul33581447666"></a><a name="zh-cn_topic_0168797262_ul33581447666"></a><ul id="zh-cn_topic_0168797262_ul33581447666"><li>SNAT规则的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797262_row93584471663"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797262_p63581047061"><a name="zh-cn_topic_0168797262_p63581047061"></a><a name="zh-cn_topic_0168797262_p63581047061"></a>public_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797262_p73587471867"><a name="zh-cn_topic_0168797262_p73587471867"></a><a name="zh-cn_topic_0168797262_p73587471867"></a>String(1024)</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797262_ul13358154715610"></a><a name="zh-cn_topic_0168797262_ul13358154715610"></a><ul id="zh-cn_topic_0168797262_ul13358154715610"><li>功能说明：弹性公网IP，多个弹性公网IP使用逗号分隔。</li><li>取值范围：最大长度1024字节。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797262_row15358247165"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797262_p1135812471861"><a name="zh-cn_topic_0168797262_p1135812471861"></a><a name="zh-cn_topic_0168797262_p1135812471861"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797262_p63581047262"><a name="zh-cn_topic_0168797262_p63581047262"></a><a name="zh-cn_topic_0168797262_p63581047262"></a>String(1024)</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797262_ul1935813477612"></a><a name="zh-cn_topic_0168797262_ul1935813477612"></a><ul id="zh-cn_topic_0168797262_ul1935813477612"><li>功能说明：冻结的弹性公网IP，多个冻结的弹性公网IP使用逗号分隔。</li><li>取值范围：最大长度1024字节。</li></ul>
</td>
</tr>
</tbody>
</table>

## 示例<a name="zh-cn_topic_0168797262_section315519471162"></a>

-   请求样例

    ```
    PUT https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/snat_rules/5b95c675-69c2-4656-ba06-58ff72e1d338 
     { 
         "snat_rule": { 
             "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8", 
             "description": "my snat rule 01", 
             "public_ip_address": "10.15.10.11,10.15.10.12" 
         } 
     }
    ```

-   响应样例

    ```
    { 
         "snat_rule": { 
             "floating_ip_id": " bdc10a4c-d81a-41ec-adf7-de857f7c812a,7a094014-9657-463f-972b-e84d56b931a0", 
             "status": "PENDING_UPDATE", 
             "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8", 
             "admin_state_up": true, 
             "network_id": "eaad9cd6-2372-4be1-9535-9bd37210ae7b",
             "source_type":0, 
             "tenant_id": "27e25061336f4af590faeabeb7fcd9a3", 
             "created_at": "2017-11-18 07:54:21.665430", 
             "id": "5b95c675-69c2-4656-ba06-58ff72e1d338", 
             "public_ip_address": "10.15.10.11,10.15.10.12",        ,
             "floating_ip_address": "",
             "description": "my snat rule 01" 
         } 
     }
    ```


## 状态码<a name="zh-cn_topic_0168797262_section7155134719617"></a>

请参考[状态码](状态码.md)。

