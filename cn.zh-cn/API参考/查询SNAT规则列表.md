# 查询SNAT规则列表<a name="nat_api_0007"></a>

## 功能介绍<a name="section3132024"></a>

查询SNAT规则列表。

## URI<a name="section28188224"></a>

GET /v2.0/snat\_rules

>![](public_sys-resources/icon-note.gif) **说明：**   
>可以在URI后面用‘?’和‘&’添加不同的查询条件组合。支持参数说明中所有非必选参数过滤，请参考请求样例。  

**表 1**  参数说明

<a name="table1994131474314"></a>
<table><thead align="left"><tr id="row1415051518436"><th class="cellrowborder" valign="top" width="21.34%" id="mcps1.2.5.1.1"><p id="p1415014152437"><a name="p1415014152437"></a><a name="p1415014152437"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="11.68%" id="mcps1.2.5.1.2"><p id="p0314161614916"><a name="p0314161614916"></a><a name="p0314161614916"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.09%" id="mcps1.2.5.1.3"><p id="p111508151438"><a name="p111508151438"></a><a name="p111508151438"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="49.89%" id="mcps1.2.5.1.4"><p id="p215041554317"><a name="p215041554317"></a><a name="p215041554317"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1415051517431"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="p131501515144316"><a name="p131501515144316"></a><a name="p131501515144316"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="11.68%" headers="mcps1.2.5.1.2 "><p id="p1931471624917"><a name="p1931471624917"></a><a name="p1931471624917"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.09%" headers="mcps1.2.5.1.3 "><p id="p111507156439"><a name="p111507156439"></a><a name="p111507156439"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="49.89%" headers="mcps1.2.5.1.4 "><p id="p191501915184313"><a name="p191501915184313"></a><a name="p191501915184313"></a>SNAT规则的id。</p>
</td>
</tr>
<tr id="row4353106192713"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="p149161116277"><a name="p149161116277"></a><a name="p149161116277"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="11.68%" headers="mcps1.2.5.1.2 "><p id="p113141516144920"><a name="p113141516144920"></a><a name="p113141516144920"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.09%" headers="mcps1.2.5.1.3 "><p id="p549121120274"><a name="p549121120274"></a><a name="p549121120274"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="49.89%" headers="mcps1.2.5.1.4 "><p id="p12495111278"><a name="p12495111278"></a><a name="p12495111278"></a>每页返回的个数。</p>
</td>
</tr>
<tr id="row15150121504310"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="p915012158432"><a name="p915012158432"></a><a name="p915012158432"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="11.68%" headers="mcps1.2.5.1.2 "><p id="p531415165495"><a name="p531415165495"></a><a name="p531415165495"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.09%" headers="mcps1.2.5.1.3 "><p id="p181501815134315"><a name="p181501815134315"></a><a name="p181501815134315"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="49.89%" headers="mcps1.2.5.1.4 "><p id="p2150101584316"><a name="p2150101584316"></a><a name="p2150101584316"></a>项目的ID。</p>
</td>
</tr>
<tr id="row21505159436"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="p3150181564316"><a name="p3150181564316"></a><a name="p3150181564316"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="11.68%" headers="mcps1.2.5.1.2 "><p id="p19314131611491"><a name="p19314131611491"></a><a name="p19314131611491"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.09%" headers="mcps1.2.5.1.3 "><p id="p11150121518435"><a name="p11150121518435"></a><a name="p11150121518435"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="49.89%" headers="mcps1.2.5.1.4 "><p id="p18150115174314"><a name="p18150115174314"></a><a name="p18150115174314"></a>所属NAT网关的id。</p>
</td>
</tr>
<tr id="row15150215204316"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="p1115051534313"><a name="p1115051534313"></a><a name="p1115051534313"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="11.68%" headers="mcps1.2.5.1.2 "><p id="p4314121617497"><a name="p4314121617497"></a><a name="p4314121617497"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.09%" headers="mcps1.2.5.1.3 "><p id="p1915071574317"><a name="p1915071574317"></a><a name="p1915071574317"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="49.89%" headers="mcps1.2.5.1.4 "><p id="p10150415104315"><a name="p10150415104315"></a><a name="p10150415104315"></a>规则使用的网络id。</p>
</td>
</tr>
<tr id="row1315041519435"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="p1115018151435"><a name="p1115018151435"></a><a name="p1115018151435"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="11.68%" headers="mcps1.2.5.1.2 "><p id="p17315101616499"><a name="p17315101616499"></a><a name="p17315101616499"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.09%" headers="mcps1.2.5.1.3 "><p id="p51501158433"><a name="p51501158433"></a><a name="p51501158433"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="49.89%" headers="mcps1.2.5.1.4 "><p id="p2150201513432"><a name="p2150201513432"></a><a name="p2150201513432"></a>cidr，vpc 子网网段的子集或专线侧网段。</p>
</td>
</tr>
<tr id="row2150215104311"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="p1150915124313"><a name="p1150915124313"></a><a name="p1150915124313"></a>source_type</p>
</td>
<td class="cellrowborder" valign="top" width="11.68%" headers="mcps1.2.5.1.2 "><p id="p2315151644912"><a name="p2315151644912"></a><a name="p2315151644912"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.09%" headers="mcps1.2.5.1.3 "><p id="p131508153431"><a name="p131508153431"></a><a name="p131508153431"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="49.89%" headers="mcps1.2.5.1.4 "><p id="p1715019154438"><a name="p1715019154438"></a><a name="p1715019154438"></a>0：VPC侧，可以指定network_id 或者cidr</p>
<p id="p4150141514433"><a name="p4150141514433"></a><a name="p4150141514433"></a>1：专线侧，只能指定cidr</p>
<p id="p915031534313"><a name="p915031534313"></a><a name="p915031534313"></a>不输入默认为0（VPC）</p>
</td>
</tr>
<tr id="row15150161513433"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="p315011152432"><a name="p315011152432"></a><a name="p315011152432"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="11.68%" headers="mcps1.2.5.1.2 "><p id="p131521634914"><a name="p131521634914"></a><a name="p131521634914"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.09%" headers="mcps1.2.5.1.3 "><p id="p91505152437"><a name="p91505152437"></a><a name="p91505152437"></a>String(4096)</p>
</td>
<td class="cellrowborder" valign="top" width="49.89%" headers="mcps1.2.5.1.4 "><p id="p138311037012"><a name="p138311037012"></a><a name="p138311037012"></a>功能说明：弹性公网IP的id。</p>
</td>
</tr>
<tr id="row1315061516437"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="p151501215144310"><a name="p151501215144310"></a><a name="p151501215144310"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="11.68%" headers="mcps1.2.5.1.2 "><p id="p131561619498"><a name="p131561619498"></a><a name="p131561619498"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.09%" headers="mcps1.2.5.1.3 "><p id="p8150101514314"><a name="p8150101514314"></a><a name="p8150101514314"></a>String(1024)</p>
</td>
<td class="cellrowborder" valign="top" width="49.89%" headers="mcps1.2.5.1.4 "><p id="p1534335207"><a name="p1534335207"></a><a name="p1534335207"></a>功能说明：弹性公网IP。</p>
</td>
</tr>
<tr id="row3150131544312"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="p181509154430"><a name="p181509154430"></a><a name="p181509154430"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="11.68%" headers="mcps1.2.5.1.2 "><p id="p3315111614912"><a name="p3315111614912"></a><a name="p3315111614912"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.09%" headers="mcps1.2.5.1.3 "><p id="p201505152437"><a name="p201505152437"></a><a name="p201505152437"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="49.89%" headers="mcps1.2.5.1.4 "><a name="ul1815011157431"></a><a name="ul1815011157431"></a><ul id="ul1815011157431"><li>功能说明：SNAT规则的状态。</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="row101509151439"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="p111506155432"><a name="p111506155432"></a><a name="p111506155432"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="11.68%" headers="mcps1.2.5.1.2 "><p id="p031511684912"><a name="p031511684912"></a><a name="p031511684912"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.09%" headers="mcps1.2.5.1.3 "><p id="p1764614265487"><a name="p1764614265487"></a><a name="p1764614265487"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="49.89%" headers="mcps1.2.5.1.4 "><a name="ul71858556358"></a><a name="ul71858556358"></a><ul id="ul71858556358"><li>解冻/冻结状态。</li><li>取值范围：<a name="ul11838172814409"></a><a name="ul11838172814409"></a><ul id="ul11838172814409"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="row14150121515435"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="p16150615184312"><a name="p16150615184312"></a><a name="p16150615184312"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="11.68%" headers="mcps1.2.5.1.2 "><p id="p13315181620498"><a name="p13315181620498"></a><a name="p13315181620498"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.09%" headers="mcps1.2.5.1.3 "><p id="p11150215184311"><a name="p11150215184311"></a><a name="p11150215184311"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="49.89%" headers="mcps1.2.5.1.4 "><p id="p39521571301"><a name="p39521571301"></a><a name="p39521571301"></a>SNAT规则的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section1544804"></a>

