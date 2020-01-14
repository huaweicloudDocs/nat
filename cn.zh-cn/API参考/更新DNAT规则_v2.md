# 更新DNAT规则<a name="nat_apiv2_0021"></a>

## 功能介绍<a name="zh-cn_topic_0168797296_section633825684817"></a>

更新DNAT规则。

>![](public_sys-resources/icon-note.gif) **说明：**   
>更新操作时，要求DNAT规则状态status = "ACTIVE"，要求网关管理员状态admin\_state\_up = True。port\_id和private\_ip不能同时生效。对于all port类型的规则，要求internal\_service\_port = 0，external\_service\_port = 0，protocol = ANY。  
>更新操作涉及以下字段更新时，要求这些字段必须一起更新。包括：port\_id、private\_ip、internal\_service\_port、external\_service\_port、floating\_ip\_id、protocol、internal\_service\_port\_range、external\_service\_port\_range。  

## URI<a name="zh-cn_topic_0168797296_section933875617481"></a>

PUT /v2/\{project\_id\}/dnat\_rules/\{dnat\_rule\_id\}

**表 1**  参数说明

<a name="zh-cn_topic_0168797296_table123387562484"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797296_row976065644812"><th class="cellrowborder" valign="top" width="23.24%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797296_p47601856204810"><a name="zh-cn_topic_0168797296_p47601856204810"></a><a name="zh-cn_topic_0168797296_p47601856204810"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.23%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797296_p2760185694817"><a name="zh-cn_topic_0168797296_p2760185694817"></a><a name="zh-cn_topic_0168797296_p2760185694817"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.65%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797296_p1786131974619"><a name="zh-cn_topic_0168797296_p1786131974619"></a><a name="zh-cn_topic_0168797296_p1786131974619"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="52.88%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797296_p1876095684819"><a name="zh-cn_topic_0168797296_p1876095684819"></a><a name="zh-cn_topic_0168797296_p1876095684819"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797296_row6760115624818"><td class="cellrowborder" valign="top" width="23.24%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797296_p976085610483"><a name="zh-cn_topic_0168797296_p976085610483"></a><a name="zh-cn_topic_0168797296_p976085610483"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.23%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797296_p776095664811"><a name="zh-cn_topic_0168797296_p776095664811"></a><a name="zh-cn_topic_0168797296_p776095664811"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797296_p3786419154616"><a name="zh-cn_topic_0168797296_p3786419154616"></a><a name="zh-cn_topic_0168797296_p3786419154616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.88%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797296_p9760856144817"><a name="zh-cn_topic_0168797296_p9760856144817"></a><a name="zh-cn_topic_0168797296_p9760856144817"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row87602056144817"><td class="cellrowborder" valign="top" width="23.24%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797296_p14760556194819"><a name="zh-cn_topic_0168797296_p14760556194819"></a><a name="zh-cn_topic_0168797296_p14760556194819"></a>dnat_rule_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.23%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797296_p18760145624818"><a name="zh-cn_topic_0168797296_p18760145624818"></a><a name="zh-cn_topic_0168797296_p18760145624818"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797296_p19786151994615"><a name="zh-cn_topic_0168797296_p19786151994615"></a><a name="zh-cn_topic_0168797296_p19786151994615"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.88%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797296_p376016568482"><a name="zh-cn_topic_0168797296_p376016568482"></a><a name="zh-cn_topic_0168797296_p376016568482"></a>DNAT规则的id。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0168797296_section11354175619487"></a>

