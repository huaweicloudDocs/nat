# 查询指定的SNAT规则详情<a name="ShowNatGatewaySnatRule"></a>

## 功能介绍<a name="section1573895517301"></a>

查询指定的SNAT规则详情。

## 接口约束<a name="section127451755153017"></a>

null

## 调试<a name="section18752155518306"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=nat&api=ShowNatGatewaySnatRule)中调试该接口。

## URI<a name="section876118554309"></a>

GET /v2/\{project\_id\}/snat\_rules/\{snat\_rule\_id\}

**表 1**  路径参数

<a name="table4769125520303"></a>
<table><thead align="left"><tr id="row1767135510301"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p16771185503013"><a name="p16771185503013"></a><a name="p16771185503013"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p5774205533015"><a name="p5774205533015"></a><a name="p5774205533015"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p20778195573010"><a name="p20778195573010"></a><a name="p20778195573010"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p77812556307"><a name="p77812556307"></a><a name="p77812556307"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row476735563014"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p17786135583015"><a name="p17786135583015"></a><a name="p17786135583015"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p77908557304"><a name="p77908557304"></a><a name="p77908557304"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p27931655123014"><a name="p27931655123014"></a><a name="p27931655123014"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p379711550302"><a name="p379711550302"></a><a name="p379711550302"></a>项目的ID。</p>
<p id="p5801755133019"><a name="p5801755133019"></a><a name="p5801755133019"></a>最小长度：<strong id="b1180295513018"><a name="b1180295513018"></a><a name="b1180295513018"></a>1</strong></p>
<p id="p380415543013"><a name="p380415543013"></a><a name="p380415543013"></a>最大长度：<strong id="b380519554307"><a name="b380519554307"></a><a name="b380519554307"></a>36</strong></p>
<p id="p2562026131319"><a name="p2562026131319"></a><a name="p2562026131319"></a>获取方法详见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row1076795513012"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p108082055163014"><a name="p108082055163014"></a><a name="p108082055163014"></a>snat_rule_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p981145583015"><a name="p981145583015"></a><a name="p981145583015"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1681415518301"><a name="p1681415518301"></a><a name="p1681415518301"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p198182555307"><a name="p198182555307"></a><a name="p198182555307"></a>SNAT规则的ID。</p>
<p id="p148225552306"><a name="p148225552306"></a><a name="p148225552306"></a>长度：<strong id="b20823155519304"><a name="b20823155519304"></a><a name="b20823155519304"></a>36</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section98301855193012"></a>

**表 2**  请求Header参数

<a name="zh-cn_topic_0297140330_HeaderParameter"></a>
<table><thead align="left"><tr id="row48331255153010"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p28391555173012"><a name="p28391555173012"></a><a name="p28391555173012"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p684325553016"><a name="p684325553016"></a><a name="p684325553016"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p0846115543012"><a name="p0846115543012"></a><a name="p0846115543012"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p6850155123019"><a name="p6850155123019"></a><a name="p6850155123019"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row18833175583013"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p68531755113019"><a name="p68531755113019"></a><a name="p68531755113019"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p11856175593019"><a name="p11856175593019"></a><a name="p11856175593019"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1860135563013"><a name="p1860135563013"></a><a name="p1860135563013"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p138642055193011"><a name="p138642055193011"></a><a name="p138642055193011"></a>用户Token。用户Token也就是调用获取用户Token获取请求认证接口的响应值，该接口是唯一不需要认证的接口。请求响应成功后在响应消息头中包含的“X-Subject-Token”的值即为Token值。</p>
<p id="p9868555163017"><a name="p9868555163017"></a><a name="p9868555163017"></a>最小长度：<strong id="b1886945516301"><a name="b1886945516301"></a><a name="b1886945516301"></a>1</strong></p>
<p id="p1987175510303"><a name="p1987175510303"></a><a name="p1987175510303"></a>最大长度：<strong id="b10872165513011"><a name="b10872165513011"></a><a name="b10872165513011"></a>10240</strong></p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section17876755123016"></a>

**状态码： 200**

**表 3**  响应Body参数

<a name="zh-cn_topic_0297140330_responseParameter"></a>
<table><thead align="left"><tr id="row288295513304"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p3886165516307"><a name="p3886165516307"></a><a name="p3886165516307"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p7890105511308"><a name="p7890105511308"></a><a name="p7890105511308"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p189418553309"><a name="p189418553309"></a><a name="p189418553309"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row48821655153018"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p58971655103015"><a name="p58971655103015"></a><a name="p58971655103015"></a>snat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1901135543015"><a name="p1901135543015"></a><a name="p1901135543015"></a><a href="#zh-cn_topic_0297140330_response_NatGatewaySnatRuleResponseBody">NatGatewaySnatRuleResponseBody</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1190475516307"><a name="p1190475516307"></a><a name="p1190475516307"></a>SNAT规则的响应体。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  NatGatewaySnatRuleResponseBody