无

## 响应消息<a name="section13903243"></a>

响应参数如[表2](#table25574495)所示。

**表 2**  响应参数

<a name="table25574495"></a>
<table><thead align="left"><tr id="row6316572"><th class="cellrowborder" valign="top" width="20.73%" id="mcps1.2.4.1.1"><p id="p41880308"><a name="p41880308"></a><a name="p41880308"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="28.050000000000004%" id="mcps1.2.4.1.2"><p id="p36861764"><a name="p36861764"></a><a name="p36861764"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p56800622"><a name="p56800622"></a><a name="p56800622"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row37447704"><td class="cellrowborder" valign="top" width="20.73%" headers="mcps1.2.4.1.1 "><p id="p13365211"><a name="p13365211"></a><a name="p13365211"></a>snat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="28.050000000000004%" headers="mcps1.2.4.1.2 "><p id="p8840286"><a name="p8840286"></a><a name="p8840286"></a>List(snat_rule)</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p19058885"><a name="p19058885"></a><a name="p19058885"></a>snat_rule对象列表。详见<a href="#table589411291812">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  snat\_rule字段说明

<a name="table589411291812"></a>
<table><thead align="left"><tr id="row78949281818"><th class="cellrowborder" valign="top" width="20.92209220922092%" id="mcps1.2.4.1.1"><p id="p144282010346"><a name="p144282010346"></a><a name="p144282010346"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="28.162816281628167%" id="mcps1.2.4.1.2"><p id="p1742881017412"><a name="p1742881017412"></a><a name="p1742881017412"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50.91509150915091%" id="mcps1.2.4.1.3"><p id="p1442813106416"><a name="p1442813106416"></a><a name="p1442813106416"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row158941625183"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="p1059722885319"><a name="p1059722885319"></a><a name="p1059722885319"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="p1859722895314"><a name="p1859722895314"></a><a name="p1859722895314"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><p id="p759782812534"><a name="p759782812534"></a><a name="p759782812534"></a>SNAT规则的id。</p>
</td>
</tr>
<tr id="row189413213184"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="p1759782816538"><a name="p1759782816538"></a><a name="p1759782816538"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="p959719287534"><a name="p959719287534"></a><a name="p959719287534"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><p id="p15597328145316"><a name="p15597328145316"></a><a name="p15597328145316"></a>项目的ID。</p>
</td>
</tr>
<tr id="row17894326185"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="p75979285538"><a name="p75979285538"></a><a name="p75979285538"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="p4597152810532"><a name="p4597152810532"></a><a name="p4597152810532"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><p id="p7597202805311"><a name="p7597202805311"></a><a name="p7597202805311"></a>所属NAT网关的id。</p>
</td>
</tr>
<tr id="row8894121185"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="p17597828105318"><a name="p17597828105318"></a><a name="p17597828105318"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="p159732815535"><a name="p159732815535"></a><a name="p159732815535"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><p id="p11597182885319"><a name="p11597182885319"></a><a name="p11597182885319"></a>规则使用的网络id。</p>
</td>
</tr>
<tr id="row1689422131813"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="p7597152814536"><a name="p7597152814536"></a><a name="p7597152814536"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="p1959752813534"><a name="p1959752813534"></a><a name="p1959752813534"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><p id="p85971428135313"><a name="p85971428135313"></a><a name="p85971428135313"></a>cidr，vpc 子网网段的子集或专线侧网段。</p>
</td>
</tr>
<tr id="row17894229186"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="p1859718289538"><a name="p1859718289538"></a><a name="p1859718289538"></a>source_type</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="p19597152810533"><a name="p19597152810533"></a><a name="p19597152810533"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><p id="p2597142811539"><a name="p2597142811539"></a><a name="p2597142811539"></a>0：VPC侧，可以指定network_id 或者cidr</p>
<p id="p175971428185312"><a name="p175971428185312"></a><a name="p175971428185312"></a>1：专线侧，只能指定cidr</p>
<p id="p159762875319"><a name="p159762875319"></a><a name="p159762875319"></a>不输入默认为0（VPC）</p>
</td>
</tr>
<tr id="row1189413211817"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="p4597152810537"><a name="p4597152810537"></a><a name="p4597152810537"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="p13597128105319"><a name="p13597128105319"></a><a name="p13597128105319"></a>String(4096)</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><a name="ul95970283530"></a><a name="ul95970283530"></a><ul id="ul95970283530"><li>功能说明：弹性公网IP的id，多个弹性公网IP使用逗号分隔。</li><li>取值范围：最大长度4096字节。</li><li>约束：弹性公网IP的id个数不能超过20个</li></ul>
</td>
</tr>
<tr id="row1214011791212"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="p7890161710129"><a name="p7890161710129"></a><a name="p7890161710129"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="p19890917111215"><a name="p19890917111215"></a><a name="p19890917111215"></a>String(1024)</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><a name="ul12890181721213"></a><a name="ul12890181721213"></a><ul id="ul12890181721213"><li>功能说明：弹性公网IP，多个弹性公网IP使用逗号分隔。</li><li>取值范围：最大长度1024字节。</li></ul>
</td>
</tr>
<tr id="row68941219185"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="p185971828135312"><a name="p185971828135312"></a><a name="p185971828135312"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="p16597228135314"><a name="p16597228135314"></a><a name="p16597228135314"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><a name="ul105971428125319"></a><a name="ul105971428125319"></a><ul id="ul105971428125319"><li>功能说明：SNAT规则的状态。</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="row689419281813"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="p1759792811533"><a name="p1759792811533"></a><a name="p1759792811533"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="p10798165216111"><a name="p10798165216111"></a><a name="p10798165216111"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><a name="ul121279715562"></a><a name="ul121279715562"></a><ul id="ul121279715562"><li>解冻/冻结状态。</li><li>取值范围：<a name="ul171281976564"></a><a name="ul171281976564"></a><ul id="ul171281976564"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="row4894182171813"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="p7382183916534"><a name="p7382183916534"></a><a name="p7382183916534"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="p1238211390533"><a name="p1238211390533"></a><a name="p1238211390533"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><p id="p1748651410013"><a name="p1748651410013"></a><a name="p1748651410013"></a>SNAT规则的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section58020329"></a>

-   请求样例

    ```
    GET https://{Endpoint}/v2.0/snat_rules?limit=10
    ```


-   响应样例

    ```
    {
        "snat_rules": [
          {
                "floating_ip_id": "bf99c679-9f41-4dac-8513-9c9228e713e1",
                "status": "ACTIVE",
                "nat_gateway_id": "cda3a125-2406-456c-a11f-598e10578541",
                "admin_state_up": true,
                "network_id": "9a469561-daac-4c94-88f5-39366e5ea193",
                "cidr": "null",
                "source_type":0,
                "tenant_id": "abc",
                "created_at": "2017-11-15 15:44:42.595173",
                "id": "79195d50-0271-41f1-bded-4c089b2502ff",
                "floating_ip_address": "5.21.11.242"
            },
            {
                "floating_ip_id": "6e496fba-abe9-4f5e-9406-2ad8c809ac8c",
                "status": "ACTIVE",
                "nat_gateway_id": "e824f1b4-4290-4ebc-8322-cfff370dbd1e",
                "admin_state_up": true,
                "network_id": "97e89905-f9c8-4ae3-9856-392b0b2fbe7f",
                "cidr": "null",
                "source_type":0,
                "tenant_id": "abc",
                "created_at": "2017-11-17 07:43:44.830845",
                "id": "4a1a10d7-0d9f-4846-8cda-24cffeffef5c",
                "floating_ip_address": "5.21.11.142"
            }
        ]
    }
    ```


## 状态码<a name="section13981185113572"></a>

请参考[状态码](状态码.md)。