请求参数如[表2](#zh-cn_topic_0168797296_table1335415654817)所示。

**表 2**  请求参数

<a name="zh-cn_topic_0168797296_table1335415654817"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797296_row1760105614813"><th class="cellrowborder" valign="top" width="21.42%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797296_p1876075620487"><a name="zh-cn_topic_0168797296_p1876075620487"></a><a name="zh-cn_topic_0168797296_p1876075620487"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.129999999999999%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797296_p137604569485"><a name="zh-cn_topic_0168797296_p137604569485"></a><a name="zh-cn_topic_0168797296_p137604569485"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.349999999999998%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797296_p14760145613485"><a name="zh-cn_topic_0168797296_p14760145613485"></a><a name="zh-cn_topic_0168797296_p14760145613485"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="53.1%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797296_p77601656164810"><a name="zh-cn_topic_0168797296_p77601656164810"></a><a name="zh-cn_topic_0168797296_p77601656164810"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797296_row076016567481"><td class="cellrowborder" valign="top" width="21.42%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797296_p276025611487"><a name="zh-cn_topic_0168797296_p276025611487"></a><a name="zh-cn_topic_0168797296_p276025611487"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.129999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797296_p16760155617489"><a name="zh-cn_topic_0168797296_p16760155617489"></a><a name="zh-cn_topic_0168797296_p16760155617489"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797296_p4760125619487"><a name="zh-cn_topic_0168797296_p4760125619487"></a><a name="zh-cn_topic_0168797296_p4760125619487"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.1%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797296_p147601356104811"><a name="zh-cn_topic_0168797296_p147601356104811"></a><a name="zh-cn_topic_0168797296_p147601356104811"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row17760156194817"><td class="cellrowborder" valign="top" width="21.42%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797296_p6760356184815"><a name="zh-cn_topic_0168797296_p6760356184815"></a><a name="zh-cn_topic_0168797296_p6760356184815"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.129999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797296_p17604568488"><a name="zh-cn_topic_0168797296_p17604568488"></a><a name="zh-cn_topic_0168797296_p17604568488"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797296_p15760155664812"><a name="zh-cn_topic_0168797296_p15760155664812"></a><a name="zh-cn_topic_0168797296_p15760155664812"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.1%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797296_p147601856124819"><a name="zh-cn_topic_0168797296_p147601856124819"></a><a name="zh-cn_topic_0168797296_p147601856124819"></a>虚拟机或者裸机的Port ID，与private_ip参数二选一。获取虚拟机Port ID的方法请参考<a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0077845908.html" target="_blank" rel="noopener noreferrer">查询云服务器网卡信息</a>，获取裸机Port ID的方法请参考<a href="https://support.huaweicloud.com/api-bms/zh-cn_topic_0053158696.html" target="_blank" rel="noopener noreferrer">查询裸金属服务器IP地址</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row1876095674814"><td class="cellrowborder" valign="top" width="21.42%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797296_p137601256104816"><a name="zh-cn_topic_0168797296_p137601256104816"></a><a name="zh-cn_topic_0168797296_p137601256104816"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="8.129999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797296_p15760185612487"><a name="zh-cn_topic_0168797296_p15760185612487"></a><a name="zh-cn_topic_0168797296_p15760185612487"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797296_p10760956114819"><a name="zh-cn_topic_0168797296_p10760956114819"></a><a name="zh-cn_topic_0168797296_p10760956114819"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.1%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797296_p3760205684818"><a name="zh-cn_topic_0168797296_p3760205684818"></a><a name="zh-cn_topic_0168797296_p3760205684818"></a>用户私有IP地址，例如专线连接的私有云地址，与port_id参数二选一。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row5760356174818"><td class="cellrowborder" valign="top" width="21.42%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797296_p1076095654810"><a name="zh-cn_topic_0168797296_p1076095654810"></a><a name="zh-cn_topic_0168797296_p1076095654810"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="8.129999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797296_p137601056174819"><a name="zh-cn_topic_0168797296_p137601056174819"></a><a name="zh-cn_topic_0168797296_p137601056174819"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797296_p17601156174813"><a name="zh-cn_topic_0168797296_p17601156174813"></a><a name="zh-cn_topic_0168797296_p17601156174813"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="53.1%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797296_p276016569489"><a name="zh-cn_topic_0168797296_p276016569489"></a><a name="zh-cn_topic_0168797296_p276016569489"></a>虚拟机或者裸机对外提供服务的协议端口号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row276010562486"><td class="cellrowborder" valign="top" width="21.42%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797296_p6760135610482"><a name="zh-cn_topic_0168797296_p6760135610482"></a><a name="zh-cn_topic_0168797296_p6760135610482"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.129999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797296_p12760175610487"><a name="zh-cn_topic_0168797296_p12760175610487"></a><a name="zh-cn_topic_0168797296_p12760175610487"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797296_p976075611489"><a name="zh-cn_topic_0168797296_p976075611489"></a><a name="zh-cn_topic_0168797296_p976075611489"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.1%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797296_p1276085617489"><a name="zh-cn_topic_0168797296_p1276085617489"></a><a name="zh-cn_topic_0168797296_p1276085617489"></a>弹性公网IP的id。获取弹性公网IP的id的方法请参考<a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090598.html" target="_blank" rel="noopener noreferrer">查询弹性公网IP列表</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row876045614484"><td class="cellrowborder" valign="top" width="21.42%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797296_p576015674811"><a name="zh-cn_topic_0168797296_p576015674811"></a><a name="zh-cn_topic_0168797296_p576015674811"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="8.129999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797296_p12760165664819"><a name="zh-cn_topic_0168797296_p12760165664819"></a><a name="zh-cn_topic_0168797296_p12760165664819"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797296_p57601156174819"><a name="zh-cn_topic_0168797296_p57601156174819"></a><a name="zh-cn_topic_0168797296_p57601156174819"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="53.1%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797296_p20760195634819"><a name="zh-cn_topic_0168797296_p20760195634819"></a><a name="zh-cn_topic_0168797296_p20760195634819"></a>Floatingip对外提供服务的端口号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row876005618487"><td class="cellrowborder" valign="top" width="21.42%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797296_p1076011562480"><a name="zh-cn_topic_0168797296_p1076011562480"></a><a name="zh-cn_topic_0168797296_p1076011562480"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="8.129999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797296_p7760135694819"><a name="zh-cn_topic_0168797296_p7760135694819"></a><a name="zh-cn_topic_0168797296_p7760135694819"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797296_p2076017563489"><a name="zh-cn_topic_0168797296_p2076017563489"></a><a name="zh-cn_topic_0168797296_p2076017563489"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.1%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797296_p1740415431329"><a name="zh-cn_topic_0168797296_p1740415431329"></a><a name="zh-cn_topic_0168797296_p1740415431329"></a>协议类型，目前支持TCP/tcp、UDP/udp、ANY/any。</p>
<p id="zh-cn_topic_0168797296_p2404114317211"><a name="zh-cn_topic_0168797296_p2404114317211"></a><a name="zh-cn_topic_0168797296_p2404114317211"></a>对应协议号6、17、0。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row1776055614480"><td class="cellrowborder" valign="top" width="21.42%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797296_p13760756134817"><a name="zh-cn_topic_0168797296_p13760756134817"></a><a name="zh-cn_topic_0168797296_p13760756134817"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="8.129999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797296_p7760205613487"><a name="zh-cn_topic_0168797296_p7760205613487"></a><a name="zh-cn_topic_0168797296_p7760205613487"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797296_p17609567487"><a name="zh-cn_topic_0168797296_p17609567487"></a><a name="zh-cn_topic_0168797296_p17609567487"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="53.1%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797296_p17603564485"><a name="zh-cn_topic_0168797296_p17603564485"></a><a name="zh-cn_topic_0168797296_p17603564485"></a>DNAT规则的描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row467214384414"><td class="cellrowborder" valign="top" width="21.42%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797296_p56908391342"><a name="zh-cn_topic_0168797296_p56908391342"></a><a name="zh-cn_topic_0168797296_p56908391342"></a>internal_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="8.129999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797296_p1069018391941"><a name="zh-cn_topic_0168797296_p1069018391941"></a><a name="zh-cn_topic_0168797296_p1069018391941"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797296_p86905391247"><a name="zh-cn_topic_0168797296_p86905391247"></a><a name="zh-cn_topic_0168797296_p86905391247"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.1%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797296_p66905399411"><a name="zh-cn_topic_0168797296_p66905399411"></a><a name="zh-cn_topic_0168797296_p66905399411"></a>虚拟机或者裸机对外提供服务的协议端口号范围。</p>
<a name="zh-cn_topic_0168797296_ul146901039349"></a><a name="zh-cn_topic_0168797296_ul146901039349"></a><ul id="zh-cn_topic_0168797296_ul146901039349"><li>功能说明：该端口范围与external _service_port_range按顺序实现1:1映射。</li><li>取值范围：1~65535。</li><li>约束：只能以’-’字符连接端口范围。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row66731438748"><td class="cellrowborder" valign="top" width="21.42%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797296_p26917395418"><a name="zh-cn_topic_0168797296_p26917395418"></a><a name="zh-cn_topic_0168797296_p26917395418"></a>external_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="8.129999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797296_p96916396410"><a name="zh-cn_topic_0168797296_p96916396410"></a><a name="zh-cn_topic_0168797296_p96916396410"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797296_p13691113913410"><a name="zh-cn_topic_0168797296_p13691113913410"></a><a name="zh-cn_topic_0168797296_p13691113913410"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.1%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797296_p46911139643"><a name="zh-cn_topic_0168797296_p46911139643"></a><a name="zh-cn_topic_0168797296_p46911139643"></a>Floatingip对外提供服务的端口号范围。</p>
<a name="zh-cn_topic_0168797296_ul969163913418"></a><a name="zh-cn_topic_0168797296_ul969163913418"></a><ul id="zh-cn_topic_0168797296_ul969163913418"><li>功能说明：该端口范围与internal _service_port_range按顺序实现1:1映射。</li><li>取值范围：1~65535。</li><li>约束：只能以’-’字符连接端口范围。</li></ul>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="zh-cn_topic_0168797296_section10401185611484"></a>

响应参数如[表3](#zh-cn_topic_0168797296_table13401145619486)所示。

**表 3**  响应参数

<a name="zh-cn_topic_0168797296_table13401145619486"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797296_row19760125624815"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797296_p11760125616482"><a name="zh-cn_topic_0168797296_p11760125616482"></a><a name="zh-cn_topic_0168797296_p11760125616482"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.48%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797296_p15760356164818"><a name="zh-cn_topic_0168797296_p15760356164818"></a><a name="zh-cn_topic_0168797296_p15760356164818"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.519999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797296_p197601056204814"><a name="zh-cn_topic_0168797296_p197601056204814"></a><a name="zh-cn_topic_0168797296_p197601056204814"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797296_row10760256134820"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797296_p376015618487"><a name="zh-cn_topic_0168797296_p376015618487"></a><a name="zh-cn_topic_0168797296_p376015618487"></a>dnat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="18.48%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797296_p13760165618484"><a name="zh-cn_topic_0168797296_p13760165618484"></a><a name="zh-cn_topic_0168797296_p13760165618484"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="61.519999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797296_p1676018567485"><a name="zh-cn_topic_0168797296_p1676018567485"></a><a name="zh-cn_topic_0168797296_p1676018567485"></a>dnat_rule对象。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  dnat\_rule字段说明

<a name="zh-cn_topic_0168797296_table1940119567484"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797296_row876055613481"><th class="cellrowborder" valign="top" width="20.49%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797296_p137606567485"><a name="zh-cn_topic_0168797296_p137606567485"></a><a name="zh-cn_topic_0168797296_p137606567485"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="17.89%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797296_p147608563484"><a name="zh-cn_topic_0168797296_p147608563484"></a><a name="zh-cn_topic_0168797296_p147608563484"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.62%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797296_p3760135615488"><a name="zh-cn_topic_0168797296_p3760135615488"></a><a name="zh-cn_topic_0168797296_p3760135615488"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797296_row47601856164820"><td class="cellrowborder" valign="top" width="20.49%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797296_p137601556124814"><a name="zh-cn_topic_0168797296_p137601556124814"></a><a name="zh-cn_topic_0168797296_p137601556124814"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797296_p876015619489"><a name="zh-cn_topic_0168797296_p876015619489"></a><a name="zh-cn_topic_0168797296_p876015619489"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797296_p14760175620486"><a name="zh-cn_topic_0168797296_p14760175620486"></a><a name="zh-cn_topic_0168797296_p14760175620486"></a>DNAT规则的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row1076019567487"><td class="cellrowborder" valign="top" width="20.49%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797296_p6760135684813"><a name="zh-cn_topic_0168797296_p6760135684813"></a><a name="zh-cn_topic_0168797296_p6760135684813"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797296_p127607562483"><a name="zh-cn_topic_0168797296_p127607562483"></a><a name="zh-cn_topic_0168797296_p127607562483"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797296_p117601056124817"><a name="zh-cn_topic_0168797296_p117601056124817"></a><a name="zh-cn_topic_0168797296_p117601056124817"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row207608569481"><td class="cellrowborder" valign="top" width="20.49%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797296_p16760456204813"><a name="zh-cn_topic_0168797296_p16760456204813"></a><a name="zh-cn_topic_0168797296_p16760456204813"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797296_p6760256104818"><a name="zh-cn_topic_0168797296_p6760256104818"></a><a name="zh-cn_topic_0168797296_p6760256104818"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797296_p57601856154813"><a name="zh-cn_topic_0168797296_p57601856154813"></a><a name="zh-cn_topic_0168797296_p57601856154813"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row8760256134810"><td class="cellrowborder" valign="top" width="20.49%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797296_p16760105634814"><a name="zh-cn_topic_0168797296_p16760105634814"></a><a name="zh-cn_topic_0168797296_p16760105634814"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797296_p1576065618488"><a name="zh-cn_topic_0168797296_p1576065618488"></a><a name="zh-cn_topic_0168797296_p1576065618488"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797296_p1776035613480"><a name="zh-cn_topic_0168797296_p1776035613480"></a><a name="zh-cn_topic_0168797296_p1776035613480"></a>虚拟机或者裸机的Port ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row57601656144812"><td class="cellrowborder" valign="top" width="20.49%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797296_p207602056154815"><a name="zh-cn_topic_0168797296_p207602056154815"></a><a name="zh-cn_topic_0168797296_p207602056154815"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797296_p1276055644819"><a name="zh-cn_topic_0168797296_p1276055644819"></a><a name="zh-cn_topic_0168797296_p1276055644819"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797296_p107601756174815"><a name="zh-cn_topic_0168797296_p107601756174815"></a><a name="zh-cn_topic_0168797296_p107601756174815"></a>用户私有IP地址，例如专线连接的私有云地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row1376075617485"><td class="cellrowborder" valign="top" width="20.49%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797296_p14760556114819"><a name="zh-cn_topic_0168797296_p14760556114819"></a><a name="zh-cn_topic_0168797296_p14760556114819"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797296_p97601056104812"><a name="zh-cn_topic_0168797296_p97601056104812"></a><a name="zh-cn_topic_0168797296_p97601056104812"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797296_p4760856194813"><a name="zh-cn_topic_0168797296_p4760856194813"></a><a name="zh-cn_topic_0168797296_p4760856194813"></a>虚拟机或者裸机对外提供服务的协议端口号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row12760125611483"><td class="cellrowborder" valign="top" width="20.49%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797296_p16760125614811"><a name="zh-cn_topic_0168797296_p16760125614811"></a><a name="zh-cn_topic_0168797296_p16760125614811"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797296_p1476085634820"><a name="zh-cn_topic_0168797296_p1476085634820"></a><a name="zh-cn_topic_0168797296_p1476085634820"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797296_p10760155654812"><a name="zh-cn_topic_0168797296_p10760155654812"></a><a name="zh-cn_topic_0168797296_p10760155654812"></a>弹性公网IP的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row776035684817"><td class="cellrowborder" valign="top" width="20.49%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797296_p1476045619488"><a name="zh-cn_topic_0168797296_p1476045619488"></a><a name="zh-cn_topic_0168797296_p1476045619488"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797296_p1176055664819"><a name="zh-cn_topic_0168797296_p1176055664819"></a><a name="zh-cn_topic_0168797296_p1176055664819"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797296_p976075618488"><a name="zh-cn_topic_0168797296_p976075618488"></a><a name="zh-cn_topic_0168797296_p976075618488"></a>弹性公网的IP地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row1876005674810"><td class="cellrowborder" valign="top" width="20.49%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797296_p17760135615485"><a name="zh-cn_topic_0168797296_p17760135615485"></a><a name="zh-cn_topic_0168797296_p17760135615485"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797296_p376016563483"><a name="zh-cn_topic_0168797296_p376016563483"></a><a name="zh-cn_topic_0168797296_p376016563483"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797296_p167601256194812"><a name="zh-cn_topic_0168797296_p167601256194812"></a><a name="zh-cn_topic_0168797296_p167601256194812"></a>Floatingip对外提供服务的端口号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row147603562489"><td class="cellrowborder" valign="top" width="20.49%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797296_p10760175664811"><a name="zh-cn_topic_0168797296_p10760175664811"></a><a name="zh-cn_topic_0168797296_p10760175664811"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797296_p19760155654812"><a name="zh-cn_topic_0168797296_p19760155654812"></a><a name="zh-cn_topic_0168797296_p19760155654812"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797296_p176017563487"><a name="zh-cn_topic_0168797296_p176017563487"></a><a name="zh-cn_topic_0168797296_p176017563487"></a>协议类型，目前支持TCP、UDP、ANY。</p>
<p id="zh-cn_topic_0168797296_p37601656194811"><a name="zh-cn_topic_0168797296_p37601656194811"></a><a name="zh-cn_topic_0168797296_p37601656194811"></a>对应协议号6、17、0。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row376015561487"><td class="cellrowborder" valign="top" width="20.49%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797296_p17760956154816"><a name="zh-cn_topic_0168797296_p17760956154816"></a><a name="zh-cn_topic_0168797296_p17760956154816"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797296_p976045674815"><a name="zh-cn_topic_0168797296_p976045674815"></a><a name="zh-cn_topic_0168797296_p976045674815"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797296_p576065664817"><a name="zh-cn_topic_0168797296_p576065664817"></a><a name="zh-cn_topic_0168797296_p576065664817"></a>DNAT规则的描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row8760556114810"><td class="cellrowborder" valign="top" width="20.49%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797296_p1976095654818"><a name="zh-cn_topic_0168797296_p1976095654818"></a><a name="zh-cn_topic_0168797296_p1976095654818"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797296_p1576015566487"><a name="zh-cn_topic_0168797296_p1576015566487"></a><a name="zh-cn_topic_0168797296_p1576015566487"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797296_ul1876035611485"></a><a name="zh-cn_topic_0168797296_ul1876035611485"></a><ul id="zh-cn_topic_0168797296_ul1876035611485"><li>功能说明：DNAT规则的状态。</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row4760556194810"><td class="cellrowborder" valign="top" width="20.49%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797296_p2076025664813"><a name="zh-cn_topic_0168797296_p2076025664813"></a><a name="zh-cn_topic_0168797296_p2076025664813"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797296_p12189161952812"><a name="zh-cn_topic_0168797296_p12189161952812"></a><a name="zh-cn_topic_0168797296_p12189161952812"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797296_ul71858556358"></a><a name="zh-cn_topic_0168797296_ul71858556358"></a><ul id="zh-cn_topic_0168797296_ul71858556358"><li>解冻/冻结状态。</li><li>取值范围：<a name="zh-cn_topic_0168797296_ul11838172814409"></a><a name="zh-cn_topic_0168797296_ul11838172814409"></a><ul id="zh-cn_topic_0168797296_ul11838172814409"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row1276085664817"><td class="cellrowborder" valign="top" width="20.49%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797296_p13760135634812"><a name="zh-cn_topic_0168797296_p13760135634812"></a><a name="zh-cn_topic_0168797296_p13760135634812"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797296_p176075612481"><a name="zh-cn_topic_0168797296_p176075612481"></a><a name="zh-cn_topic_0168797296_p176075612481"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797296_ul476005604819"></a><a name="zh-cn_topic_0168797296_ul476005604819"></a><ul id="zh-cn_topic_0168797296_ul476005604819"><li>DNAT规则的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row71551544954"><td class="cellrowborder" valign="top" width="20.49%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797296_p7324134513512"><a name="zh-cn_topic_0168797296_p7324134513512"></a><a name="zh-cn_topic_0168797296_p7324134513512"></a>internal_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797296_p17324194514512"><a name="zh-cn_topic_0168797296_p17324194514512"></a><a name="zh-cn_topic_0168797296_p17324194514512"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797296_p153244451555"><a name="zh-cn_topic_0168797296_p153244451555"></a><a name="zh-cn_topic_0168797296_p153244451555"></a>虚拟机或者裸机对外提供服务的协议端口号范围。</p>
<a name="zh-cn_topic_0168797296_ul13241045155"></a><a name="zh-cn_topic_0168797296_ul13241045155"></a><ul id="zh-cn_topic_0168797296_ul13241045155"><li>功能说明：该端口范围与external _service_port_range按顺序实现1:1映射。</li><li>取值范围：1~65535。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797296_row141554442052"><td class="cellrowborder" valign="top" width="20.49%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797296_p1732411451358"><a name="zh-cn_topic_0168797296_p1732411451358"></a><a name="zh-cn_topic_0168797296_p1732411451358"></a>external_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797296_p14324164510519"><a name="zh-cn_topic_0168797296_p14324164510519"></a><a name="zh-cn_topic_0168797296_p14324164510519"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797296_p183247457517"><a name="zh-cn_topic_0168797296_p183247457517"></a><a name="zh-cn_topic_0168797296_p183247457517"></a>Floatingip对外提供服务的端口号范围。</p>
<a name="zh-cn_topic_0168797296_ul163249455519"></a><a name="zh-cn_topic_0168797296_ul163249455519"></a><ul id="zh-cn_topic_0168797296_ul163249455519"><li>功能说明：该端口范围与internal _service_port_range按顺序实现1:1映射。</li><li>取值范围：1~65535。</li></ul>
</td>
</tr>
</tbody>
</table>

## 示例<a name="zh-cn_topic_0168797296_section2046325618486"></a>

-   请求样例
    1.  更新指定端口的规则。

        ```
        PUT https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/dnat_rules/79195d50-0271-41f1-bded-4c089b2502ff
        { 
             "dnat_rule": { 
                 "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
                 "floating_ip_id": "cf99c679-9f41-4dac-8513-9c9228e713e1", 
                 "port_id": "9a469561-daac-4c94-88f5-39366e5ea193", 
                 "internal_service_port": 993, 
                 "protocol": "tcp", 
                 "external_service_port": 242, 
                 "description": "my dnat rule 01"
             } 
         }
        ```

    2.  更新all port类型的规则。

        ```
        PUT https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/dnat_rules/79195d50-0271-41f1-bded-4c089b2502ff
        { 
             "dnat_rule": { 
                 "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
                 "floating_ip_id": "bf99c679-9f41-4dac-8513-9c9228e713e1",
                 "private_ip": "192.168.1.100", 
                 "internal_service_port": 0, 
                 "protocol": "any", 
                 "external_service_port": 0, 
                "description": "my dnat rule 01" 
             } 
         }
        ```

    3.  更新指定端口范围的规则。

        ```
        PUT https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/dnat_rules/79195d50-0271-41f1-bded-4c089b2502ff
        { 
             "dnat_rule": { 
                 "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
                 "floating_ip_id": "bf99c679-9f41-4dac-8513-9c9228e713e1",
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

    4.  只更新规则的描述信息。

        ```
        PUT https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/dnat_rules/79195d50-0271-41f1-bded-4c089b2502ff
        { 
             "dnat_rule": { 
                "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
                "description": "my dnat rule 01"
             } 
        }
        ```


-   响应样例
    1.  更新指定端口的规则的响应

        ```
        { 
             "dnat_rule": { 
                 "status": "ACTIVE", 
                 "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8", 
                 "admin_state_up": true, 
                 "port_id": "9a469561-daac-4c94-88f5-39366e5ea193", 
                 "internal_service_port": 993, 
                 "protocol": "tcp", 
                 "tenant_id": "abc", 
                 "floating_ip_id": "cf99c679-9f41-4dac-8513-9c9228e713e1",
                 "created_at": "2017-11-15 15:44:42.595173", 
                 "id": "79195d50-0271-41f1-bded-4c089b2502ff", 
                 "floating_ip_address": "5.21.11.226", 
                 "external_service_port": 242, 
                 "description": "my dnat rule 01" 
             } 
         }
        ```

    2.  更新all port类型的规则的响应

        ```
        { 
             "dnat_rule": { 
                 "status": "ACTIVE", 
                 "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8", 
                 "admin_state_up": true, 
                 "private_ip": "192.168.1.100", 
                 "internal_service_port": 0, 
                 "protocol": "any", 
                 "tenant_id": "abc", 
                 "floating_ip_id": "bf99c679-9f41-4dac-8513-9c9228e713e1",
                 "created_at": "2017-11-15 15:44:42.595173", 
                 "id": "79195d50-0271-41f1-bded-4c089b2502ff", 
                 "floating_ip_address ": "5.21.11.227", 
                 "external_service_port": 0, 
                 "description": "my dnat rule 01" 
             } 
         }
        ```

    3.  更新指定端口范围的规则的响应

        ```
        { 
             "dnat_rule": { 
                 "status": "ACTIVE", 
                 "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8", 
                 "admin_state_up": true, 
                 "private_ip": "192.168.1.100", 
                 "internal_service_port": 0, 
                 "protocol": "tcp", 
                 "tenant_id": "abc", 
                 "floating_ip_id": "bf99c679-9f41-4dac-8513-9c9228e713e1",
                 "created_at": "2017-11-15 15:44:42.595173", 
                 "id": "79195d50-0271-41f1-bded-4c089b2502ff", 
                 "floating_ip_address ": "5.21.11.227", 
                 "external_service_port": 0, 
                 "description": "my dnat rule 01",
                 "internal_service_port_range": "100-200",
                 "external_service_port_range": "100-200"
             } 
         }
        ```

    4.  只更新规则的描述信息的响应

        ```
        { 
             "dnat_rule": { 
                 "status": "ACTIVE", 
                 "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8", 
                 "admin_state_up": true, 
                 "port_id": "9a469561-daac-4c94-88f5-39366e5ea193", 
                 "private_ip": "",
                 "internal_service_port": 993, 
                 "protocol": "tcp", 
                 "tenant_id": "abc", 
                 "floating_ip_id": "cf99c679-9f41-4dac-8513-9c9228e713e1",
                 "created_at": "2017-11-15 15:44:42.595173", 
                 "id": "79195d50-0271-41f1-bded-4c089b2502ff", 
                 "floating_ip_address": "5.21.11.226", 
                 "external_service_port": 242, 
                 "description": "my dnat rule 01" 
             } 
         }
        ```



## 状态码<a name="zh-cn_topic_0168797296_section16479115674819"></a>

请参考[状态码](状态码.md)。