<a name="zh-cn_topic_0297140330_response_NatGatewaySnatRuleResponseBody"></a>
<table><thead align="left"><tr id="row390865512301"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p14913145583018"><a name="p14913145583018"></a><a name="p14913145583018"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1291713558306"><a name="p1291713558306"></a><a name="p1291713558306"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1920155518305"><a name="p1920155518305"></a><a name="p1920155518305"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row79083551309"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p49253552302"><a name="p49253552302"></a><a name="p49253552302"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1928175519301"><a name="p1928175519301"></a><a name="p1928175519301"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p7932205517303"><a name="p7932205517303"></a><a name="p7932205517303"></a>SNAT规则的ID。</p>
<p id="p129352550303"><a name="p129352550303"></a><a name="p129352550303"></a>长度：<strong id="b493675503019"><a name="b493675503019"></a><a name="b493675503019"></a>36</strong></p>
</td>
</tr>
<tr id="row2908155103017"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p79421557301"><a name="p79421557301"></a><a name="p79421557301"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p09461655103020"><a name="p09461655103020"></a><a name="p09461655103020"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1949455163018"><a name="p1949455163018"></a><a name="p1949455163018"></a>项目的ID。</p>
</td>
</tr>
<tr id="row590845523011"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p16953855103012"><a name="p16953855103012"></a><a name="p16953855103012"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p695713551304"><a name="p695713551304"></a><a name="p695713551304"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p396395516300"><a name="p396395516300"></a><a name="p396395516300"></a>公网NAT网关实例的ID。</p>
<p id="p4966205553014"><a name="p4966205553014"></a><a name="p4966205553014"></a>长度：<strong id="b149685559308"><a name="b149685559308"></a><a name="b149685559308"></a>36</strong></p>
</td>
</tr>
<tr id="row11908455163014"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p697445515303"><a name="p697445515303"></a><a name="p697445515303"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p99781655103019"><a name="p99781655103019"></a><a name="p99781655103019"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p698275503013"><a name="p698275503013"></a><a name="p698275503013"></a>cidr，可以是网段或者主机格式，与network_id参数二选一。source_type=0时，cidr必须是vpc 子网网段的子集（不能相等）; source_type=1时，cidr必须指定专线侧网段。</p>
<p id="p49851355113014"><a name="p49851355113014"></a><a name="p49851355113014"></a>最小长度：<strong id="b498612551305"><a name="b498612551305"></a><a name="b498612551305"></a>9</strong></p>
<p id="p13989135519309"><a name="p13989135519309"></a><a name="p13989135519309"></a>最大长度：<strong id="b09911755173011"><a name="b09911755173011"></a><a name="b09911755173011"></a>39</strong></p>
</td>
</tr>
<tr id="row49087551305"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p5994175593018"><a name="p5994175593018"></a><a name="p5994175593018"></a>source_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p799805553012"><a name="p799805553012"></a><a name="p799805553012"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><a name="ul112891112318"></a><a name="ul112891112318"></a><ul id="ul112891112318"><li>0：VPC侧，可以指定network_id 或者cidr</li><li>1：专线侧，只能指定cidr</li></ul>
<p id="p135656113014"><a name="p135656113014"></a><a name="p135656113014"></a>缺省值：<strong id="b1162056143015"><a name="b1162056143015"></a><a name="b1162056143015"></a>0</strong></p>
</td>
</tr>
<tr id="row5908105519307"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p381756183018"><a name="p381756183018"></a><a name="p381756183018"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1111205683017"><a name="p1111205683017"></a><a name="p1111205683017"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1814856153017"><a name="p1814856153017"></a><a name="p1814856153017"></a>功能说明：弹性公网IP的id，多个弹性公网IP的id使用逗号分隔。取值范围：最大长度4096字节。</p>
</td>
</tr>
<tr id="row8908125533016"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4181656163011"><a name="p4181656163011"></a><a name="p4181656163011"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p92195614301"><a name="p92195614301"></a><a name="p92195614301"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12256560309"><a name="p12256560309"></a><a name="p12256560309"></a>SNAT规则的描述，长度限制为255。</p>
<p id="p628175693015"><a name="p628175693015"></a><a name="p628175693015"></a>最大长度：<strong id="b1829135612305"><a name="b1829135612305"></a><a name="b1829135612305"></a>255</strong></p>
</td>
</tr>
<tr id="row1908195517309"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p153215683019"><a name="p153215683019"></a><a name="p153215683019"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p83518564304"><a name="p83518564304"></a><a name="p83518564304"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p114075615303"><a name="p114075615303"></a><a name="p114075615303"></a>功能说明：SNAT规则的状态。</p>
<p id="p543195612302"><a name="p543195612302"></a><a name="p543195612302"></a>枚举值：</p>
<a name="ul164705617306"></a><a name="ul164705617306"></a><ul id="ul164705617306"><li><strong id="b1851135616306"><a name="b1851135616306"></a><a name="b1851135616306"></a>ACTIVE</strong></li><li><strong id="b125535653016"><a name="b125535653016"></a><a name="b125535653016"></a>PENDING_CREATE</strong></li><li><strong id="b3591056163019"><a name="b3591056163019"></a><a name="b3591056163019"></a>PENDING_UPDATE</strong></li><li><strong id="b1462185683017"><a name="b1462185683017"></a><a name="b1462185683017"></a>PENDING_DELETE</strong></li><li><strong id="b13657566302"><a name="b13657566302"></a><a name="b13657566302"></a>EIP_FREEZED</strong></li><li><strong id="b668656103018"><a name="b668656103018"></a><a name="b668656103018"></a>INACTIVE</strong></li></ul>
</td>
</tr>
<tr id="row69091955153018"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p18721256123010"><a name="p18721256123010"></a><a name="p18721256123010"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p87616566309"><a name="p87616566309"></a><a name="p87616566309"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p118145611300"><a name="p118145611300"></a><a name="p118145611300"></a>SNAT规则的创建时间，遵循UTC时间，格式是yyyy-mm-ddThh:mm:ssZ。最小长度：<strong id="b1886185663018"><a name="b1886185663018"></a><a name="b1886185663018"></a>1</strong></p>
<p id="p188816569302"><a name="p188816569302"></a><a name="p188816569302"></a>最大长度：<strong id="b109075613012"><a name="b109075613012"></a><a name="b109075613012"></a>36</strong></p>
</td>
</tr>
<tr id="row13909185523016"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p292156143012"><a name="p292156143012"></a><a name="p292156143012"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p796125683011"><a name="p796125683011"></a><a name="p796125683011"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p51011856113010"><a name="p51011856113010"></a><a name="p51011856113010"></a>规则使用的网络id。与cidr参数二选一。</p>
<p id="p16104856123012"><a name="p16104856123012"></a><a name="p16104856123012"></a>长度：<strong id="b1410595614305"><a name="b1410595614305"></a><a name="b1410595614305"></a>36</strong></p>
</td>
</tr>
<tr id="row29091055123019"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1511211569305"><a name="p1511211569305"></a><a name="p1511211569305"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p20115956173019"><a name="p20115956173019"></a><a name="p20115956173019"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p212085617304"><a name="p212085617304"></a><a name="p212085617304"></a>解冻/冻结状态。取值范围：</p>
<a name="ul4123356163017"></a><a name="ul4123356163017"></a><ul id="ul4123356163017"><li>"true"：解冻</li><li>"false"：冻结</li></ul>
</td>
</tr>
<tr id="row2909165516307"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1813425612308"><a name="p1813425612308"></a><a name="p1813425612308"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p7137056173019"><a name="p7137056173019"></a><a name="p7137056173019"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2141135616302"><a name="p2141135616302"></a><a name="p2141135616302"></a>功能说明：弹性公网IP，多个弹性公网IP使用逗号分隔。取值范围：最大长度1024字节。</p>
</td>
</tr>
<tr id="row390920555306"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1145135613010"><a name="p1145135613010"></a><a name="p1145135613010"></a>freezed_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p18150185614308"><a name="p18150185614308"></a><a name="p18150185614308"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p121537569301"><a name="p121537569301"></a><a name="p121537569301"></a>功能说明：冻结的弹性公网IP，多个冻结的弹性公网IP使用逗号分隔。取值范围：最大长度1024字节。</p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section11157956123018"></a>

