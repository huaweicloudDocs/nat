# 创建SNAT规则<a name="ZH-CN_TOPIC_0201533683"></a>

## 功能介绍<a name="section45647471"></a>

创建SNAT规则。

>![](public_sys-resources/icon-note.gif) **说明：**   
>创建规则时，要求网关状态status = "ACTIVE"，要求网关管理员状态admin\_state\_up = True。  

## URI<a name="section8174056"></a>

POST /v2.0/snat\_rules

## 请求消息<a name="section58118839"></a>

请求参数如[表1](#table10267194320114)所示。

**表 1**  请求参数

<a name="table10267194320114"></a>
<table><thead align="left"><tr id="row6376174317113"><th class="cellrowborder" valign="top" width="23.72%" id="mcps1.2.5.1.1"><p id="p83761431417"><a name="p83761431417"></a><a name="p83761431417"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.219999999999999%" id="mcps1.2.5.1.2"><p id="p19376144311113"><a name="p19376144311113"></a><a name="p19376144311113"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.56%" id="mcps1.2.5.1.3"><p id="p1237644310118"><a name="p1237644310118"></a><a name="p1237644310118"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="49.5%" id="mcps1.2.5.1.4"><p id="p19376243814"><a name="p19376243814"></a><a name="p19376243814"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row113769431511"><td class="cellrowborder" valign="top" width="23.72%" headers="mcps1.2.5.1.1 "><p id="p143761543316"><a name="p143761543316"></a><a name="p143761543316"></a>snat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="8.219999999999999%" headers="mcps1.2.5.1.2 "><p id="p143761543914"><a name="p143761543914"></a><a name="p143761543914"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.56%" headers="mcps1.2.5.1.3 "><p id="p3376143212"><a name="p3376143212"></a><a name="p3376143212"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="49.5%" headers="mcps1.2.5.1.4 "><p id="p63766431210"><a name="p63766431210"></a><a name="p63766431210"></a>snat_rule对象。详见<a href="#table628219431019">表2</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  snat\_rule字段说明

<a name="table628219431019"></a>
<table><thead align="left"><tr id="row5376743718"><th class="cellrowborder" valign="top" width="22.57%" id="mcps1.2.5.1.1"><p id="p4376134314114"><a name="p4376134314114"></a><a name="p4376134314114"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.649999999999999%" id="mcps1.2.5.1.2"><p id="p43767431317"><a name="p43767431317"></a><a name="p43767431317"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.9%" id="mcps1.2.5.1.3"><p id="p3376643415"><a name="p3376643415"></a><a name="p3376643415"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.879999999999995%" id="mcps1.2.5.1.4"><p id="p5376154315117"><a name="p5376154315117"></a><a name="p5376154315117"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row9376643318"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="p33764431917"><a name="p33764431917"></a><a name="p33764431917"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="p143761343014"><a name="p143761343014"></a><a name="p143761343014"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="p143761143518"><a name="p143761143518"></a><a name="p143761143518"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="p15376243712"><a name="p15376243712"></a><a name="p15376243712"></a>所属NAT网关的id。</p>
</td>
</tr>
<tr id="row73761743512"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="p18522143016410"><a name="p18522143016410"></a><a name="p18522143016410"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="p115225301847"><a name="p115225301847"></a><a name="p115225301847"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="p9522830441"><a name="p9522830441"></a><a name="p9522830441"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="p115223302049"><a name="p115223302049"></a><a name="p115223302049"></a>规则使用的网络id。与cidr参数二选一。</p>
</td>
</tr>
<tr id="row237617432112"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="p56167320519"><a name="p56167320519"></a><a name="p56167320519"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="p11616163653"><a name="p11616163653"></a><a name="p11616163653"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="p7616132519"><a name="p7616132519"></a><a name="p7616132519"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="p96161631513"><a name="p96161631513"></a><a name="p96161631513"></a>cidr，可以是网段或者主机格式，与network_id参数二选一。</p>
<p id="p1861612320514"><a name="p1861612320514"></a><a name="p1861612320514"></a>Source_type=0时，cidr必须是vpc 子网网段的子集(不能相等）;</p>
<p id="p20616431753"><a name="p20616431753"></a><a name="p20616431753"></a>Source_type=1时，cidr必须指定专线侧网段。</p>
</td>
</tr>
<tr id="row1637684317119"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="p1437611434114"><a name="p1437611434114"></a><a name="p1437611434114"></a>source_type</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="p1537617431518"><a name="p1537617431518"></a><a name="p1537617431518"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="p537624314120"><a name="p537624314120"></a><a name="p537624314120"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="p037614433118"><a name="p037614433118"></a><a name="p037614433118"></a>0：VPC侧，可以指定network_id 或者cidr</p>
<p id="p1937614436114"><a name="p1937614436114"></a><a name="p1937614436114"></a>1：专线侧，只能指定cidr</p>
<p id="p1137616431711"><a name="p1137616431711"></a><a name="p1137616431711"></a>不输入默认为0（VPC）</p>
</td>
</tr>
<tr id="row19376114318117"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="p63761431119"><a name="p63761431119"></a><a name="p63761431119"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="p183763431012"><a name="p183763431012"></a><a name="p183763431012"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="p173763431417"><a name="p173763431417"></a><a name="p173763431417"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="p03765431213"><a name="p03765431213"></a><a name="p03765431213"></a>功能说明：弹性公网IP的id，多个弹性公网IP使用逗号分隔。</p>
<p id="p123761343915"><a name="p123761343915"></a><a name="p123761343915"></a>取值范围：最大长度4096字节。</p>
<p id="p103761343515"><a name="p103761343515"></a><a name="p103761343515"></a>约束：弹性公网IP的id个数不能超过20个。</p>
<p id="p1337614318111"><a name="p1337614318111"></a><a name="p1337614318111"></a>获取弹性公网IP的id的方法请参考<a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090598.html" target="_blank" rel="noopener noreferrer">查询弹性公网IP列表</a>。</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section53307511"></a>

响应参数如[表3](#table64245911)所示。

**表 3**  响应参数

<a name="table64245911"></a>
<table><thead align="left"><tr id="row15388566"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p38514356"><a name="p38514356"></a><a name="p38514356"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="22.67%" id="mcps1.2.4.1.2"><p id="p32655106"><a name="p32655106"></a><a name="p32655106"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.330000000000005%" id="mcps1.2.4.1.3"><p id="p38657103"><a name="p38657103"></a><a name="p38657103"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row44217630"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p24858302"><a name="p24858302"></a><a name="p24858302"></a>snat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="22.67%" headers="mcps1.2.4.1.2 "><p id="p256599"><a name="p256599"></a><a name="p256599"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="57.330000000000005%" headers="mcps1.2.4.1.3 "><p id="p5825169"><a name="p5825169"></a><a name="p5825169"></a>snat_rule对象。详见<a href="#table161525103">表4</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  snat\_rule字段说明

<a name="table161525103"></a>
<table><thead align="left"><tr id="row1725172181011"><th class="cellrowborder" valign="top" width="20.05%" id="mcps1.2.4.1.1"><p id="p1725119218105"><a name="p1725119218105"></a><a name="p1725119218105"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="22.37%" id="mcps1.2.4.1.2"><p id="p162517218107"><a name="p162517218107"></a><a name="p162517218107"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.4.1.3"><p id="p525182161010"><a name="p525182161010"></a><a name="p525182161010"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row112519221010"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="p42513251017"><a name="p42513251017"></a><a name="p42513251017"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="22.37%" headers="mcps1.2.4.1.2 "><p id="p1225113212107"><a name="p1225113212107"></a><a name="p1225113212107"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><p id="p102511291019"><a name="p102511291019"></a><a name="p102511291019"></a>SNAT规则的id。</p>
</td>
</tr>
<tr id="row125152161012"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="p625113241017"><a name="p625113241017"></a><a name="p625113241017"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.37%" headers="mcps1.2.4.1.2 "><p id="p152512024103"><a name="p152512024103"></a><a name="p152512024103"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><p id="p152510211012"><a name="p152510211012"></a><a name="p152510211012"></a>项目的ID。</p>
</td>
</tr>
<tr id="row13251172191013"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="p172667221018"><a name="p172667221018"></a><a name="p172667221018"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.37%" headers="mcps1.2.4.1.2 "><p id="p82666214109"><a name="p82666214109"></a><a name="p82666214109"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><p id="p1726611251011"><a name="p1726611251011"></a><a name="p1726611251011"></a>所属NAT网关的id。</p>
</td>
</tr>
<tr id="row226622101019"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="p162661929108"><a name="p162661929108"></a><a name="p162661929108"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.37%" headers="mcps1.2.4.1.2 "><p id="p02661226100"><a name="p02661226100"></a><a name="p02661226100"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><p id="p42669211108"><a name="p42669211108"></a><a name="p42669211108"></a>规则使用的网络id。</p>
</td>
</tr>
<tr id="row1266724105"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="p1266132131018"><a name="p1266132131018"></a><a name="p1266132131018"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="22.37%" headers="mcps1.2.4.1.2 "><p id="p5266122121017"><a name="p5266122121017"></a><a name="p5266122121017"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><p id="p10266122191010"><a name="p10266122191010"></a><a name="p10266122191010"></a>cidr，vpc 子网网段的子集或专线侧网段。</p>
</td>
</tr>
<tr id="row16266192191014"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="p182661326103"><a name="p182661326103"></a><a name="p182661326103"></a>source_type</p>
</td>
<td class="cellrowborder" valign="top" width="22.37%" headers="mcps1.2.4.1.2 "><p id="p62661213102"><a name="p62661213102"></a><a name="p62661213102"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><p id="p172664291014"><a name="p172664291014"></a><a name="p172664291014"></a>0：VPC侧，可以指定network_id 或者cidr</p>
<p id="p192667291014"><a name="p192667291014"></a><a name="p192667291014"></a>1：专线侧，只能指定cidr</p>
<p id="p1026615271011"><a name="p1026615271011"></a><a name="p1026615271011"></a>不输入默认为0（VPC）</p>
</td>
</tr>
<tr id="row1526617211109"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="p82661421103"><a name="p82661421103"></a><a name="p82661421103"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.37%" headers="mcps1.2.4.1.2 "><p id="p8266142121011"><a name="p8266142121011"></a><a name="p8266142121011"></a>String(4096)</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><a name="ul1926613271020"></a><a name="ul1926613271020"></a><ul id="ul1926613271020"><li>功能说明：弹性公网IP的id，多个弹性公网IP使用逗号分隔。</li><li>取值范围：最大长度4096字节。</li></ul>
</td>
</tr>
<tr id="row1326617261012"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="p5266123104"><a name="p5266123104"></a><a name="p5266123104"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="22.37%" headers="mcps1.2.4.1.2 "><p id="p19266427107"><a name="p19266427107"></a><a name="p19266427107"></a>String(1024)</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><a name="ul026610212101"></a><a name="ul026610212101"></a><ul id="ul026610212101"><li>功能说明：弹性公网IP，多个弹性公网IP使用逗号分隔。</li><li>取值范围：最大长度1024字节。</li></ul>
</td>
</tr>
<tr id="row20266627104"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="p1426682131019"><a name="p1426682131019"></a><a name="p1426682131019"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="22.37%" headers="mcps1.2.4.1.2 "><p id="p7266202101010"><a name="p7266202101010"></a><a name="p7266202101010"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><a name="ul132663212108"></a><a name="ul132663212108"></a><ul id="ul132663212108"><li>功能说明：SNAT规则的状态。</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="row826616212109"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="p226611211104"><a name="p226611211104"></a><a name="p226611211104"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="22.37%" headers="mcps1.2.4.1.2 "><p id="p1764614265487"><a name="p1764614265487"></a><a name="p1764614265487"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><a name="ul71858556358"></a><a name="ul71858556358"></a><ul id="ul71858556358"><li>解冻/冻结状态。</li><li>取值范围：<a name="ul11838172814409"></a><a name="ul11838172814409"></a><ul id="ul11838172814409"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="row626642101011"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="p18266122141014"><a name="p18266122141014"></a><a name="p18266122141014"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="22.37%" headers="mcps1.2.4.1.2 "><p id="p32669214104"><a name="p32669214104"></a><a name="p32669214104"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.4.1.3 "><a name="ul1726613220108"></a><a name="ul1726613220108"></a><ul id="ul1726613220108"><li>SNAT规则的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</li></ul>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section10005551"></a>

-   请求样例
    1.  VPC 侧指定network\_id

        ```
        POST https://{Endpoint}/v2.0/snat_rules 
        {
            "snat_rule": {
                "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
                "network_id": "eaad9cd6-2372-4be1-9535-9bd37210ae7b",
                "source_type":0,
                "floating_ip_id": "bdc10a4c-d81a-41ec-adf7-de857f7c812a"
            }
        }
        ```

    1.  VPC侧指定CIDR

        ```
        POST https://{Endpoint}/v2.0/snat_rules
        {      
           "snat_rule": {
                 "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
                 "cidr": "192.168.1.10/32",
                 "source_type":0,
                 "floating_ip_id": "bdc10a4c-d81a-41ec-adf7-de857f7c812a"
              }
          }
        ```

    1.  专线侧 指定CIDR

        ```
        POST https://{Endpoint}/v2.0/snat_rules 
         {
              "snat_rule": { 
                 "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
                 "cidr": "172.30.0.0/24",
                 "source_type":1,
                 "floating_ip_id": "bdc10a4c-d81a-41ec-adf7-de857f7c812a"
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
                 "cidr": null, 
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
                 "source_type":1, 
                 "tenant_id": "27e25061336f4af590faeabeb7fcd9a3", 
                 "created_at": "2017-11-18 07:54:21.665430", 
                 "id": "5b95c675-69c2-4656-ba06-58ff72e1d338", 
                 "floating_ip_address": "5.21.11.226"
             } 
         }
        ```



## 状态码<a name="section5143287"></a>

请参考[状态码](状态码.md)。

