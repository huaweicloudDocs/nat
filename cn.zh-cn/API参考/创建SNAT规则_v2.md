# 创建SNAT规则<a name="nat_apiv2_0011"></a>

## 功能介绍<a name="zh-cn_topic_0168797293_section45647471"></a>

创建SNAT规则。

>![](public_sys-resources/icon-note.gif) **说明：**   
>创建规则时，要求网关状态status = "ACTIVE"，要求网关管理员状态admin\_state\_up = True。  

## URI<a name="zh-cn_topic_0168797293_section8174056"></a>

POST /v2/\{project\_id\}/snat\_rules

**表 1**  参数说明

<a name="zh-cn_topic_0168797293_table14514455567"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797293_row64694517562"><th class="cellrowborder" valign="top" width="24.349999999999998%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797293_p7437419576"><a name="zh-cn_topic_0168797293_p7437419576"></a><a name="zh-cn_topic_0168797293_p7437419576"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.200000000000001%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797293_p5437715575"><a name="zh-cn_topic_0168797293_p5437715575"></a><a name="zh-cn_topic_0168797293_p5437715575"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.9%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797293_p89446415326"><a name="zh-cn_topic_0168797293_p89446415326"></a><a name="zh-cn_topic_0168797293_p89446415326"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="49.55%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797293_p143751105718"><a name="zh-cn_topic_0168797293_p143751105718"></a><a name="zh-cn_topic_0168797293_p143751105718"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797293_row7468456567"><td class="cellrowborder" valign="top" width="24.349999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797293_p64371019574"><a name="zh-cn_topic_0168797293_p64371019574"></a><a name="zh-cn_topic_0168797293_p64371019574"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.200000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797293_p164375145715"><a name="zh-cn_topic_0168797293_p164375145715"></a><a name="zh-cn_topic_0168797293_p164375145715"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797293_p194415412323"><a name="zh-cn_topic_0168797293_p194415412323"></a><a name="zh-cn_topic_0168797293_p194415412323"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="49.55%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797293_p34371616575"><a name="zh-cn_topic_0168797293_p34371616575"></a><a name="zh-cn_topic_0168797293_p34371616575"></a>项目ID。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0168797293_section58118839"></a>

