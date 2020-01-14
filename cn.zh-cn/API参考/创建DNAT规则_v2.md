# 创建DNAT规则<a name="nat_apiv2_0017"></a>

## 功能介绍<a name="zh-cn_topic_0168797276_section2213133217038"></a>

创建DNAT规则。

>![](public_sys-resources/icon-note.gif) **说明：**   
>创建规则时，要求网关状态status = "ACTIVE"，要求网关管理员状态admin\_state\_up = True。port\_id和private\_ip不能同时生效。对于all port类型的规则，要求internal\_service\_port = 0，external\_service\_port = 0，protocol = ANY.  

## URI<a name="zh-cn_topic_0168797276_section2631225217131"></a>

POST /v2/\{project\_id\}/dnat\_rules

**表 1**  参数说明

<a name="zh-cn_topic_0168797276_table12336194004817"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797276_row14337540164818"><th class="cellrowborder" valign="top" width="23.56%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797276_p16239411480"><a name="zh-cn_topic_0168797276_p16239411480"></a><a name="zh-cn_topic_0168797276_p16239411480"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.66%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797276_p18623114184813"><a name="zh-cn_topic_0168797276_p18623114184813"></a><a name="zh-cn_topic_0168797276_p18623114184813"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.65%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797276_p1328082133316"><a name="zh-cn_topic_0168797276_p1328082133316"></a><a name="zh-cn_topic_0168797276_p1328082133316"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.13%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797276_p4623141144812"><a name="zh-cn_topic_0168797276_p4623141144812"></a><a name="zh-cn_topic_0168797276_p4623141144812"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797276_row13337740104817"><td class="cellrowborder" valign="top" width="23.56%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797276_p1862324118488"><a name="zh-cn_topic_0168797276_p1862324118488"></a><a name="zh-cn_topic_0168797276_p1862324118488"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.66%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797276_p4623134119487"><a name="zh-cn_topic_0168797276_p4623134119487"></a><a name="zh-cn_topic_0168797276_p4623134119487"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797276_p6280182110334"><a name="zh-cn_topic_0168797276_p6280182110334"></a><a name="zh-cn_topic_0168797276_p6280182110334"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.13%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797276_p66231541124819"><a name="zh-cn_topic_0168797276_p66231541124819"></a><a name="zh-cn_topic_0168797276_p66231541124819"></a>项目ID。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0168797276_section1572764517510"></a>

