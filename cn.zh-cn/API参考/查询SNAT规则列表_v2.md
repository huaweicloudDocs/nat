# 查询SNAT规则列表<a name="nat_apiv2_0012"></a>

## 功能介绍<a name="zh-cn_topic_0168797266_section3132024"></a>

查询SNAT规则列表。

## URI<a name="zh-cn_topic_0168797266_section28188224"></a>

GET /v2/\{project\_id\}/snat\_rules

>![](public_sys-resources/icon-note.gif) **说明：**   
>可以在URI后面用‘?’和‘&’添加不同的查询条件组合。支持参数说明中所有非必选参数过滤，请参考请求样例。  

**表 1**  参数说明

<a name="zh-cn_topic_0168797266_table1994131474314"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797266_row1415051518436"><th class="cellrowborder" valign="top" width="21.34%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797266_p1415014152437"><a name="zh-cn_topic_0168797266_p1415014152437"></a><a name="zh-cn_topic_0168797266_p1415014152437"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.08%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797266_p175233518262"><a name="zh-cn_topic_0168797266_p175233518262"></a><a name="zh-cn_topic_0168797266_p175233518262"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.65%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797266_p111508151438"><a name="zh-cn_topic_0168797266_p111508151438"></a><a name="zh-cn_topic_0168797266_p111508151438"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="52.93%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797266_p215041554317"><a name="zh-cn_topic_0168797266_p215041554317"></a><a name="zh-cn_topic_0168797266_p215041554317"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797266_row10403155131217"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797266_p123101240139"><a name="zh-cn_topic_0168797266_p123101240139"></a><a name="zh-cn_topic_0168797266_p123101240139"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797266_p14523185111268"><a name="zh-cn_topic_0168797266_p14523185111268"></a><a name="zh-cn_topic_0168797266_p14523185111268"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797266_p231054131314"><a name="zh-cn_topic_0168797266_p231054131314"></a><a name="zh-cn_topic_0168797266_p231054131314"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797266_p131074161319"><a name="zh-cn_topic_0168797266_p131074161319"></a><a name="zh-cn_topic_0168797266_p131074161319"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row3975185111124"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797266_p53101241133"><a name="zh-cn_topic_0168797266_p53101241133"></a><a name="zh-cn_topic_0168797266_p53101241133"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797266_p05231951172613"><a name="zh-cn_topic_0168797266_p05231951172613"></a><a name="zh-cn_topic_0168797266_p05231951172613"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797266_p5729181885117"><a name="zh-cn_topic_0168797266_p5729181885117"></a><a name="zh-cn_topic_0168797266_p5729181885117"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797266_p1231014191310"><a name="zh-cn_topic_0168797266_p1231014191310"></a><a name="zh-cn_topic_0168797266_p1231014191310"></a>功能说明：每页返回的个数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row1415051517431"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797266_p131501515144316"><a name="zh-cn_topic_0168797266_p131501515144316"></a><a name="zh-cn_topic_0168797266_p131501515144316"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797266_p12523145142615"><a name="zh-cn_topic_0168797266_p12523145142615"></a><a name="zh-cn_topic_0168797266_p12523145142615"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797266_p111507156439"><a name="zh-cn_topic_0168797266_p111507156439"></a><a name="zh-cn_topic_0168797266_p111507156439"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797266_p191501915184313"><a name="zh-cn_topic_0168797266_p191501915184313"></a><a name="zh-cn_topic_0168797266_p191501915184313"></a>SNAT规则的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row15150121504310"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797266_p915012158432"><a name="zh-cn_topic_0168797266_p915012158432"></a><a name="zh-cn_topic_0168797266_p915012158432"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797266_p45241851162613"><a name="zh-cn_topic_0168797266_p45241851162613"></a><a name="zh-cn_topic_0168797266_p45241851162613"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797266_p181501815134315"><a name="zh-cn_topic_0168797266_p181501815134315"></a><a name="zh-cn_topic_0168797266_p181501815134315"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797266_p2150101584316"><a name="zh-cn_topic_0168797266_p2150101584316"></a><a name="zh-cn_topic_0168797266_p2150101584316"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row21505159436"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797266_p3150181564316"><a name="zh-cn_topic_0168797266_p3150181564316"></a><a name="zh-cn_topic_0168797266_p3150181564316"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797266_p125241951192619"><a name="zh-cn_topic_0168797266_p125241951192619"></a><a name="zh-cn_topic_0168797266_p125241951192619"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797266_p11150121518435"><a name="zh-cn_topic_0168797266_p11150121518435"></a><a name="zh-cn_topic_0168797266_p11150121518435"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797266_p18150115174314"><a name="zh-cn_topic_0168797266_p18150115174314"></a><a name="zh-cn_topic_0168797266_p18150115174314"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row15150215204316"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797266_p1115051534313"><a name="zh-cn_topic_0168797266_p1115051534313"></a><a name="zh-cn_topic_0168797266_p1115051534313"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797266_p155241251142613"><a name="zh-cn_topic_0168797266_p155241251142613"></a><a name="zh-cn_topic_0168797266_p155241251142613"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797266_p1915071574317"><a name="zh-cn_topic_0168797266_p1915071574317"></a><a name="zh-cn_topic_0168797266_p1915071574317"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797266_p10150415104315"><a name="zh-cn_topic_0168797266_p10150415104315"></a><a name="zh-cn_topic_0168797266_p10150415104315"></a>规则使用的网络id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row1315041519435"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797266_p1115018151435"><a name="zh-cn_topic_0168797266_p1115018151435"></a><a name="zh-cn_topic_0168797266_p1115018151435"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797266_p8524125172611"><a name="zh-cn_topic_0168797266_p8524125172611"></a><a name="zh-cn_topic_0168797266_p8524125172611"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797266_p51501158433"><a name="zh-cn_topic_0168797266_p51501158433"></a><a name="zh-cn_topic_0168797266_p51501158433"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797266_p2150201513432"><a name="zh-cn_topic_0168797266_p2150201513432"></a><a name="zh-cn_topic_0168797266_p2150201513432"></a>cidr，vpc 子网网段的子集或专线侧网段。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row2150215104311"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797266_p1150915124313"><a name="zh-cn_topic_0168797266_p1150915124313"></a><a name="zh-cn_topic_0168797266_p1150915124313"></a>source_type</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797266_p135241951122617"><a name="zh-cn_topic_0168797266_p135241951122617"></a><a name="zh-cn_topic_0168797266_p135241951122617"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797266_p131508153431"><a name="zh-cn_topic_0168797266_p131508153431"></a><a name="zh-cn_topic_0168797266_p131508153431"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797266_p1715019154438"><a name="zh-cn_topic_0168797266_p1715019154438"></a><a name="zh-cn_topic_0168797266_p1715019154438"></a>0：VPC侧，可以指定network_id 或者cidr</p>
<p id="zh-cn_topic_0168797266_p4150141514433"><a name="zh-cn_topic_0168797266_p4150141514433"></a><a name="zh-cn_topic_0168797266_p4150141514433"></a>1：专线侧，只能指定cidr</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row15150161513433"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797266_p315011152432"><a name="zh-cn_topic_0168797266_p315011152432"></a><a name="zh-cn_topic_0168797266_p315011152432"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797266_p55241751102620"><a name="zh-cn_topic_0168797266_p55241751102620"></a><a name="zh-cn_topic_0168797266_p55241751102620"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797266_p91505152437"><a name="zh-cn_topic_0168797266_p91505152437"></a><a name="zh-cn_topic_0168797266_p91505152437"></a>String(4096)</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0168797266_ul51501150435"></a><a name="zh-cn_topic_0168797266_ul51501150435"></a><ul id="zh-cn_topic_0168797266_ul51501150435"><li>功能说明：弹性公网IP的id。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row1315061516437"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797266_p151501215144310"><a name="zh-cn_topic_0168797266_p151501215144310"></a><a name="zh-cn_topic_0168797266_p151501215144310"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797266_p052445110260"><a name="zh-cn_topic_0168797266_p052445110260"></a><a name="zh-cn_topic_0168797266_p052445110260"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797266_p8150101514314"><a name="zh-cn_topic_0168797266_p8150101514314"></a><a name="zh-cn_topic_0168797266_p8150101514314"></a>String(1024)</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0168797266_ul1715061514439"></a><a name="zh-cn_topic_0168797266_ul1715061514439"></a><ul id="zh-cn_topic_0168797266_ul1715061514439"><li>功能说明：弹性公网IP。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row3150131544312"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797266_p181509154430"><a name="zh-cn_topic_0168797266_p181509154430"></a><a name="zh-cn_topic_0168797266_p181509154430"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797266_p17524165117265"><a name="zh-cn_topic_0168797266_p17524165117265"></a><a name="zh-cn_topic_0168797266_p17524165117265"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797266_p201505152437"><a name="zh-cn_topic_0168797266_p201505152437"></a><a name="zh-cn_topic_0168797266_p201505152437"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0168797266_ul1815011157431"></a><a name="zh-cn_topic_0168797266_ul1815011157431"></a><ul id="zh-cn_topic_0168797266_ul1815011157431"><li>功能说明：SNAT规则的状态。</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row101509151439"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797266_p111506155432"><a name="zh-cn_topic_0168797266_p111506155432"></a><a name="zh-cn_topic_0168797266_p111506155432"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797266_p4524951182611"><a name="zh-cn_topic_0168797266_p4524951182611"></a><a name="zh-cn_topic_0168797266_p4524951182611"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797266_p123591715152620"><a name="zh-cn_topic_0168797266_p123591715152620"></a><a name="zh-cn_topic_0168797266_p123591715152620"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0168797266_ul71858556358"></a><a name="zh-cn_topic_0168797266_ul71858556358"></a><ul id="zh-cn_topic_0168797266_ul71858556358"><li>解冻/冻结状态。</li><li>取值范围：<a name="zh-cn_topic_0168797266_ul11838172814409"></a><a name="zh-cn_topic_0168797266_ul11838172814409"></a><ul id="zh-cn_topic_0168797266_ul11838172814409"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row14150121515435"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797266_p16150615184312"><a name="zh-cn_topic_0168797266_p16150615184312"></a><a name="zh-cn_topic_0168797266_p16150615184312"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797266_p4524135142616"><a name="zh-cn_topic_0168797266_p4524135142616"></a><a name="zh-cn_topic_0168797266_p4524135142616"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797266_p11150215184311"><a name="zh-cn_topic_0168797266_p11150215184311"></a><a name="zh-cn_topic_0168797266_p11150215184311"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797266_p63411931122018"><a name="zh-cn_topic_0168797266_p63411931122018"></a><a name="zh-cn_topic_0168797266_p63411931122018"></a>SNAT规则的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0168797266_section1544804"></a>

