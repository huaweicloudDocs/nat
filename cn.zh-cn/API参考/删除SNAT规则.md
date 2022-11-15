# 删除SNAT规则<a name="DeleteNatGatewaySnatRule"></a>

## 功能介绍<a name="section1133717143317"></a>

删除指定的SNAT规则。

## 调试<a name="section7346131411313"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=nat&api=DeleteNatGatewaySnatRule)中调试该接口。

## URI<a name="section1435851413319"></a>

DELETE /v2/\{project\_id\}/nat\_gateways/\{nat\_gateway\_id\}/snat\_rules/\{snat\_rule\_id\}

**表 1**  路径参数

<a name="table4372814163115"></a>
<table><thead align="left"><tr id="row1636981423117"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1137571453110"><a name="p1137571453110"></a><a name="p1137571453110"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p1637961423116"><a name="p1637961423116"></a><a name="p1637961423116"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p143861514113117"><a name="p143861514113117"></a><a name="p143861514113117"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p12392414183119"><a name="p12392414183119"></a><a name="p12392414183119"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row136961473114"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p33989143315"><a name="p33989143315"></a><a name="p33989143315"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p540317142316"><a name="p540317142316"></a><a name="p540317142316"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1540811443118"><a name="p1540811443118"></a><a name="p1540811443118"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1041351415318"><a name="p1041351415318"></a><a name="p1041351415318"></a>项目的ID。</p>
<p id="p84178143317"><a name="p84178143317"></a><a name="p84178143317"></a>最小长度：<strong id="b17419171443118"><a name="b17419171443118"></a><a name="b17419171443118"></a>1</strong></p>
<p id="p742341453114"><a name="p742341453114"></a><a name="p742341453114"></a>最大长度：<strong id="b3425914163118"><a name="b3425914163118"></a><a name="b3425914163118"></a>36</strong></p>
<p id="p2562026131319"><a name="p2562026131319"></a><a name="p2562026131319"></a>获取方法详见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row73691614103112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p2428614193114"><a name="p2428614193114"></a><a name="p2428614193114"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p14433314203113"><a name="p14433314203113"></a><a name="p14433314203113"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p134388148311"><a name="p134388148311"></a><a name="p134388148311"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p16443171403119"><a name="p16443171403119"></a><a name="p16443171403119"></a>公网NAT网关实例的ID。</p>
<p id="p344921493112"><a name="p344921493112"></a><a name="p344921493112"></a>长度：<strong id="b7451181418312"><a name="b7451181418312"></a><a name="b7451181418312"></a>36</strong></p>
</td>
</tr>
<tr id="row1369181412313"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p44597146311"><a name="p44597146311"></a><a name="p44597146311"></a>snat_rule_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p04641214153110"><a name="p04641214153110"></a><a name="p04641214153110"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1046851493115"><a name="p1046851493115"></a><a name="p1046851493115"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1447411415317"><a name="p1447411415317"></a><a name="p1447411415317"></a>SNAT规则的ID。</p>
<p id="p1747981433118"><a name="p1747981433118"></a><a name="p1747981433118"></a>长度：<strong id="b948181412313"><a name="b948181412313"></a><a name="b948181412313"></a>36</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section1149011411311"></a>

**表 2**  请求Header参数

<a name="zh-cn_topic_0297140332_HeaderParameter"></a>
<table><thead align="left"><tr id="row9496101493110"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1650141413312"><a name="p1650141413312"></a><a name="p1650141413312"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p1850515147317"><a name="p1850515147317"></a><a name="p1850515147317"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1511121443119"><a name="p1511121443119"></a><a name="p1511121443119"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p551651453118"><a name="p551651453118"></a><a name="p551651453118"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row9496181415311"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p5521714203116"><a name="p5521714203116"></a><a name="p5521714203116"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p35265141311"><a name="p35265141311"></a><a name="p35265141311"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p2531214143117"><a name="p2531214143117"></a><a name="p2531214143117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p2053691413112"><a name="p2053691413112"></a><a name="p2053691413112"></a>用户Token。用户Token也就是调用获取用户Token获取请求认证接口的响应值，该接口是唯一不需要认证的接口。请求响应成功后在响应消息头中包含的“X-Subject-Token”的值即为Token值。</p>
<p id="p75406149318"><a name="p75406149318"></a><a name="p75406149318"></a>最小长度：<strong id="b65411914103117"><a name="b65411914103117"></a><a name="b65411914103117"></a>1</strong></p>
<p id="p0545141453112"><a name="p0545141453112"></a><a name="p0545141453112"></a>最大长度：<strong id="b12546214183118"><a name="b12546214183118"></a><a name="b12546214183118"></a>10240</strong></p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section25494141316"></a>

无

## 请求示例<a name="section205601014113119"></a>

```
DELETE https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/nat_gateways/f4dfea98-874a-46f7-aa2a-fb348d0ceb02/snat_rules/a78fb3eb-1654-4710-8742-3fc49d5f04f8

  
```

## 响应示例<a name="section1958010148318"></a>

无

## 状态码<a name="section19591414113119"></a>

<a name="zh-cn_topic_0297140332_status_code"></a>
<table><thead align="left"><tr id="row17596101414311"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p460017141315"><a name="p460017141315"></a><a name="p460017141315"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p106041414143115"><a name="p106041414143115"></a><a name="p106041414143115"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row155960146310"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1460921413312"><a name="p1460921413312"></a><a name="p1460921413312"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p76146146315"><a name="p76146146315"></a><a name="p76146146315"></a>删除SNAT规则成功。</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section1862017143312"></a>

请参见[错误码](错误码.md)。