请求参数如[表2](#zh-cn_topic_0168797276_table19385203615518)所示。

**表 2**  请求参数

<a name="zh-cn_topic_0168797276_table19385203615518"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797276_row7697336175113"><th class="cellrowborder" valign="top" width="22.85771422857714%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797276_p969713363516"><a name="zh-cn_topic_0168797276_p969713363516"></a><a name="zh-cn_topic_0168797276_p969713363516"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.64913508649135%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797276_p1269717362514"><a name="zh-cn_topic_0168797276_p1269717362514"></a><a name="zh-cn_topic_0168797276_p1269717362514"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.03869613038696%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797276_p269717363519"><a name="zh-cn_topic_0168797276_p269717363519"></a><a name="zh-cn_topic_0168797276_p269717363519"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.45445455454454%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797276_p176971936105117"><a name="zh-cn_topic_0168797276_p176971936105117"></a><a name="zh-cn_topic_0168797276_p176971936105117"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797276_row4697436175118"><td class="cellrowborder" valign="top" width="22.85771422857714%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797276_p96971336105112"><a name="zh-cn_topic_0168797276_p96971336105112"></a><a name="zh-cn_topic_0168797276_p96971336105112"></a>dnat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="8.64913508649135%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797276_p7697436175113"><a name="zh-cn_topic_0168797276_p7697436175113"></a><a name="zh-cn_topic_0168797276_p7697436175113"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.03869613038696%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797276_p143167141570"><a name="zh-cn_topic_0168797276_p143167141570"></a><a name="zh-cn_topic_0168797276_p143167141570"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.45445455454454%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797276_p14697113614518"><a name="zh-cn_topic_0168797276_p14697113614518"></a><a name="zh-cn_topic_0168797276_p14697113614518"></a>dnat_rule对象。请参考<a href="#zh-cn_topic_0168797276_table132796437212">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  dnat\_rule字段说明

<a name="zh-cn_topic_0168797276_table132796437212"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797276_row184049431027"><th class="cellrowborder" valign="top" width="22.57%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797276_p14043431726"><a name="zh-cn_topic_0168797276_p14043431726"></a><a name="zh-cn_topic_0168797276_p14043431726"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.649999999999999%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797276_p154049430210"><a name="zh-cn_topic_0168797276_p154049430210"></a><a name="zh-cn_topic_0168797276_p154049430210"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.9%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797276_p1740416433219"><a name="zh-cn_topic_0168797276_p1740416433219"></a><a name="zh-cn_topic_0168797276_p1740416433219"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.879999999999995%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797276_p240420437215"><a name="zh-cn_topic_0168797276_p240420437215"></a><a name="zh-cn_topic_0168797276_p240420437215"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797276_row134041433214"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797276_p164043431129"><a name="zh-cn_topic_0168797276_p164043431129"></a><a name="zh-cn_topic_0168797276_p164043431129"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797276_p1140424312213"><a name="zh-cn_topic_0168797276_p1140424312213"></a><a name="zh-cn_topic_0168797276_p1140424312213"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797276_p8404443921"><a name="zh-cn_topic_0168797276_p8404443921"></a><a name="zh-cn_topic_0168797276_p8404443921"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797276_p1440494313213"><a name="zh-cn_topic_0168797276_p1440494313213"></a><a name="zh-cn_topic_0168797276_p1440494313213"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row040412436218"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797276_p19404204314213"><a name="zh-cn_topic_0168797276_p19404204314213"></a><a name="zh-cn_topic_0168797276_p19404204314213"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797276_p154048432027"><a name="zh-cn_topic_0168797276_p154048432027"></a><a name="zh-cn_topic_0168797276_p154048432027"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797276_p540414431823"><a name="zh-cn_topic_0168797276_p540414431823"></a><a name="zh-cn_topic_0168797276_p540414431823"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797276_p13404243429"><a name="zh-cn_topic_0168797276_p13404243429"></a><a name="zh-cn_topic_0168797276_p13404243429"></a>虚拟机或者裸机的Port ID，与private_ip参数二选一。获取虚拟机Port ID的方法请参考<a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0077845908.html" target="_blank" rel="noopener noreferrer">查询云服务器网卡信息</a>，获取裸机Port ID的方法请参考<a href="https://support.huaweicloud.com/api-bms/zh-cn_topic_0053158696.html" target="_blank" rel="noopener noreferrer">查询裸金属服务器IP地址</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row14041643528"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797276_p740415432025"><a name="zh-cn_topic_0168797276_p740415432025"></a><a name="zh-cn_topic_0168797276_p740415432025"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797276_p12404194314216"><a name="zh-cn_topic_0168797276_p12404194314216"></a><a name="zh-cn_topic_0168797276_p12404194314216"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797276_p184045434218"><a name="zh-cn_topic_0168797276_p184045434218"></a><a name="zh-cn_topic_0168797276_p184045434218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797276_p84041843221"><a name="zh-cn_topic_0168797276_p84041843221"></a><a name="zh-cn_topic_0168797276_p84041843221"></a>用户私有IP地址，例如专线连接的私有云地址，与port_id参数二选一。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row16404204313220"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797276_p5404144313210"><a name="zh-cn_topic_0168797276_p5404144313210"></a><a name="zh-cn_topic_0168797276_p5404144313210"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797276_p64041431726"><a name="zh-cn_topic_0168797276_p64041431726"></a><a name="zh-cn_topic_0168797276_p64041431726"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797276_p12380554155211"><a name="zh-cn_topic_0168797276_p12380554155211"></a><a name="zh-cn_topic_0168797276_p12380554155211"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797276_p1740419431628"><a name="zh-cn_topic_0168797276_p1740419431628"></a><a name="zh-cn_topic_0168797276_p1740419431628"></a>虚拟机或者裸机对外提供服务的协议端口号。请参考<a href="https://support.huaweicloud.com/natgateway_faq/zh-cn_topic_0115901776.html" target="_blank" rel="noopener noreferrer">哪些端口无法无法访问</a>。</p>
<p id="zh-cn_topic_0168797276_p1513213291913"><a name="zh-cn_topic_0168797276_p1513213291913"></a><a name="zh-cn_topic_0168797276_p1513213291913"></a>取值范围：0~65535。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row14404174310215"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797276_p19404343926"><a name="zh-cn_topic_0168797276_p19404343926"></a><a name="zh-cn_topic_0168797276_p19404343926"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797276_p144048432217"><a name="zh-cn_topic_0168797276_p144048432217"></a><a name="zh-cn_topic_0168797276_p144048432217"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797276_p240484314213"><a name="zh-cn_topic_0168797276_p240484314213"></a><a name="zh-cn_topic_0168797276_p240484314213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797276_p1404343021"><a name="zh-cn_topic_0168797276_p1404343021"></a><a name="zh-cn_topic_0168797276_p1404343021"></a>弹性公网IP的id。获取弹性公网IP的id的方法请参考<a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090598.html" target="_blank" rel="noopener noreferrer">查询弹性公网IP列表</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row74041243421"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797276_p1440444312219"><a name="zh-cn_topic_0168797276_p1440444312219"></a><a name="zh-cn_topic_0168797276_p1440444312219"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797276_p1740404311216"><a name="zh-cn_topic_0168797276_p1740404311216"></a><a name="zh-cn_topic_0168797276_p1740404311216"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797276_p19729165665215"><a name="zh-cn_topic_0168797276_p19729165665215"></a><a name="zh-cn_topic_0168797276_p19729165665215"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797276_p1140419436216"><a name="zh-cn_topic_0168797276_p1140419436216"></a><a name="zh-cn_topic_0168797276_p1140419436216"></a>Floatingip对外提供服务的端口号。请参考<a href="https://support.huaweicloud.com/natgateway_faq/zh-cn_topic_0115901776.html" target="_blank" rel="noopener noreferrer">哪些端口无法无法访问</a>。</p>
<p id="zh-cn_topic_0168797276_p19475436235"><a name="zh-cn_topic_0168797276_p19475436235"></a><a name="zh-cn_topic_0168797276_p19475436235"></a>取值范围：0~65535。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row1040494319212"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797276_p740414312213"><a name="zh-cn_topic_0168797276_p740414312213"></a><a name="zh-cn_topic_0168797276_p740414312213"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797276_p34041343627"><a name="zh-cn_topic_0168797276_p34041343627"></a><a name="zh-cn_topic_0168797276_p34041343627"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797276_p1440414314215"><a name="zh-cn_topic_0168797276_p1440414314215"></a><a name="zh-cn_topic_0168797276_p1440414314215"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797276_p1740415431329"><a name="zh-cn_topic_0168797276_p1740415431329"></a><a name="zh-cn_topic_0168797276_p1740415431329"></a>协议类型，目前支持TCP/tcp、UDP/udp、ANY/any。</p>
<p id="zh-cn_topic_0168797276_p2404114317211"><a name="zh-cn_topic_0168797276_p2404114317211"></a><a name="zh-cn_topic_0168797276_p2404114317211"></a>对应协议号6、17、0。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row11404104315210"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797276_p1540419434218"><a name="zh-cn_topic_0168797276_p1540419434218"></a><a name="zh-cn_topic_0168797276_p1540419434218"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797276_p154049431822"><a name="zh-cn_topic_0168797276_p154049431822"></a><a name="zh-cn_topic_0168797276_p154049431822"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797276_p114041143427"><a name="zh-cn_topic_0168797276_p114041143427"></a><a name="zh-cn_topic_0168797276_p114041143427"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797276_p2040414436212"><a name="zh-cn_topic_0168797276_p2040414436212"></a><a name="zh-cn_topic_0168797276_p2040414436212"></a>DNAT规则的描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row143028138507"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797276_p4500172416506"><a name="zh-cn_topic_0168797276_p4500172416506"></a><a name="zh-cn_topic_0168797276_p4500172416506"></a>internal_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797276_p205001824185015"><a name="zh-cn_topic_0168797276_p205001824185015"></a><a name="zh-cn_topic_0168797276_p205001824185015"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797276_p15500192435011"><a name="zh-cn_topic_0168797276_p15500192435011"></a><a name="zh-cn_topic_0168797276_p15500192435011"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797276_p145009241508"><a name="zh-cn_topic_0168797276_p145009241508"></a><a name="zh-cn_topic_0168797276_p145009241508"></a>虚拟机或者裸机对外提供服务的协议端口号范围。</p>
<a name="zh-cn_topic_0168797276_ul165008243508"></a><a name="zh-cn_topic_0168797276_ul165008243508"></a><ul id="zh-cn_topic_0168797276_ul165008243508"><li>功能说明：该端口范围与external _service_port_range按顺序实现1:1映射。</li><li>取值范围：1~65535。</li><li>约束：只能以’-’字符连接端口范围。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row20102117125013"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797276_p150118248505"><a name="zh-cn_topic_0168797276_p150118248505"></a><a name="zh-cn_topic_0168797276_p150118248505"></a>external_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797276_p1550120240502"><a name="zh-cn_topic_0168797276_p1550120240502"></a><a name="zh-cn_topic_0168797276_p1550120240502"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797276_p125011424145010"><a name="zh-cn_topic_0168797276_p125011424145010"></a><a name="zh-cn_topic_0168797276_p125011424145010"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797276_p13501122475019"><a name="zh-cn_topic_0168797276_p13501122475019"></a><a name="zh-cn_topic_0168797276_p13501122475019"></a>Floatingip对外提供服务的端口号范围。</p>
<a name="zh-cn_topic_0168797276_ul6501172414509"></a><a name="zh-cn_topic_0168797276_ul6501172414509"></a><ul id="zh-cn_topic_0168797276_ul6501172414509"><li>功能说明：该端口范围与internal _service_port_range按顺序实现1:1映射。</li><li>取值范围：1~65535。</li><li>约束：只能以’-’字符连接端口范围。</li></ul>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="zh-cn_topic_0168797276_section4576293817529"></a>

响应参数如[表4](#zh-cn_topic_0168797276_table4946919917549)所示。

**表 4**  响应参数

<a name="zh-cn_topic_0168797276_table4946919917549"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797276_row3265693817549"><th class="cellrowborder" valign="top" width="24%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797276_p2796632617549"><a name="zh-cn_topic_0168797276_p2796632617549"></a><a name="zh-cn_topic_0168797276_p2796632617549"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="28.000000000000004%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797276_p5067993017549"><a name="zh-cn_topic_0168797276_p5067993017549"></a><a name="zh-cn_topic_0168797276_p5067993017549"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="48%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797276_p5371412517549"><a name="zh-cn_topic_0168797276_p5371412517549"></a><a name="zh-cn_topic_0168797276_p5371412517549"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797276_row5587684317549"><td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797276_p2973040117549"><a name="zh-cn_topic_0168797276_p2973040117549"></a><a name="zh-cn_topic_0168797276_p2973040117549"></a>dnat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797276_p5935228017549"><a name="zh-cn_topic_0168797276_p5935228017549"></a><a name="zh-cn_topic_0168797276_p5935228017549"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="48%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797276_p4468272717549"><a name="zh-cn_topic_0168797276_p4468272717549"></a><a name="zh-cn_topic_0168797276_p4468272717549"></a>dnat_rule对象。请参考<a href="#zh-cn_topic_0168797276_table1730611321529">表5</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 5**  dnat\_rule字段说明

<a name="zh-cn_topic_0168797276_table1730611321529"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797276_row1530623213215"><th class="cellrowborder" valign="top" width="24.152415241524153%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797276_p78428281539"><a name="zh-cn_topic_0168797276_p78428281539"></a><a name="zh-cn_topic_0168797276_p78428281539"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="28.072807280728075%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797276_p6842132819314"><a name="zh-cn_topic_0168797276_p6842132819314"></a><a name="zh-cn_topic_0168797276_p6842132819314"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="47.774777477747776%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797276_p1384232814313"><a name="zh-cn_topic_0168797276_p1384232814313"></a><a name="zh-cn_topic_0168797276_p1384232814313"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797276_row183067321216"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797276_p1684216281036"><a name="zh-cn_topic_0168797276_p1684216281036"></a><a name="zh-cn_topic_0168797276_p1684216281036"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797276_p1884242812310"><a name="zh-cn_topic_0168797276_p1884242812310"></a><a name="zh-cn_topic_0168797276_p1884242812310"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797276_p08422281337"><a name="zh-cn_topic_0168797276_p08422281337"></a><a name="zh-cn_topic_0168797276_p08422281337"></a>DNAT规则的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row530610328215"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797276_p10842228633"><a name="zh-cn_topic_0168797276_p10842228633"></a><a name="zh-cn_topic_0168797276_p10842228633"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797276_p1284214286314"><a name="zh-cn_topic_0168797276_p1284214286314"></a><a name="zh-cn_topic_0168797276_p1284214286314"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797276_p1842172811317"><a name="zh-cn_topic_0168797276_p1842172811317"></a><a name="zh-cn_topic_0168797276_p1842172811317"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row1230612322216"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797276_p68422281533"><a name="zh-cn_topic_0168797276_p68422281533"></a><a name="zh-cn_topic_0168797276_p68422281533"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797276_p7842028439"><a name="zh-cn_topic_0168797276_p7842028439"></a><a name="zh-cn_topic_0168797276_p7842028439"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797276_p188422286314"><a name="zh-cn_topic_0168797276_p188422286314"></a><a name="zh-cn_topic_0168797276_p188422286314"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row93061232920"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797276_p18429281134"><a name="zh-cn_topic_0168797276_p18429281134"></a><a name="zh-cn_topic_0168797276_p18429281134"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797276_p19842152810314"><a name="zh-cn_topic_0168797276_p19842152810314"></a><a name="zh-cn_topic_0168797276_p19842152810314"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797276_p9168847174116"><a name="zh-cn_topic_0168797276_p9168847174116"></a><a name="zh-cn_topic_0168797276_p9168847174116"></a>虚拟机或者裸机的Port ID，与private_ip参数二选一。获取虚拟机Port ID的方法请参考<a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0077845908.html" target="_blank" rel="noopener noreferrer">查询云服务器网卡信息</a>，获取裸机Port ID的方法请参考<a href="https://support.huaweicloud.com/api-bms/zh-cn_topic_0053158696.html" target="_blank" rel="noopener noreferrer">查询裸金属服务器IP地址</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row93061325220"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797276_p384216281635"><a name="zh-cn_topic_0168797276_p384216281635"></a><a name="zh-cn_topic_0168797276_p384216281635"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797276_p1384220280311"><a name="zh-cn_topic_0168797276_p1384220280311"></a><a name="zh-cn_topic_0168797276_p1384220280311"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797276_p1884215284318"><a name="zh-cn_topic_0168797276_p1884215284318"></a><a name="zh-cn_topic_0168797276_p1884215284318"></a>用户私有IP地址，例如专线连接的私有云地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row930619322026"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797276_p1984218280319"><a name="zh-cn_topic_0168797276_p1984218280319"></a><a name="zh-cn_topic_0168797276_p1984218280319"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797276_p81061737537"><a name="zh-cn_topic_0168797276_p81061737537"></a><a name="zh-cn_topic_0168797276_p81061737537"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797276_p284210281312"><a name="zh-cn_topic_0168797276_p284210281312"></a><a name="zh-cn_topic_0168797276_p284210281312"></a>虚拟机或者裸机对外提供服务的协议端口号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row0306133219211"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797276_p1184216281632"><a name="zh-cn_topic_0168797276_p1184216281632"></a><a name="zh-cn_topic_0168797276_p1184216281632"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797276_p1484210288313"><a name="zh-cn_topic_0168797276_p1484210288313"></a><a name="zh-cn_topic_0168797276_p1484210288313"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797276_p384214281237"><a name="zh-cn_topic_0168797276_p384214281237"></a><a name="zh-cn_topic_0168797276_p384214281237"></a>弹性公网IP的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row1530611323214"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797276_p745117426320"><a name="zh-cn_topic_0168797276_p745117426320"></a><a name="zh-cn_topic_0168797276_p745117426320"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797276_p545119422037"><a name="zh-cn_topic_0168797276_p545119422037"></a><a name="zh-cn_topic_0168797276_p545119422037"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797276_p12451642538"><a name="zh-cn_topic_0168797276_p12451642538"></a><a name="zh-cn_topic_0168797276_p12451642538"></a>弹性公网IP的IP地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row1130693214212"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797276_p245164217314"><a name="zh-cn_topic_0168797276_p245164217314"></a><a name="zh-cn_topic_0168797276_p245164217314"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797276_p2173962537"><a name="zh-cn_topic_0168797276_p2173962537"></a><a name="zh-cn_topic_0168797276_p2173962537"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797276_p16451144211314"><a name="zh-cn_topic_0168797276_p16451144211314"></a><a name="zh-cn_topic_0168797276_p16451144211314"></a>Floatingip对外提供服务的端口号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row530618321326"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797276_p12451342037"><a name="zh-cn_topic_0168797276_p12451342037"></a><a name="zh-cn_topic_0168797276_p12451342037"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797276_p74515424310"><a name="zh-cn_topic_0168797276_p74515424310"></a><a name="zh-cn_topic_0168797276_p74515424310"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797276_p74511242439"><a name="zh-cn_topic_0168797276_p74511242439"></a><a name="zh-cn_topic_0168797276_p74511242439"></a>协议类型，目前支持TCP、UDP、ANY。</p>
<p id="zh-cn_topic_0168797276_p1445110421435"><a name="zh-cn_topic_0168797276_p1445110421435"></a><a name="zh-cn_topic_0168797276_p1445110421435"></a>对应协议号6、17、0。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row33063326217"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797276_p1645114421933"><a name="zh-cn_topic_0168797276_p1645114421933"></a><a name="zh-cn_topic_0168797276_p1645114421933"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797276_p44518421316"><a name="zh-cn_topic_0168797276_p44518421316"></a><a name="zh-cn_topic_0168797276_p44518421316"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797276_p9451114220316"><a name="zh-cn_topic_0168797276_p9451114220316"></a><a name="zh-cn_topic_0168797276_p9451114220316"></a>DNAT规则的描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row1630620322219"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797276_p1445104217312"><a name="zh-cn_topic_0168797276_p1445104217312"></a><a name="zh-cn_topic_0168797276_p1445104217312"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797276_p124515425318"><a name="zh-cn_topic_0168797276_p124515425318"></a><a name="zh-cn_topic_0168797276_p124515425318"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797276_ul2045134211310"></a><a name="zh-cn_topic_0168797276_ul2045134211310"></a><ul id="zh-cn_topic_0168797276_ul2045134211310"><li>功能说明：DNAT规则的状态。</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row14306173212214"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797276_p945116428311"><a name="zh-cn_topic_0168797276_p945116428311"></a><a name="zh-cn_topic_0168797276_p945116428311"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797276_p10451134220314"><a name="zh-cn_topic_0168797276_p10451134220314"></a><a name="zh-cn_topic_0168797276_p10451134220314"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797276_ul71858556358"></a><a name="zh-cn_topic_0168797276_ul71858556358"></a><ul id="zh-cn_topic_0168797276_ul71858556358"><li>解冻/冻结状态。</li><li>取值范围：<a name="zh-cn_topic_0168797276_ul11838172814409"></a><a name="zh-cn_topic_0168797276_ul11838172814409"></a><ul id="zh-cn_topic_0168797276_ul11838172814409"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row143061032627"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797276_p184511342035"><a name="zh-cn_topic_0168797276_p184511342035"></a><a name="zh-cn_topic_0168797276_p184511342035"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797276_p145144217316"><a name="zh-cn_topic_0168797276_p145144217316"></a><a name="zh-cn_topic_0168797276_p145144217316"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797276_ul1145164214319"></a><a name="zh-cn_topic_0168797276_ul1145164214319"></a><ul id="zh-cn_topic_0168797276_ul1145164214319"><li>DNAT规则的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row10727105612546"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797276_p1320696125519"><a name="zh-cn_topic_0168797276_p1320696125519"></a><a name="zh-cn_topic_0168797276_p1320696125519"></a>internal_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797276_p520615614559"><a name="zh-cn_topic_0168797276_p520615614559"></a><a name="zh-cn_topic_0168797276_p520615614559"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797276_p102060625518"><a name="zh-cn_topic_0168797276_p102060625518"></a><a name="zh-cn_topic_0168797276_p102060625518"></a>虚拟机或者裸机对外提供服务的协议端口号范围。</p>
<a name="zh-cn_topic_0168797276_ul1220686115515"></a><a name="zh-cn_topic_0168797276_ul1220686115515"></a><ul id="zh-cn_topic_0168797276_ul1220686115515"><li>功能说明：该端口范围与external _service_port_range按顺序实现1:1映射。</li><li>取值范围：1~65535。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797276_row14728135605411"><td class="cellrowborder" valign="top" width="24.152415241524153%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797276_p1420636165519"><a name="zh-cn_topic_0168797276_p1420636165519"></a><a name="zh-cn_topic_0168797276_p1420636165519"></a>external_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="28.072807280728075%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797276_p2206868553"><a name="zh-cn_topic_0168797276_p2206868553"></a><a name="zh-cn_topic_0168797276_p2206868553"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797276_p220614655512"><a name="zh-cn_topic_0168797276_p220614655512"></a><a name="zh-cn_topic_0168797276_p220614655512"></a>Floatingip对外提供服务的端口号范围。</p>
<a name="zh-cn_topic_0168797276_ul22064665519"></a><a name="zh-cn_topic_0168797276_ul22064665519"></a><ul id="zh-cn_topic_0168797276_ul22064665519"><li>功能说明：该端口范围与internal _service_port_range按顺序实现1:1映射。</li><li>取值范围：1~65535。</li></ul>
</td>
</tr>
</tbody>
</table>

## 示例<a name="zh-cn_topic_0168797276_section956164017620"></a>

-   请求样例
    1.  创建指定端口的规则

        ```
        POST https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/dnat_rules
        { 
             "dnat_rule": { 
                 "floating_ip_id": "bf99c679-9f41-4dac-8513-9c9228e713e1", 
                 "nat_gateway_id": "cda3a125-2406-456c-a11f-598e10578541", 
                 "port_id": "9a469561-daac-4c94-88f5-39366e5ea193", 
                 "internal_service_port": 993, 
                 "protocol": "tcp", 
                 "external_service_port": 242, 
                 "description": "my dnat rule 01"
             } 
         }
        ```

    1.  创建all port类型的规则。

        ```
        POST https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/dnat_rules
        { 
             "dnat_rule": { 
                 "floating_ip_id": "Cf99c679-9f41-4dac-8513-9c9228e713e1", 
                 "nat_gateway_id": "Dda3a125-2406-456c-a11f-598e10578541", 
                 "private_ip": "192.168.1.100", 
                 "internal_service_port": 0, 
                 "protocol": "any", 
                 "external_service_port": 0, 
                 "description": "my dnat rule 01" 
             } 
         }
        ```

    2.  指定端口范围创建规则

        ```
        POST https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/dnat_rules
        { 
             "dnat_rule": { 
                 "floating_ip_id": "Cf99c679-9f41-4dac-8513-9c9228e713e1", 
                 "nat_gateway_id": "Dda3a125-2406-456c-a11f-598e10578541", 
                 "private_ip": "192.168.1.100", 
                 "internal_service_port": 0, 
                 "protocol": "tcp", 
                 "external_service_port": 0, 
                 "description": "my dnat rule 01" ,
                 "external_service_port_range":"100-200",
                 "internal_service_port_range":"100-200"
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
                 "external_service_port": 242, 
                 "floating_ip_address": "5.21.11.226",
                 "description": "my dnat rule 01" 
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
                 "external_service_port": 0, 
                 "floating_ip_address": "5.21.11.227",
                 "description": "my dnat rule 01" 
             } 
         }
        ```

    3.  指定端口范围创建规则

        ```
        { 
             "dnat_rule": { 
                 "floating_ip_id": "cf99c679-9f41-4dac-8513-9c9228e713e1", 
                 "status": "ACTIVE", 
                 "nat_gateway_id": "dda3a125-2406-456c-a11f-598e10578541", 
                 "admin_state_up": true, 
                 "private_ip": "192.168.1.100", 
                 "internal_service_port": 0, 
                 "protocol": "tcp", 
                 "tenant_id": "abc", 
                 "created_at": "2017-11-15 15:44:42.595173", 
                 "id": "79195d50-0271-41f1-bded-4c089b2502ff", 
                 "external_service_port": 0, 
                 "floating_ip_address": "5.21.11.227",
                 "description": "my dnat rule 01",
                 "internal_service_port_range":"100-200",
                 "external_service_port_range":"100-200"
             } 
         }
        ```



## 状态码<a name="zh-cn_topic_0168797276_section5446226317959"></a>

请参考[状态码](状态码.md)。