```
GET https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/snat_rules/5b95c675-69c2-4656-ba06-58ff72e1d33

  
```

## 响应示例<a name="section1171105613010"></a>

**状态码： 200**

查询SNAT规则成功。

```
{
  "snat_rule" : {
    "floating_ip_id" : "bdc10a4c-d81a-41ec-adf7-de857f7c812a",
    "status" : "ACTIVE",
    "nat_gateway_id" : "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
    "admin_state_up" : true,
    "network_id" : "eaad9cd6-2372-4be1-9535-9bd37210ae7b",
    "source_type" : 0,
    "tenant_id" : "d199ba7e0ba64899b2e81518104b1526",
    "created_at" : "2017-11-18 07:54:21.665430",
    "id" : "5b95c675-69c2-4656-ba06-58ff72e1d338",
    "floating_ip_address" : "5.21.11.226",
    "freezed_ip_address" : "",
    "description" : "my snat rule 01"
  }
}
```

## 状态码<a name="section72351156123016"></a>

<a name="zh-cn_topic_0297140330_status_code"></a>
<table><thead align="left"><tr id="row823965612303"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p9242135618303"><a name="p9242135618303"></a><a name="p9242135618303"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p13246356133014"><a name="p13246356133014"></a><a name="p13246356133014"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row22392569303"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1125065653018"><a name="p1125065653018"></a><a name="p1125065653018"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1525395611309"><a name="p1525395611309"></a><a name="p1525395611309"></a>查询SNAT规则成功。</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section9255856123010"></a>

请参见[错误码](错误码.md)。

