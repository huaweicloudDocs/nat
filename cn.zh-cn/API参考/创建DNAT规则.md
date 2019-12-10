# 创建DNAT规则<a name="ZH-CN_TOPIC_0201533649"></a>

## 功能介绍<a name="section2213133217038"></a>

创建DNAT规则

>![](public_sys-resources/icon-note.gif) **说明：**   
>创建规则时，要求网关状态status = "ACTIVE"，要求网关管理员状态admin\_state\_up = True。port\_id和private\_ip不能同时生效。对于all port类型的规则，要求internal\_service\_port = 0，external\_service\_port = 0，protocol = ANY.  

## URI<a name="section2631225217131"></a>

POST /v2.0/dnat\_rules

## 请求消息<a name="section1572764517510"></a>

请求参数如[表1](#table19385203615518)所示。

**表 1**  请求参数

<a name="table19385203615518"></a>
<table><thead align="left"><tr id="row7697336175113"><th class="cellrowborder" valign="top" width="21.19%" id="mcps1.2.5.1.1"><p id="p969713363516"><a name="p969713363516"></a><a name="p969713363516"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="12.29%" id="mcps1.2.5.1.2"><p id="p1269717362514"><a name="p1269717362514"></a><a name="p1269717362514"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.02%" id="mcps1.2.5.1.3"><p id="p269717363519"><a name="p269717363519"></a><a name="p269717363519"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="49.5%" id="mcps1.2.5.1.4"><p id="p176971936105117"><a name="p176971936105117"></a><a name="p176971936105117"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row4697436175118"><td class="cellrowborder" valign="top" width="21.19%" headers="mcps1.2.5.1.1 "><p id="p96971336105112"><a name="p96971336105112"></a><a name="p96971336105112"></a>dnat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="12.29%" headers="mcps1.2.5.1.2 "><p id="p7697436175113"><a name="p7697436175113"></a><a name="p7697436175113"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.02%" headers="mcps1.2.5.1.3 "><p id="p1869713366514"><a name="p1869713366514"></a><a name="p1869713366514"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="49.5%" headers="mcps1.2.5.1.4 "><p id="p14697113614518"><a name="p14697113614518"></a><a name="p14697113614518"></a>dnat_rule对象。详见<a href="#table132796437212">表2</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  dnat\_rule字段说明

<a name="table132796437212"></a>
<table><thead align="left"><tr id="row184049431027"><th class="cellrowborder" valign="top" width="20.919999999999998%" id="mcps1.2.5.1.1"><p id="p14043431726"><a name="p14043431726"></a><a name="p14043431726"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="12.29%" id="mcps1.2.5.1.2"><p id="p154049430210"><a name="p154049430210"></a><a name="p154049430210"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.02%" id="mcps1.2.5.1.3"><p id="p1740416433219"><a name="p1740416433219"></a><a name="p1740416433219"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="49.769999999999996%" id="mcps1.2.5.1.4"><p id="p240420437215"><a name="p240420437215"></a><a name="p240420437215"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row134041433214"><td class="cellrowborder" valign="top" width="20.919999999999998%" headers="mcps1.2.5.1.1 "><p id="p164043431129"><a name="p164043431129"></a><a name="p164043431129"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="12.29%" headers="mcps1.2.5.1.2 "><p id="p1140424312213"><a name="p1140424312213"></a><a name="p1140424312213"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.02%" headers="mcps1.2.5.1.3 "><p id="p8404443921"><a name="p8404443921"></a><a name="p8404443921"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="49.769999999999996%" headers="mcps1.2.5.1.4 "><p id="p1440494313213"><a name="p1440494313213"></a><a name="p1440494313213"></a>所属NAT网关的id。</p>
</td>
</tr>
<tr id="row040412436218"><td class="cellrowborder" valign="top" width="20.919999999999998%" headers="mcps1.2.5.1.1 "><p id="p19404204314213"><a name="p19404204314213"></a><a name="p19404204314213"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="12.29%" headers="mcps1.2.5.1.2 "><p id="p154048432027"><a name="p154048432027"></a><a name="p154048432027"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.02%" headers="mcps1.2.5.1.3 "><p id="p540414431823"><a name="p540414431823"></a><a name="p540414431823"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="49.769999999999996%" headers="mcps1.2.5.1.4 "><p id="p86078310224"><a name="p86078310224"></a><a name="p86078310224"></a>虚拟机或者裸机的Port ID，与private_ip参数二选一。</p>
<p id="p13404243429"><a name="p13404243429"></a><a name="p13404243429"></a>获取虚拟机Port ID的方法请参考<a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0077845908.html" target="_blank" rel="noopener noreferrer">查询云服务器网卡信息</a>，获取裸机Port ID的方法请参考<a href="https://support.huaweicloud.com/api-bms/zh-cn_topic_0053158696.html" target="_blank" rel="noopener noreferrer">查询裸金属服务器IP地址</a>。</p>
</td>
</tr>
<tr id="row14041643528"><td class="cellrowborder" valign="top" width="20.919999999999998%" headers="mcps1.2.5.1.1 "><p id="p740415432025"><a name="p740415432025"></a><a name="p740415432025"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="12.29%" headers="mcps1.2.5.1.2 "><p id="p12404194314216"><a name="p12404194314216"></a><a name="p12404194314216"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.02%" headers="mcps1.2.5.1.3 "><p id="p184045434218"><a name="p184045434218"></a><a name="p184045434218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="49.769999999999996%" headers="mcps1.2.5.1.4 "><p id="p84041843221"><a name="p84041843221"></a><a name="p84041843221"></a>用户私有IP地址，例如专线连接的私有云地址，与port_id参数二选一。</p>
</td>
</tr>
<tr id="row16404204313220"><td class="cellrowborder" valign="top" width="20.919999999999998%" headers="mcps1.2.5.1.1 "><p id="p5404144313210"><a name="p5404144313210"></a><a name="p5404144313210"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="12.29%" headers="mcps1.2.5.1.2 "><p id="p64041431726"><a name="p64041431726"></a><a name="p64041431726"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.02%" headers="mcps1.2.5.1.3 "><p id="p740413431823"><a name="p740413431823"></a><a name="p740413431823"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="49.769999999999996%" headers="mcps1.2.5.1.4 "><p id="p1740419431628"><a name="p1740419431628"></a><a name="p1740419431628"></a>虚拟机或者裸机对外提供服务的协议端口号。</p>
<p id="p223280102618"><a name="p223280102618"></a><a name="p223280102618"></a>取值范围：0~65535。</p>
</td>
</tr>
<tr id="row14404174310215"><td class="cellrowborder" valign="top" width="20.919999999999998%" headers="mcps1.2.5.1.1 "><p id="p19404343926"><a name="p19404343926"></a><a name="p19404343926"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="12.29%" headers="mcps1.2.5.1.2 "><p id="p144048432217"><a name="p144048432217"></a><a name="p144048432217"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.02%" headers="mcps1.2.5.1.3 "><p id="p240484314213"><a name="p240484314213"></a><a name="p240484314213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="49.769999999999996%" headers="mcps1.2.5.1.4 "><p id="p1404343021"><a name="p1404343021"></a><a name="p1404343021"></a>弹性公网IP的id。获取弹性公网IP的id的方法请参考<a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090598.html" target="_blank" rel="noopener noreferrer">查询弹性公网IP列表</a>。</p>
</td>
</tr>
<tr id="row74041243421"><td class="cellrowborder" valign="top" width="20.919999999999998%" headers="mcps1.2.5.1.1 "><p id="p1440444312219"><a name="p1440444312219"></a><a name="p1440444312219"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="12.29%" headers="mcps1.2.5.1.2 "><p id="p1740404311216"><a name="p1740404311216"></a><a name="p1740404311216"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.02%" headers="mcps1.2.5.1.3 "><p id="p64041430217"><a name="p64041430217"></a><a name="p64041430217"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="49.769999999999996%" headers="mcps1.2.5.1.4 "><p id="p1140419436216"><a name="p1140419436216"></a><a name="p1140419436216"></a>Floatingip对外提供服务的端口号。</p>
<p id="p47430417266"><a name="p47430417266"></a><a name="p47430417266"></a>取值范围：0~65535。</p>
</td>
</tr>
<tr id="row1040494319212"><td class="cellrowborder" valign="top" width="20.919999999999998%" headers="mcps1.2.5.1.1 "><p id="p740414312213"><a name="p740414312213"></a><a name="p740414312213"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="12.29%" headers="mcps1.2.5.1.2 "><p id="p34041343627"><a name="p34041343627"></a><a name="p34041343627"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.02%" headers="mcps1.2.5.1.3 "><p id="p1440414314215"><a name="p1440414314215"></a><a name="p1440414314215"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="49.769999999999996%" headers="mcps1.2.5.1.4 "><p id="p1740415431329"><a name="p1740415431329"></a><a name="p1740415431329"></a>协议类型，目前支持TCP/UDP/ANY</p>
<p id="p2404114317211"><a name="p2404114317211"></a><a name="p2404114317211"></a>对应协议号6/17/0</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section4576293817529"></a>

响应参数如[表3](#table4946919917549)所示。

**表 3**  响应参数

<a name="table4946919917549"></a>
<table><thead align="left"><tr id="row3265693817549"><th class="cellrowborder" valign="top" width="24%" id="mcps1.2.4.1.1"><p id="p2796632617549"><a name="p2796632617549"></a><a name="p2796632617549"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="28.000000000000004%" id="mcps1.2.4.1.2"><p id="p5067993017549"><a name="p5067993017549"></a><a name="p5067993017549"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="48%" id="mcps1.2.4.1.3"><p id="p5371412517549"><a name="p5371412517549"></a><a name="p5371412517549"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row5587684317549"><td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.1 "><p id="p2973040117549"><a name="p2973040117549"></a><a name="p2973040117549"></a>dnat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.2 "><p id="p5935228017549"><a name="p5935228017549"></a><a name="p5935228017549"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="48%" headers="mcps1.2.4.1.3 "><p id="p4468272717549"><a name="p4468272717549"></a><a name="p4468272717549"></a>dnat_rule对象。详见<a href="#table1730611321529">表4</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  dnat\_rule字段说明

<a name="table1730611321529"></a>
<table><thead align="left"><tr id="row1530623213215"><th class="cellrowborder" valign="top" width="24.152415241524153%" id="mcps1.2.4.1.1"><p id="p78428281539"><a name="p78428281539"></a><a name="p78428281539"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="28.072807280728075%" id="mcps1.2.4.1.2"><p id="p6842132819314"><a name="p6842132819314"></a><a name="p6842132819314"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="47.774777477747776%" id="mcps1.2.4.1.3"><p id="p1384232814313"><a name="p1384232814313"></a><a name="p1384232814313"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row183067321216"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="p1684216281036"><a name="p1684216281036"></a><a name="p1684216281036"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="p1884242812310"><a name="p1884242812310"></a><a name="p1884242812310"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="p08422281337"><a name="p08422281337"></a><a name="p08422281337"></a>DNAT规则的id。</p>
</td>
</tr>
<tr id="row530610328215"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="p10842228633"><a name="p10842228633"></a><a name="p10842228633"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="p1284214286314"><a name="p1284214286314"></a><a name="p1284214286314"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="p1842172811317"><a name="p1842172811317"></a><a name="p1842172811317"></a>项目的ID。</p>
</td>
</tr>
<tr id="row1230612322216"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="p68422281533"><a name="p68422281533"></a><a name="p68422281533"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="p7842028439"><a name="p7842028439"></a><a name="p7842028439"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="p188422286314"><a name="p188422286314"></a><a name="p188422286314"></a>所属NAT网关的id。</p>
</td>
</tr>
<tr id="row93061232920"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="p18429281134"><a name="p18429281134"></a><a name="p18429281134"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="p19842152810314"><a name="p19842152810314"></a><a name="p19842152810314"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="p145561716582"><a name="p145561716582"></a><a name="p145561716582"></a>虚拟机或者裸机的Port ID，在VPC场景时使用此参数，与private_ip参数二选一。</p>
</td>
</tr>
<tr id="row93061325220"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="p384216281635"><a name="p384216281635"></a><a name="p384216281635"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="p1384220280311"><a name="p1384220280311"></a><a name="p1384220280311"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="p1247121916108"><a name="p1247121916108"></a><a name="p1247121916108"></a>用户私有IP地址，例如专线连接的私有云地址，</p>
<p id="p192471019141012"><a name="p192471019141012"></a><a name="p192471019141012"></a>在专线场景时使用此参数，与port_id参数二选一。</p>
</td>
</tr>
<tr id="row930619322026"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="p1984218280319"><a name="p1984218280319"></a><a name="p1984218280319"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="p11842928334"><a name="p11842928334"></a><a name="p11842928334"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="p284210281312"><a name="p284210281312"></a><a name="p284210281312"></a>虚拟机或者裸机对外提供服务的协议端口号。</p>
</td>
</tr>
<tr id="row0306133219211"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="p1184216281632"><a name="p1184216281632"></a><a name="p1184216281632"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="p1484210288313"><a name="p1484210288313"></a><a name="p1484210288313"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="p384214281237"><a name="p384214281237"></a><a name="p384214281237"></a>弹性公网IP的id。</p>
</td>
</tr>
<tr id="row1530611323214"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="p745117426320"><a name="p745117426320"></a><a name="p745117426320"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="p545119422037"><a name="p545119422037"></a><a name="p545119422037"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="p12451642538"><a name="p12451642538"></a><a name="p12451642538"></a>弹性公网IP的IP地址。</p>
</td>
</tr>
<tr id="row1130693214212"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="p245164217314"><a name="p245164217314"></a><a name="p245164217314"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="p134512421939"><a name="p134512421939"></a><a name="p134512421939"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="p16451144211314"><a name="p16451144211314"></a><a name="p16451144211314"></a>Floatingip对外提供服务的端口号。</p>
</td>
</tr>
<tr id="row530618321326"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="p12451342037"><a name="p12451342037"></a><a name="p12451342037"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="p74515424310"><a name="p74515424310"></a><a name="p74515424310"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="p74511242439"><a name="p74511242439"></a><a name="p74511242439"></a>协议类型，目前支持TCP/UDP/ANY</p>
<p id="p1445110421435"><a name="p1445110421435"></a><a name="p1445110421435"></a>对应协议号6/17/0</p>
</td>
</tr>
<tr id="row1630620322219"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="p1445104217312"><a name="p1445104217312"></a><a name="p1445104217312"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="p124515425318"><a name="p124515425318"></a><a name="p124515425318"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><a name="ul2045134211310"></a><a name="ul2045134211310"></a><ul id="ul2045134211310"><li>功能说明：DNAT规则的状态。</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="row14306173212214"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="p945116428311"><a name="p945116428311"></a><a name="p945116428311"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="p1764614265487"><a name="p1764614265487"></a><a name="p1764614265487"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><a name="ul71858556358"></a><a name="ul71858556358"></a><ul id="ul71858556358"><li>解冻/冻结状态。</li><li>取值范围：<a name="ul11838172814409"></a><a name="ul11838172814409"></a><ul id="ul11838172814409"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="row143061032627"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="p184511342035"><a name="p184511342035"></a><a name="p184511342035"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="p145144217316"><a name="p145144217316"></a><a name="p145144217316"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><a name="ul1145164214319"></a><a name="ul1145164214319"></a><ul id="ul1145164214319"><li>DNAT规则的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</li></ul>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section956164017620"></a>

-   请求样例
    1.  创建指定端口的规则

        ```
        POST https://{Endpoint}/v2.0/dnat_rules
        {
            "dnat_rule": {
                "floating_ip_id": "bf99c679-9f41-4dac-8513-9c9228e713e1",
                "nat_gateway_id": "cda3a125-2406-456c-a11f-598e10578541",
                "port_id": "9a469561-daac-4c94-88f5-39366e5ea193",
                "internal_service_port": 993,
                "protocol": "tcp",
                "external_service_port": 242
            }
        }
        ```

    1.  创建all port类型的规则。

        ```
        POST https://{Endpoint}/v2.0/dnat_rules
        {
            "dnat_rule": {
                "floating_ip_id": "Cf99c679-9f41-4dac-8513-9c9228e713e1",
                "nat_gateway_id": "Dda3a125-2406-456c-a11f-598e10578541",
                "private_ip": "192.168.1.100",
                "internal_service_port": 0,
                "protocol": "any",
                "external_service_port": 0
            }
        }
        ```



-   响应样例
    1.  创建指定端口的规则的响应

        ```
        {
            "dnat_rule": {
                "floating_ip_id": "bf99c679-9f41-4dac-8513-9c9228e713e1",
                "status": "ACTIVE",
                "nat_gateway_id": "cda3a125-2406-456c-a11f-598e10578541",
                "admin_state_up": true,
                "port_id": "9a469561-daac-4c94-88f5-39366e5ea193",
                "internal_service_port": 993,
                "protocol": "tcp",
                "tenant_id": "abc",
                "created_at": "2017-11-15 15:44:42.595173",
                "id": "79195d50-0271-41f1-bded-4c089b2502ff",
                "floating_ip_address": "5.21.11.226",
                "external_service_port": 242,
                "private_ip": ""
            }
        }
        ```

    2.  创建all port类型的规则的响应

        ```
        {
            "dnat_rule": {
                "floating_ip_id": "cf99c679-9f41-4dac-8513-9c9228e713e1",
                "status": "ACTIVE",
                "nat_gateway_id": "dda3a125-2406-456c-a11f-598e10578541",
                "admin_state_up": true,
                "private_ip": "192.168.1.100",
                "internal_service_port": 0,
                "protocol": "any",
                "tenant_id": "abc",
                "created_at": "2017-11-15 15:44:42.595173",
                "id": "79195d50-0271-41f1-bded-4c089b2502ff",
                "floating_ip_address": "5.21.11.227",
                "external_service_port": 0
            }
        }
        ```



## 状态码<a name="section5446226317959"></a>

请参考[状态码](状态码.md)。