请求参数如[表2](#zh-cn_topic_0168797293_table10267194320114)所示。

**表 2**  请求参数

<a name="zh-cn_topic_0168797293_table10267194320114"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797293_row6376174317113"><th class="cellrowborder" valign="top" width="23.72%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797293_p83761431417"><a name="zh-cn_topic_0168797293_p83761431417"></a><a name="zh-cn_topic_0168797293_p83761431417"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.219999999999999%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797293_p19376144311113"><a name="zh-cn_topic_0168797293_p19376144311113"></a><a name="zh-cn_topic_0168797293_p19376144311113"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.56%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797293_p1237644310118"><a name="zh-cn_topic_0168797293_p1237644310118"></a><a name="zh-cn_topic_0168797293_p1237644310118"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="49.5%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797293_p19376243814"><a name="zh-cn_topic_0168797293_p19376243814"></a><a name="zh-cn_topic_0168797293_p19376243814"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797293_row113769431511"><td class="cellrowborder" valign="top" width="23.72%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797293_p143761543316"><a name="zh-cn_topic_0168797293_p143761543316"></a><a name="zh-cn_topic_0168797293_p143761543316"></a>snat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="8.219999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797293_p143761543914"><a name="zh-cn_topic_0168797293_p143761543914"></a><a name="zh-cn_topic_0168797293_p143761543914"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.56%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797293_p3376143212"><a name="zh-cn_topic_0168797293_p3376143212"></a><a name="zh-cn_topic_0168797293_p3376143212"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="49.5%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797293_p63766431210"><a name="zh-cn_topic_0168797293_p63766431210"></a><a name="zh-cn_topic_0168797293_p63766431210"></a>snat_rule对象。请参考<a href="#zh-cn_topic_0168797293_table628219431019">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  snat\_rule字段说明

<a name="zh-cn_topic_0168797293_table628219431019"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797293_row5376743718"><th class="cellrowborder" valign="top" width="22.57%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797293_p4376134314114"><a name="zh-cn_topic_0168797293_p4376134314114"></a><a name="zh-cn_topic_0168797293_p4376134314114"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.649999999999999%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797293_p43767431317"><a name="zh-cn_topic_0168797293_p43767431317"></a><a name="zh-cn_topic_0168797293_p43767431317"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.9%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797293_p3376643415"><a name="zh-cn_topic_0168797293_p3376643415"></a><a name="zh-cn_topic_0168797293_p3376643415"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.879999999999995%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797293_p5376154315117"><a name="zh-cn_topic_0168797293_p5376154315117"></a><a name="zh-cn_topic_0168797293_p5376154315117"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797293_row9376643318"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797293_p33764431917"><a name="zh-cn_topic_0168797293_p33764431917"></a><a name="zh-cn_topic_0168797293_p33764431917"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797293_p143761343014"><a name="zh-cn_topic_0168797293_p143761343014"></a><a name="zh-cn_topic_0168797293_p143761343014"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797293_p143761143518"><a name="zh-cn_topic_0168797293_p143761143518"></a><a name="zh-cn_topic_0168797293_p143761143518"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797293_p15376243712"><a name="zh-cn_topic_0168797293_p15376243712"></a><a name="zh-cn_topic_0168797293_p15376243712"></a>NAT网关的id。请参考<a href="查询NAT网关列表_v2.md#nat_apiv2_0006">查询NAT网关列表</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0168797293_row73761743512"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797293_p18522143016410"><a name="zh-cn_topic_0168797293_p18522143016410"></a><a name="zh-cn_topic_0168797293_p18522143016410"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797293_p115225301847"><a name="zh-cn_topic_0168797293_p115225301847"></a><a name="zh-cn_topic_0168797293_p115225301847"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797293_p9522830441"><a name="zh-cn_topic_0168797293_p9522830441"></a><a name="zh-cn_topic_0168797293_p9522830441"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797293_p115223302049"><a name="zh-cn_topic_0168797293_p115223302049"></a><a name="zh-cn_topic_0168797293_p115223302049"></a>规则使用的网络id。请参考<a href="https://support.huaweicloud.com/api-vpc/vpc_network_0001.html" target="_blank" rel="noopener noreferrer">查询网络列表</a>。与cidr参数二选一。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797293_row237617432112"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797293_p56167320519"><a name="zh-cn_topic_0168797293_p56167320519"></a><a name="zh-cn_topic_0168797293_p56167320519"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797293_p11616163653"><a name="zh-cn_topic_0168797293_p11616163653"></a><a name="zh-cn_topic_0168797293_p11616163653"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797293_p7616132519"><a name="zh-cn_topic_0168797293_p7616132519"></a><a name="zh-cn_topic_0168797293_p7616132519"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797293_p96161631513"><a name="zh-cn_topic_0168797293_p96161631513"></a><a name="zh-cn_topic_0168797293_p96161631513"></a>可以是网段或者主机格式，与network_id参数二选一。</p>
<p id="zh-cn_topic_0168797293_p1861612320514"><a name="zh-cn_topic_0168797293_p1861612320514"></a><a name="zh-cn_topic_0168797293_p1861612320514"></a>Source_type=0时，cidr必须是vpc子网网段的子集(不能相等）;</p>
<p id="zh-cn_topic_0168797293_p20616431753"><a name="zh-cn_topic_0168797293_p20616431753"></a><a name="zh-cn_topic_0168797293_p20616431753"></a>Source_type=1时，cidr必须指定专线侧网段。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797293_row1637684317119"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797293_p1437611434114"><a name="zh-cn_topic_0168797293_p1437611434114"></a><a name="zh-cn_topic_0168797293_p1437611434114"></a>source_type</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797293_p1537617431518"><a name="zh-cn_topic_0168797293_p1537617431518"></a><a name="zh-cn_topic_0168797293_p1537617431518"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797293_p537624314120"><a name="zh-cn_topic_0168797293_p537624314120"></a><a name="zh-cn_topic_0168797293_p537624314120"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797293_p037614433118"><a name="zh-cn_topic_0168797293_p037614433118"></a><a name="zh-cn_topic_0168797293_p037614433118"></a>0：VPC侧，可以指定network_id 或者cidr。</p>
<p id="zh-cn_topic_0168797293_p1937614436114"><a name="zh-cn_topic_0168797293_p1937614436114"></a><a name="zh-cn_topic_0168797293_p1937614436114"></a>1：专线侧，只能指定cidr。</p>
<p id="zh-cn_topic_0168797293_p1137616431711"><a name="zh-cn_topic_0168797293_p1137616431711"></a><a name="zh-cn_topic_0168797293_p1137616431711"></a>不输入默认为0（VPC）。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797293_row19376114318117"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797293_p63761431119"><a name="zh-cn_topic_0168797293_p63761431119"></a><a name="zh-cn_topic_0168797293_p63761431119"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797293_p183763431012"><a name="zh-cn_topic_0168797293_p183763431012"></a><a name="zh-cn_topic_0168797293_p183763431012"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797293_p415981315020"><a name="zh-cn_topic_0168797293_p415981315020"></a><a name="zh-cn_topic_0168797293_p415981315020"></a>String(4096)</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797293_p03765431213"><a name="zh-cn_topic_0168797293_p03765431213"></a><a name="zh-cn_topic_0168797293_p03765431213"></a>功能说明：弹性公网IP的id，多个弹性公网IP使用逗号分隔。</p>
<p id="zh-cn_topic_0168797293_p123761343915"><a name="zh-cn_topic_0168797293_p123761343915"></a><a name="zh-cn_topic_0168797293_p123761343915"></a>取值范围：最大长度4096字节。</p>
<p id="zh-cn_topic_0168797293_p103761343515"><a name="zh-cn_topic_0168797293_p103761343515"></a><a name="zh-cn_topic_0168797293_p103761343515"></a>约束：弹性公网IP的id个数不能超过20个。</p>
<p id="zh-cn_topic_0168797293_p1337614318111"><a name="zh-cn_topic_0168797293_p1337614318111"></a><a name="zh-cn_topic_0168797293_p1337614318111"></a>获取弹性公网IP的id的方法请参考<a href="https://support.huaweicloud.com/api-eip/eip_api_0003.html" target="_blank" rel="noopener noreferrer">查询弹性公网IP列表</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797293_row537613431120"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797293_p83761431715"><a name="zh-cn_topic_0168797293_p83761431715"></a><a name="zh-cn_topic_0168797293_p83761431715"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797293_p637615431416"><a name="zh-cn_topic_0168797293_p637615431416"></a><a name="zh-cn_topic_0168797293_p637615431416"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797293_p552922907"><a name="zh-cn_topic_0168797293_p552922907"></a><a name="zh-cn_topic_0168797293_p552922907"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797293_p037619431019"><a name="zh-cn_topic_0168797293_p037619431019"></a><a name="zh-cn_topic_0168797293_p037619431019"></a>SNAT规则的描述。</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="zh-cn_topic_0168797293_section53307511"></a>

响应参数如[表4](#zh-cn_topic_0168797293_table64245911)所示。

**表 4**  响应参数

<a name="zh-cn_topic_0168797293_table64245911"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797293_row15388566"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797293_p38514356"><a name="zh-cn_topic_0168797293_p38514356"></a><a name="zh-cn_topic_0168797293_p38514356"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="22.84%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797293_p32655106"><a name="zh-cn_topic_0168797293_p32655106"></a><a name="zh-cn_topic_0168797293_p32655106"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.16%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797293_p38657103"><a name="zh-cn_topic_0168797293_p38657103"></a><a name="zh-cn_topic_0168797293_p38657103"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797293_row44217630"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797293_p24858302"><a name="zh-cn_topic_0168797293_p24858302"></a><a name="zh-cn_topic_0168797293_p24858302"></a>snat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="22.84%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797293_p256599"><a name="zh-cn_topic_0168797293_p256599"></a><a name="zh-cn_topic_0168797293_p256599"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="57.16%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797293_p5825169"><a name="zh-cn_topic_0168797293_p5825169"></a><a name="zh-cn_topic_0168797293_p5825169"></a>snat_rule对象。请参考<a href="#zh-cn_topic_0168797293_table161525103">表5</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 5**  snat\_rule字段说明

<a name="zh-cn_topic_0168797293_table161525103"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797293_row1725172181011"><th class="cellrowborder" valign="top" width="20.31%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797293_p1725119218105"><a name="zh-cn_topic_0168797293_p1725119218105"></a><a name="zh-cn_topic_0168797293_p1725119218105"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="22.11%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797293_p162517218107"><a name="zh-cn_topic_0168797293_p162517218107"></a><a name="zh-cn_topic_0168797293_p162517218107"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797293_p525182161010"><a name="zh-cn_topic_0168797293_p525182161010"></a><a name="zh-cn_topic_0168797293_p525182161010"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797293_row112519221010"><td class="cellrowborder" valign="top" width="20.31%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797293_p42513251017"><a name="zh-cn_topic_0168797293_p42513251017"></a><a name="zh-cn_topic_0168797293_p42513251017"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="22.11%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797293_p1225113212107"><a name="zh-cn_topic_0168797293_p1225113212107"></a><a name="zh-cn_topic_0168797293_p1225113212107"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797293_p102511291019"><a name="zh-cn_topic_0168797293_p102511291019"></a><a name="zh-cn_topic_0168797293_p102511291019"></a>SNAT规则的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797293_row125152161012"><td class="cellrowborder" valign="top" width="20.31%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797293_p625113241017"><a name="zh-cn_topic_0168797293_p625113241017"></a><a name="zh-cn_topic_0168797293_p625113241017"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.11%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797293_p152512024103"><a name="zh-cn_topic_0168797293_p152512024103"></a><a name="zh-cn_topic_0168797293_p152512024103"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797293_p152510211012"><a name="zh-cn_topic_0168797293_p152510211012"></a><a name="zh-cn_topic_0168797293_p152510211012"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797293_row13251172191013"><td class="cellrowborder" valign="top" width="20.31%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797293_p172667221018"><a name="zh-cn_topic_0168797293_p172667221018"></a><a name="zh-cn_topic_0168797293_p172667221018"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.11%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797293_p82666214109"><a name="zh-cn_topic_0168797293_p82666214109"></a><a name="zh-cn_topic_0168797293_p82666214109"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797293_p1726611251011"><a name="zh-cn_topic_0168797293_p1726611251011"></a><a name="zh-cn_topic_0168797293_p1726611251011"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797293_row226622101019"><td class="cellrowborder" valign="top" width="20.31%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797293_p162661929108"><a name="zh-cn_topic_0168797293_p162661929108"></a><a name="zh-cn_topic_0168797293_p162661929108"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.11%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797293_p02661226100"><a name="zh-cn_topic_0168797293_p02661226100"></a><a name="zh-cn_topic_0168797293_p02661226100"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797293_p42669211108"><a name="zh-cn_topic_0168797293_p42669211108"></a><a name="zh-cn_topic_0168797293_p42669211108"></a>规则使用的网络id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797293_row16266192191014"><td class="cellrowborder" valign="top" width="20.31%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797293_p182661326103"><a name="zh-cn_topic_0168797293_p182661326103"></a><a name="zh-cn_topic_0168797293_p182661326103"></a>source_type</p>
</td>
<td class="cellrowborder" valign="top" width="22.11%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797293_p126442387010"><a name="zh-cn_topic_0168797293_p126442387010"></a><a name="zh-cn_topic_0168797293_p126442387010"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797293_p172664291014"><a name="zh-cn_topic_0168797293_p172664291014"></a><a name="zh-cn_topic_0168797293_p172664291014"></a>0：VPC侧，可以指定network_id 或者cidr。</p>
<p id="zh-cn_topic_0168797293_p192667291014"><a name="zh-cn_topic_0168797293_p192667291014"></a><a name="zh-cn_topic_0168797293_p192667291014"></a>1：专线侧，只能指定cidr。</p>
<p id="zh-cn_topic_0168797293_p1026615271011"><a name="zh-cn_topic_0168797293_p1026615271011"></a><a name="zh-cn_topic_0168797293_p1026615271011"></a>不输入默认为0（VPC）。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797293_row1526617211109"><td class="cellrowborder" valign="top" width="20.31%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797293_p82661421103"><a name="zh-cn_topic_0168797293_p82661421103"></a><a name="zh-cn_topic_0168797293_p82661421103"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.11%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797293_p8266142121011"><a name="zh-cn_topic_0168797293_p8266142121011"></a><a name="zh-cn_topic_0168797293_p8266142121011"></a>String(4096)</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797293_ul1926613271020"></a><a name="zh-cn_topic_0168797293_ul1926613271020"></a><ul id="zh-cn_topic_0168797293_ul1926613271020"><li>功能说明：弹性公网IP的id，多个弹性公网IP使用逗号分隔。</li><li>取值范围：最大长度4096字节。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797293_row1326617261012"><td class="cellrowborder" valign="top" width="20.31%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797293_p10354521830"><a name="zh-cn_topic_0168797293_p10354521830"></a><a name="zh-cn_topic_0168797293_p10354521830"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="22.11%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797293_p103541210310"><a name="zh-cn_topic_0168797293_p103541210310"></a><a name="zh-cn_topic_0168797293_p103541210310"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797293_p33542215320"><a name="zh-cn_topic_0168797293_p33542215320"></a><a name="zh-cn_topic_0168797293_p33542215320"></a>SNAT规则的描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797293_row102666231019"><td class="cellrowborder" valign="top" width="20.31%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797293_p128220169310"><a name="zh-cn_topic_0168797293_p128220169310"></a><a name="zh-cn_topic_0168797293_p128220169310"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="22.11%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797293_p1882211161139"><a name="zh-cn_topic_0168797293_p1882211161139"></a><a name="zh-cn_topic_0168797293_p1882211161139"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797293_ul188226161339"></a><a name="zh-cn_topic_0168797293_ul188226161339"></a><ul id="zh-cn_topic_0168797293_ul188226161339"><li>功能说明：SNAT规则的状态。</li><li>取值范围：<a href="资源状态说明.md">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797293_row20266627104"><td class="cellrowborder" valign="top" width="20.31%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797293_p28247161232"><a name="zh-cn_topic_0168797293_p28247161232"></a><a name="zh-cn_topic_0168797293_p28247161232"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="22.11%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797293_p9716203515259"><a name="zh-cn_topic_0168797293_p9716203515259"></a><a name="zh-cn_topic_0168797293_p9716203515259"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797293_ul71858556358"></a><a name="zh-cn_topic_0168797293_ul71858556358"></a><ul id="zh-cn_topic_0168797293_ul71858556358"><li>解冻/冻结状态。</li><li>取值范围：<a name="zh-cn_topic_0168797293_ul11838172814409"></a><a name="zh-cn_topic_0168797293_ul11838172814409"></a><ul id="zh-cn_topic_0168797293_ul11838172814409"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797293_row826616212109"><td class="cellrowborder" valign="top" width="20.31%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797293_p1082419161231"><a name="zh-cn_topic_0168797293_p1082419161231"></a><a name="zh-cn_topic_0168797293_p1082419161231"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="22.11%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797293_p4824141611312"><a name="zh-cn_topic_0168797293_p4824141611312"></a><a name="zh-cn_topic_0168797293_p4824141611312"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797293_ul1482419162316"></a><a name="zh-cn_topic_0168797293_ul1482419162316"></a><ul id="zh-cn_topic_0168797293_ul1482419162316"><li>SNAT规则的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797293_row626642101011"><td class="cellrowborder" valign="top" width="20.31%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797293_p198246161738"><a name="zh-cn_topic_0168797293_p198246161738"></a><a name="zh-cn_topic_0168797293_p198246161738"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="22.11%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797293_p882414164320"><a name="zh-cn_topic_0168797293_p882414164320"></a><a name="zh-cn_topic_0168797293_p882414164320"></a>String(1024)</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797293_ul2824131615314"></a><a name="zh-cn_topic_0168797293_ul2824131615314"></a><ul id="zh-cn_topic_0168797293_ul2824131615314"><li>功能说明：弹性公网IP，多个弹性公网IP使用逗号分隔。</li><li>取值范围：最大长度1024字节。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797293_row126001334528"><td class="cellrowborder" valign="top" width="20.31%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797293_p68247165311"><a name="zh-cn_topic_0168797293_p68247165311"></a><a name="zh-cn_topic_0168797293_p68247165311"></a>freezed_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="22.11%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797293_p198241616236"><a name="zh-cn_topic_0168797293_p198241616236"></a><a name="zh-cn_topic_0168797293_p198241616236"></a>String(1024)</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797293_ul0824121619318"></a><a name="zh-cn_topic_0168797293_ul0824121619318"></a><ul id="zh-cn_topic_0168797293_ul0824121619318"><li>功能说明：冻结的弹性公网IP，多个冻结的弹性公网IP使用逗号分隔。</li><li>取值范围：最大长度1024字节。</li></ul>
</td>
</tr>
</tbody>
</table>

## 示例<a name="zh-cn_topic_0168797293_section10005551"></a>

-   请求样例
    1.  VPC 侧指定network\_id

        ```
        POST https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/snat_rules    
         { 
             "snat_rule": { 
                 "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8", 
                 "network_id": "eaad9cd6-2372-4be1-9535-9bd37210ae7b", 
                 "source_type":0,
                 "floating_ip_id": "bdc10a4c-d81a-41ec-adf7-de857f7c812a", 
                 "description": "my snat rule 01" 
             } 
         }
        ```

    1.  VPC侧指定CIDR

        ```
        POST /v2/d199ba7e0ba64899b2e81518104b1526/snat_rules  
         {       
            "snat_rule": { 
                  "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8", 
                  "cidr": "192.168.1.10/32", 
                  "source_type":0, 
                  "floating_ip_id": "bdc10a4c-d81a-41ec-adf7-de857f7c812a", 
                  "description": "my snat rule 01" 
             } 
         }
        ```

    1.  专线侧 指定CIDR

        ```
        POST https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/snat_rules 
          { 
               "snat_rule": {  
                  "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8", 
                  "cidr": "172.30.0.0/24", 
                  "source_type":1, 
                  "floating_ip_id": "bdc10a4c-d81a-41ec-adf7-de857f7c812a", 
                  "description": "my snat rule 01" 
               } 
           }
        ```



-   响应样例
    1.  VPC 侧指定network\_id的响应

        ```
        { 
             "snat_rule": { 
                 "floating_ip_id": "bdc10a4c-d81a-41ec-adf7-de857f7c812a", 
                 "status": "PENDING_CREATE", 
                 "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8", 
                 "admin_state_up": true, 
                 "network_id": "eaad9cd6-2372-4be1-9535-9bd37210ae7b", 
                 "description": "",
                 "source_type":0, 
                 "tenant_id": "27e25061336f4af590faeabeb7fcd9a3", 
                 "created_at": "2017-11-18 07:54:21.665430", 
                 "id": "5b95c675-69c2-4656-ba06-58ff72e1d338", 
                 "floating_ip_address": "5.21.11.226"
             } 
         }
        ```

    2.  VPC 侧指定CIDR的响应

        ```
        { 
             "snat_rule": { 
                 "floating_ip_id": "bdc10a4c-d81a-41ec-adf7-de857f7c812a", 
                 "status": "PENDING_CREATE", 
                 "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8", 
                 "admin_state_up": true, 
                 "cidr": "192.168.1.10/32", 
                 "description": "",
                 "source_type":0, 
                 "tenant_id": "27e25061336f4af590faeabeb7fcd9a3", 
                 "created_at": "2017-11-18 07:54:21.665430", 
                 "id": "5b95c675-69c2-4656-ba06-58ff72e1d338", 
                 "floating_ip_address": "5.21.11.226"
             } 
         }
        ```

    3.  专线侧指定CIDR的响应

        ```
        { 
             "snat_rule": { 
                 "floating_ip_id": "bdc10a4c-d81a-41ec-adf7-de857f7c812a", 
                 "status": "PENDING_CREATE", 
                 "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8", 
                 "admin_state_up": true, 
                 "cidr": "172.30.0.0/24", 
                 "description": "",
                 "source_type":1, 
                 "tenant_id": "27e25061336f4af590faeabeb7fcd9a3", 
                 "created_at": "2017-11-18 07:54:21.665430", 
                 "id": "5b95c675-69c2-4656-ba06-58ff72e1d338", 
                 "floating_ip_address": "5.21.11.226"
             } 
         }
        ```



## 状态码<a name="zh-cn_topic_0168797293_section5143287"></a>

请参考[状态码](状态码.md)。