无

## 响应消息<a name="zh-cn_topic_0168797266_section13903243"></a>

响应参数如[表2](#zh-cn_topic_0168797266_table25574495)所示。

**表 2**  响应参数

<a name="zh-cn_topic_0168797266_table25574495"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797266_row6316572"><th class="cellrowborder" valign="top" width="20.73%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797266_p41880308"><a name="zh-cn_topic_0168797266_p41880308"></a><a name="zh-cn_topic_0168797266_p41880308"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="28.050000000000004%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797266_p36861764"><a name="zh-cn_topic_0168797266_p36861764"></a><a name="zh-cn_topic_0168797266_p36861764"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797266_p56800622"><a name="zh-cn_topic_0168797266_p56800622"></a><a name="zh-cn_topic_0168797266_p56800622"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797266_row37447704"><td class="cellrowborder" valign="top" width="20.73%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797266_p13365211"><a name="zh-cn_topic_0168797266_p13365211"></a><a name="zh-cn_topic_0168797266_p13365211"></a>snat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="28.050000000000004%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797266_p8840286"><a name="zh-cn_topic_0168797266_p8840286"></a><a name="zh-cn_topic_0168797266_p8840286"></a>Array(Object)</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797266_p19058885"><a name="zh-cn_topic_0168797266_p19058885"></a><a name="zh-cn_topic_0168797266_p19058885"></a>snat_rule对象列表。请参考<a href="#zh-cn_topic_0168797266_table589411291812">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  snat\_rule字段说明

<a name="zh-cn_topic_0168797266_table589411291812"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797266_row78949281818"><th class="cellrowborder" valign="top" width="20.92209220922092%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797266_p144282010346"><a name="zh-cn_topic_0168797266_p144282010346"></a><a name="zh-cn_topic_0168797266_p144282010346"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="28.162816281628167%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797266_p1742881017412"><a name="zh-cn_topic_0168797266_p1742881017412"></a><a name="zh-cn_topic_0168797266_p1742881017412"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50.91509150915091%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797266_p1442813106416"><a name="zh-cn_topic_0168797266_p1442813106416"></a><a name="zh-cn_topic_0168797266_p1442813106416"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797266_row158941625183"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797266_p1059722885319"><a name="zh-cn_topic_0168797266_p1059722885319"></a><a name="zh-cn_topic_0168797266_p1059722885319"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797266_p1859722895314"><a name="zh-cn_topic_0168797266_p1859722895314"></a><a name="zh-cn_topic_0168797266_p1859722895314"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797266_p759782812534"><a name="zh-cn_topic_0168797266_p759782812534"></a><a name="zh-cn_topic_0168797266_p759782812534"></a>SNAT规则的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row189413213184"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797266_p1759782816538"><a name="zh-cn_topic_0168797266_p1759782816538"></a><a name="zh-cn_topic_0168797266_p1759782816538"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797266_p959719287534"><a name="zh-cn_topic_0168797266_p959719287534"></a><a name="zh-cn_topic_0168797266_p959719287534"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797266_p15597328145316"><a name="zh-cn_topic_0168797266_p15597328145316"></a><a name="zh-cn_topic_0168797266_p15597328145316"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row17894326185"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797266_p75979285538"><a name="zh-cn_topic_0168797266_p75979285538"></a><a name="zh-cn_topic_0168797266_p75979285538"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797266_p4597152810532"><a name="zh-cn_topic_0168797266_p4597152810532"></a><a name="zh-cn_topic_0168797266_p4597152810532"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797266_p7597202805311"><a name="zh-cn_topic_0168797266_p7597202805311"></a><a name="zh-cn_topic_0168797266_p7597202805311"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row8894121185"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797266_p17597828105318"><a name="zh-cn_topic_0168797266_p17597828105318"></a><a name="zh-cn_topic_0168797266_p17597828105318"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797266_p159732815535"><a name="zh-cn_topic_0168797266_p159732815535"></a><a name="zh-cn_topic_0168797266_p159732815535"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797266_p11597182885319"><a name="zh-cn_topic_0168797266_p11597182885319"></a><a name="zh-cn_topic_0168797266_p11597182885319"></a>规则使用的网络id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row17894229186"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797266_p1859718289538"><a name="zh-cn_topic_0168797266_p1859718289538"></a><a name="zh-cn_topic_0168797266_p1859718289538"></a>source_type</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797266_p123061471519"><a name="zh-cn_topic_0168797266_p123061471519"></a><a name="zh-cn_topic_0168797266_p123061471519"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797266_p2597142811539"><a name="zh-cn_topic_0168797266_p2597142811539"></a><a name="zh-cn_topic_0168797266_p2597142811539"></a>0：VPC侧，可以指定network_id 或者cidr</p>
<p id="zh-cn_topic_0168797266_p175971428185312"><a name="zh-cn_topic_0168797266_p175971428185312"></a><a name="zh-cn_topic_0168797266_p175971428185312"></a>1：专线侧，只能指定cidr</p>
<p id="zh-cn_topic_0168797266_p159762875319"><a name="zh-cn_topic_0168797266_p159762875319"></a><a name="zh-cn_topic_0168797266_p159762875319"></a>不输入默认为0（VPC）</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row1189413211817"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797266_p2023152014194"><a name="zh-cn_topic_0168797266_p2023152014194"></a><a name="zh-cn_topic_0168797266_p2023152014194"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797266_p523152081918"><a name="zh-cn_topic_0168797266_p523152081918"></a><a name="zh-cn_topic_0168797266_p523152081918"></a>String(4096)</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797266_ul11231112012196"></a><a name="zh-cn_topic_0168797266_ul11231112012196"></a><ul id="zh-cn_topic_0168797266_ul11231112012196"><li>功能说明：弹性公网IP的id，多个弹性公网IP使用逗号分隔。</li><li>取值范围：最大长度4096字节。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row1214011791212"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797266_p3231182071920"><a name="zh-cn_topic_0168797266_p3231182071920"></a><a name="zh-cn_topic_0168797266_p3231182071920"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797266_p12231202021914"><a name="zh-cn_topic_0168797266_p12231202021914"></a><a name="zh-cn_topic_0168797266_p12231202021914"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797266_p11231620171912"><a name="zh-cn_topic_0168797266_p11231620171912"></a><a name="zh-cn_topic_0168797266_p11231620171912"></a>SNAT规则的描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row65931115125"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797266_p72311207198"><a name="zh-cn_topic_0168797266_p72311207198"></a><a name="zh-cn_topic_0168797266_p72311207198"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797266_p19232192041910"><a name="zh-cn_topic_0168797266_p19232192041910"></a><a name="zh-cn_topic_0168797266_p19232192041910"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797266_ul11232102091919"></a><a name="zh-cn_topic_0168797266_ul11232102091919"></a><ul id="zh-cn_topic_0168797266_ul11232102091919"><li>功能说明：SNAT规则的状态。</li><li>取值范围：<u id="zh-cn_topic_0168797266_u723242018192"><a name="zh-cn_topic_0168797266_u723242018192"></a><a name="zh-cn_topic_0168797266_u723242018192"></a><u id="zh-cn_topic_0168797266_u42321720161917"><a name="zh-cn_topic_0168797266_u42321720161917"></a><a name="zh-cn_topic_0168797266_u42321720161917"></a><a href="资源状态说明.md">资源状态说明</a></u></u>。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row14894172111816"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797266_p22321020121910"><a name="zh-cn_topic_0168797266_p22321020121910"></a><a name="zh-cn_topic_0168797266_p22321020121910"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797266_p57349190268"><a name="zh-cn_topic_0168797266_p57349190268"></a><a name="zh-cn_topic_0168797266_p57349190268"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797266_ul525919441039"></a><a name="zh-cn_topic_0168797266_ul525919441039"></a><ul id="zh-cn_topic_0168797266_ul525919441039"><li>解冻/冻结状态。</li><li>取值范围：<a name="zh-cn_topic_0168797266_ul13259114415319"></a><a name="zh-cn_topic_0168797266_ul13259114415319"></a><ul id="zh-cn_topic_0168797266_ul13259114415319"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row68941219185"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797266_p62325209194"><a name="zh-cn_topic_0168797266_p62325209194"></a><a name="zh-cn_topic_0168797266_p62325209194"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797266_p1723252018193"><a name="zh-cn_topic_0168797266_p1723252018193"></a><a name="zh-cn_topic_0168797266_p1723252018193"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797266_p7323161892411"><a name="zh-cn_topic_0168797266_p7323161892411"></a><a name="zh-cn_topic_0168797266_p7323161892411"></a>SNAT规则的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row689419281813"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797266_p16232620141916"><a name="zh-cn_topic_0168797266_p16232620141916"></a><a name="zh-cn_topic_0168797266_p16232620141916"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797266_p2232192061911"><a name="zh-cn_topic_0168797266_p2232192061911"></a><a name="zh-cn_topic_0168797266_p2232192061911"></a>String(1024)</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797266_ul15232720111914"></a><a name="zh-cn_topic_0168797266_ul15232720111914"></a><ul id="zh-cn_topic_0168797266_ul15232720111914"><li>功能说明：弹性公网IP，多个弹性公网IP使用逗号分隔。</li><li>取值范围：最大长度1024字节。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797266_row4894182171813"><td class="cellrowborder" valign="top" width="20.92209220922092%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797266_p15232162011911"><a name="zh-cn_topic_0168797266_p15232162011911"></a><a name="zh-cn_topic_0168797266_p15232162011911"></a>freezed_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="28.162816281628167%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797266_p11232420121911"><a name="zh-cn_topic_0168797266_p11232420121911"></a><a name="zh-cn_topic_0168797266_p11232420121911"></a>String(1024)</p>
</td>
<td class="cellrowborder" valign="top" width="50.91509150915091%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797266_ul8232520181919"></a><a name="zh-cn_topic_0168797266_ul8232520181919"></a><ul id="zh-cn_topic_0168797266_ul8232520181919"><li>功能说明：冻结的弹性公网IP，多个冻结的弹性公网IP使用逗号分隔。</li><li>取值范围：最大长度1024字节。</li></ul>
</td>
</tr>
</tbody>
</table>

## 示例<a name="zh-cn_topic_0168797266_section58020329"></a>

-   请求样例

    ```
    GET https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/snat_rules?limit=10
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
                 "source_type":0,
                 "tenant_id": "d199ba7e0ba64899b2e81518104b1526", 
                 "created_at": "2017-11-15 15:44:42.595173", 
                 "id": "79195d50-0271-41f1-bded-4c089b2502ff", 
                 "floating_ip_address": "5.21.11.242", 
                 "freezed_ip_address": "", 
                 "description": "my snat rule 01" 
             }, 
             { 
                 "floating_ip_id": "6e496fba-abe9-4f5e-9406-2ad8c809ac8c", 
                 "status": "ACTIVE", 
                 "nat_gateway_id": "e824f1b4-4290-4ebc-8322-cfff370dbd1e", 
                 "admin_state_up": true, 
                 "network_id": "97e89905-f9c8-4ae3-9856-392b0b2fbe7f", 
                 "source_type":0,
                 "tenant_id": "d199ba7e0ba64899b2e81518104b1526",
                 "created_at": "2017-11-17 07:43:44.830845", 
                 "id": "4a1a10d7-0d9f-4846-8cda-24cffeffef5c", 
                 "floating_ip_address": "5.21.11.142,5.21.11.143", 
                 "freezed_ip_address": "5.21.11.142", 
                 "description": "my snat rule 01" 
             } 
         ] 
     }
    ```


## 状态码<a name="zh-cn_topic_0168797266_section13981185113572"></a>

请参考[状态码](状态码.md)。

