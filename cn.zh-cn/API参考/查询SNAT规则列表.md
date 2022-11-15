# 查询SNAT规则列表<a name="ListNatGatewaySnatRules"></a>

## 功能介绍<a name="section670111234286"></a>

查询SNAT规则列表。

## 接口约束<a name="section187021023142818"></a>

可以在URI后面用'?'和'&'添加不同的查询条件组合。支持参数说明中所有非必选参数过滤，请参考请求样例。

## 调试<a name="section47049239284"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=nat&api=ListNatGatewaySnatRules)中调试该接口。

## URI<a name="section1770632362819"></a>

GET /v2/\{project\_id\}/snat\_rules

**表 1**  路径参数

<a name="table3716182322816"></a>
<table><thead align="left"><tr id="row1271310231284"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p12718192318282"><a name="p12718192318282"></a><a name="p12718192318282"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p971952372818"><a name="p971952372818"></a><a name="p971952372818"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p17720112311285"><a name="p17720112311285"></a><a name="p17720112311285"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p87211723192818"><a name="p87211723192818"></a><a name="p87211723192818"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row147141723142819"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p13722172312285"><a name="p13722172312285"></a><a name="p13722172312285"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p197237236282"><a name="p197237236282"></a><a name="p197237236282"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p97247236280"><a name="p97247236280"></a><a name="p97247236280"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p272562319285"><a name="p272562319285"></a><a name="p272562319285"></a>项目的ID。</p>
<p id="p197251823182817"><a name="p197251823182817"></a><a name="p197251823182817"></a>最小长度：<strong id="b20726192316281"><a name="b20726192316281"></a><a name="b20726192316281"></a>1</strong></p>
<p id="p972617237288"><a name="p972617237288"></a><a name="p972617237288"></a>最大长度：<strong id="b072632372817"><a name="b072632372817"></a><a name="b072632372817"></a>36</strong></p>
<p id="p2562026131319"><a name="p2562026131319"></a><a name="p2562026131319"></a>获取方法详见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  Query参数

<a name="table173182310283"></a>
<table><thead align="left"><tr id="row272822318287"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1473118235282"><a name="p1473118235282"></a><a name="p1473118235282"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p97321323142813"><a name="p97321323142813"></a><a name="p97321323142813"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p2733172318284"><a name="p2733172318284"></a><a name="p2733172318284"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p18734102382818"><a name="p18734102382818"></a><a name="p18734102382818"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row16729152317280"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p18734112392812"><a name="p18734112392812"></a><a name="p18734112392812"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p27351023122810"><a name="p27351023122810"></a><a name="p27351023122810"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p573652382812"><a name="p573652382812"></a><a name="p573652382812"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p12737132316283"><a name="p12737132316283"></a><a name="p12737132316283"></a>解冻/冻结状态。取值范围： "true"：解冻 "false"：冻结</p>
</td>
</tr>
<tr id="row16729923192815"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p673722313289"><a name="p673722313289"></a><a name="p673722313289"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1573810234283"><a name="p1573810234283"></a><a name="p1573810234283"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p2073916232282"><a name="p2073916232282"></a><a name="p2073916232282"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p8741162342819"><a name="p8741162342819"></a><a name="p8741162342819"></a>可以是网段或者主机格式，与network_id参数二选一。source_type=0时，cidr必须是vpc子网网段的子集（不能相等）; source_type=1时，cidr必须指定专线侧网段。</p>
</td>
</tr>
<tr id="row1729182319282"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p5742162302814"><a name="p5742162302814"></a><a name="p5742162302814"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p974292313282"><a name="p974292313282"></a><a name="p974292313282"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p14743723142816"><a name="p14743723142816"></a><a name="p14743723142816"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p4744102382817"><a name="p4744102382817"></a><a name="p4744102382817"></a>功能说明：每页返回的个数。取值范围：0~2000。默认值：2000。</p>
<p id="p6745142382813"><a name="p6745142382813"></a><a name="p6745142382813"></a>最小值：<strong id="b174522315288"><a name="b174522315288"></a><a name="b174522315288"></a>1</strong></p>
<p id="p1746172322812"><a name="p1746172322812"></a><a name="p1746172322812"></a>最大值：<strong id="b874632318283"><a name="b874632318283"></a><a name="b874632318283"></a>2000</strong></p>
<p id="p1374622311284"><a name="p1374622311284"></a><a name="p1374622311284"></a>缺省值：<strong id="b174632318285"><a name="b174632318285"></a><a name="b174632318285"></a>2000</strong></p>
</td>
</tr>
<tr id="row187298236288"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p174752311287"><a name="p174752311287"></a><a name="p174752311287"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p474818232287"><a name="p474818232287"></a><a name="p474818232287"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p274892332820"><a name="p274892332820"></a><a name="p274892332820"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p7749172362819"><a name="p7749172362819"></a><a name="p7749172362819"></a>功能说明：弹性公网IP，多个弹性公网IP使用逗号分隔。取值范围：最大长度1024字节。</p>
</td>
</tr>
<tr id="row1729202310282"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1975012315282"><a name="p1975012315282"></a><a name="p1975012315282"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p12751152319281"><a name="p12751152319281"></a><a name="p12751152319281"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p5752223202816"><a name="p5752223202816"></a><a name="p5752223202816"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p197531523132812"><a name="p197531523132812"></a><a name="p197531523132812"></a>功能说明：弹性公网IP的id，多个弹性公网IP的id使用逗号分隔。取值范围：最大长度4096字节。</p>
</td>
</tr>
<tr id="row1072920237280"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p18754323162818"><a name="p18754323162818"></a><a name="p18754323162818"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p5755102318288"><a name="p5755102318288"></a><a name="p5755102318288"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p11756152382815"><a name="p11756152382815"></a><a name="p11756152382815"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p575692362820"><a name="p575692362820"></a><a name="p575692362820"></a>SNAT规则的ID。</p>
<p id="p12757023152815"><a name="p12757023152815"></a><a name="p12757023152815"></a>最小长度：<strong id="b4757162310284"><a name="b4757162310284"></a><a name="b4757162310284"></a>1</strong></p>
<p id="p675892312286"><a name="p675892312286"></a><a name="p675892312286"></a>最大长度：<strong id="b87588238288"><a name="b87588238288"></a><a name="b87588238288"></a>36</strong></p>
</td>
</tr>
<tr id="row20729162318289"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1975911230288"><a name="p1975911230288"></a><a name="p1975911230288"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p47594230289"><a name="p47594230289"></a><a name="p47594230289"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p776022312812"><a name="p776022312812"></a><a name="p776022312812"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p2761122362814"><a name="p2761122362814"></a><a name="p2761122362814"></a>SNAT规则的描述，长度限制为255。</p>
<p id="p1761162352815"><a name="p1761162352815"></a><a name="p1761162352815"></a>最大长度：<strong id="b3762423152819"><a name="b3762423152819"></a><a name="b3762423152819"></a>255</strong></p>
</td>
</tr>
<tr id="row167293238287"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p4763192332819"><a name="p4763192332819"></a><a name="p4763192332819"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p876414237289"><a name="p876414237289"></a><a name="p876414237289"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p8765182319286"><a name="p8765182319286"></a><a name="p8765182319286"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p117661823122813"><a name="p117661823122813"></a><a name="p117661823122813"></a>SNAT规则的创建时间，遵循UTC时间，格式是yyyy-mm-ddThh:mm:ssZ。</p>
<p id="p976622392817"><a name="p976622392817"></a><a name="p976622392817"></a>最小长度：<strong id="b1876692313287"><a name="b1876692313287"></a><a name="b1876692313287"></a>1</strong></p>
<p id="p2076710235280"><a name="p2076710235280"></a><a name="p2076710235280"></a>最大长度：<strong id="b7767202318286"><a name="b7767202318286"></a><a name="b7767202318286"></a>36</strong></p>
</td>
</tr>
<tr id="row9730223172819"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1476882317281"><a name="p1476882317281"></a><a name="p1476882317281"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p3768162314287"><a name="p3768162314287"></a><a name="p3768162314287"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p576902312811"><a name="p576902312811"></a><a name="p576902312811"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1277022322819"><a name="p1277022322819"></a><a name="p1277022322819"></a>公网NAT网关实例的ID。</p>
</td>
</tr>
<tr id="row17730423122819"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p8771132312816"><a name="p8771132312816"></a><a name="p8771132312816"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p377122311280"><a name="p377122311280"></a><a name="p377122311280"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1477212302811"><a name="p1477212302811"></a><a name="p1477212302811"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1773162382817"><a name="p1773162382817"></a><a name="p1773162382817"></a>规则使用的网络id。与cidr参数二选一。</p>
</td>
</tr>
<tr id="row1873092372819"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p107741823122815"><a name="p107741823122815"></a><a name="p107741823122815"></a>source_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p13775152362814"><a name="p13775152362814"></a><a name="p13775152362814"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p12775123162820"><a name="p12775123162820"></a><a name="p12775123162820"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p3371111483013"><a name="p3371111483013"></a><a name="p3371111483013"></a>0：VPC侧，可以指定network_id 或者cidr</p>
<p id="p07885171307"><a name="p07885171307"></a><a name="p07885171307"></a>1：专线侧，只能指定cidr</p>
<p id="p13776923142814"><a name="p13776923142814"></a><a name="p13776923142814"></a>缺省值：<strong id="b1477732342813"><a name="b1477732342813"></a><a name="b1477732342813"></a>0</strong></p>
</td>
</tr>
<tr id="row14730323172815"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p47789237284"><a name="p47789237284"></a><a name="p47789237284"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p7778112322812"><a name="p7778112322812"></a><a name="p7778112322812"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p9779623192817"><a name="p9779623192817"></a><a name="p9779623192817"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p7780102316282"><a name="p7780102316282"></a><a name="p7780102316282"></a>功能说明：SNAT规则的状态。</p>
<p id="p1478032322813"><a name="p1478032322813"></a><a name="p1478032322813"></a>枚举值：</p>
<a name="ul07811236285"></a><a name="ul07811236285"></a><ul id="ul07811236285"><li><strong id="b197811723132819"><a name="b197811723132819"></a><a name="b197811723132819"></a>ACTIVE</strong></li><li><strong id="b478232311283"><a name="b478232311283"></a><a name="b478232311283"></a>PENDING_CREATE</strong></li><li><strong id="b167831423152817"><a name="b167831423152817"></a><a name="b167831423152817"></a>PENDING_UPDATE</strong></li><li><strong id="b178413235289"><a name="b178413235289"></a><a name="b178413235289"></a>PENDING_DELETE</strong></li><li><strong id="b1078422352810"><a name="b1078422352810"></a><a name="b1078422352810"></a>EIP_FREEZED</strong></li><li><strong id="b147851723152814"><a name="b147851723152814"></a><a name="b147851723152814"></a>INACTIVE</strong></li></ul>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section16786123142814"></a>

**表 3**  请求Header参数

<a name="zh-cn_topic_0297140338_HeaderParameter"></a>
<table><thead align="left"><tr id="row167881823112810"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p6790102372812"><a name="p6790102372812"></a><a name="p6790102372812"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p9791172372811"><a name="p9791172372811"></a><a name="p9791172372811"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1479212342814"><a name="p1479212342814"></a><a name="p1479212342814"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p207931423162814"><a name="p207931423162814"></a><a name="p207931423162814"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row578852322817"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p3793162319281"><a name="p3793162319281"></a><a name="p3793162319281"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p13794152372818"><a name="p13794152372818"></a><a name="p13794152372818"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p14795152313283"><a name="p14795152313283"></a><a name="p14795152313283"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p579632392813"><a name="p579632392813"></a><a name="p579632392813"></a>用户Token。用户Token也就是调用获取用户Token获取请求认证接口的响应值，该接口是唯一不需要认证的接口。请求响应成功后在响应消息头中包含的“X-Subject-Token”的值即为Token值。</p>
<p id="p87971923182810"><a name="p87971923182810"></a><a name="p87971923182810"></a>最小长度：<strong id="b12798192320285"><a name="b12798192320285"></a><a name="b12798192320285"></a>1</strong></p>
<p id="p14798112312286"><a name="p14798112312286"></a><a name="p14798112312286"></a>最大长度：<strong id="b37981123122816"><a name="b37981123122816"></a><a name="b37981123122816"></a>10240</strong></p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section17799122342814"></a>

**状态码： 200**

**表 4**  响应Body参数

<a name="zh-cn_topic_0297140338_responseParameter"></a>
<table><thead align="left"><tr id="row2080072372815"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p380218231287"><a name="p380218231287"></a><a name="p380218231287"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p68031623192818"><a name="p68031623192818"></a><a name="p68031623192818"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p10804202392813"><a name="p10804202392813"></a><a name="p10804202392813"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1680122311287"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p118048236286"><a name="p118048236286"></a><a name="p118048236286"></a>snat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p168051123112812"><a name="p168051123112812"></a><a name="p168051123112812"></a>Array of <a href="#zh-cn_topic_0297140338_response_NatGatewaySnatRuleResponseBody">NatGatewaySnatRuleResponseBody</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p980622322817"><a name="p980622322817"></a><a name="p980622322817"></a>查询SNAT规则列表的响应体。</p>
</td>
</tr>
</tbody>
</table>

**表 5**  NatGatewaySnatRuleResponseBody

<a name="zh-cn_topic_0297140338_response_NatGatewaySnatRuleResponseBody"></a>
<table><thead align="left"><tr id="row19808823162819"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p381142310286"><a name="p381142310286"></a><a name="p381142310286"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p18121223202818"><a name="p18121223202818"></a><a name="p18121223202818"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p98139230285"><a name="p98139230285"></a><a name="p98139230285"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row980812237285"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p881372314288"><a name="p881372314288"></a><a name="p881372314288"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p15814142322819"><a name="p15814142322819"></a><a name="p15814142322819"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1381552312815"><a name="p1381552312815"></a><a name="p1381552312815"></a>SNAT规则的ID。</p>
<p id="p17816623192819"><a name="p17816623192819"></a><a name="p17816623192819"></a>长度：<strong id="b481652317286"><a name="b481652317286"></a><a name="b481652317286"></a>36</strong></p>
</td>
</tr>
<tr id="row780814236286"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1818723102819"><a name="p1818723102819"></a><a name="p1818723102819"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p0819123142816"><a name="p0819123142816"></a><a name="p0819123142816"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p13820323172810"><a name="p13820323172810"></a><a name="p13820323172810"></a>项目的ID。</p>
</td>
</tr>
<tr id="row7808122382815"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p582132382811"><a name="p582132382811"></a><a name="p582132382811"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p6822182302820"><a name="p6822182302820"></a><a name="p6822182302820"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p8823423102816"><a name="p8823423102816"></a><a name="p8823423102816"></a>公网NAT网关实例的ID。</p>
<p id="p118234236283"><a name="p118234236283"></a><a name="p118234236283"></a>长度：<strong id="b1782362302819"><a name="b1782362302819"></a><a name="b1782362302819"></a>36</strong></p>
</td>
</tr>
<tr id="row18808123192810"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p38241423162812"><a name="p38241423162812"></a><a name="p38241423162812"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p682532352814"><a name="p682532352814"></a><a name="p682532352814"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p736446341"><a name="p736446341"></a><a name="p736446341"></a>cidr，可以是网段或者主机格式，与network_id参数二选一。source_type=0时，cidr必须是vpc子网网段的子集（不能相等）;</p>
<p id="p158251237281"><a name="p158251237281"></a><a name="p158251237281"></a>source_type=1时，cidr必须指定专线侧网段。</p>
<p id="p14826152315287"><a name="p14826152315287"></a><a name="p14826152315287"></a>最小长度：<strong id="b13826152312814"><a name="b13826152312814"></a><a name="b13826152312814"></a>9</strong></p>
<p id="p1782692310285"><a name="p1782692310285"></a><a name="p1782692310285"></a>最大长度：<strong id="b18827112315280"><a name="b18827112315280"></a><a name="b18827112315280"></a>39</strong></p>
</td>
</tr>
<tr id="row1780892316284"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11827123172813"><a name="p11827123172813"></a><a name="p11827123172813"></a>source_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p6828192315286"><a name="p6828192315286"></a><a name="p6828192315286"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p7600104543216"><a name="p7600104543216"></a><a name="p7600104543216"></a>0：VPC侧，可以指定network_id 或者cidr</p>
<p id="p482972382811"><a name="p482972382811"></a><a name="p482972382811"></a>1：专线侧，只能指定cidr</p>
<p id="p19441171125915"><a name="p19441171125915"></a><a name="p19441171125915"></a>缺省值：<strong id="b1883002302818"><a name="b1883002302818"></a><a name="b1883002302818"></a>0</strong></p>
</td>
</tr>
<tr id="row9808823152817"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p98301323102816"><a name="p98301323102816"></a><a name="p98301323102816"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1831202392813"><a name="p1831202392813"></a><a name="p1831202392813"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p88311323102814"><a name="p88311323102814"></a><a name="p88311323102814"></a>功能说明：弹性公网IP的id，多个弹性公网IP的id使用逗号分隔。取值范围：最大长度4096字节。</p>
</td>
</tr>
<tr id="row880832372813"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15832162316289"><a name="p15832162316289"></a><a name="p15832162316289"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p683302310283"><a name="p683302310283"></a><a name="p683302310283"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p383412232281"><a name="p383412232281"></a><a name="p383412232281"></a>SNAT规则的描述，长度限制为255。</p>
<p id="p19835823162815"><a name="p19835823162815"></a><a name="p19835823162815"></a>最大长度：<strong id="b1383512235281"><a name="b1383512235281"></a><a name="b1383512235281"></a>255</strong></p>
</td>
</tr>
<tr id="row118081123142819"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p16835142312810"><a name="p16835142312810"></a><a name="p16835142312810"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p3836923122818"><a name="p3836923122818"></a><a name="p3836923122818"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5837152302812"><a name="p5837152302812"></a><a name="p5837152302812"></a>功能说明：SNAT规则的状态。</p>
<p id="p2838162342816"><a name="p2838162342816"></a><a name="p2838162342816"></a>枚举值：</p>
<a name="ul1839152319285"></a><a name="ul1839152319285"></a><ul id="ul1839152319285"><li><strong id="b198401123142813"><a name="b198401123142813"></a><a name="b198401123142813"></a>ACTIVE</strong></li><li><strong id="b15841423192818"><a name="b15841423192818"></a><a name="b15841423192818"></a>PENDING_CREATE</strong></li><li><strong id="b1841162322811"><a name="b1841162322811"></a><a name="b1841162322811"></a>PENDING_UPDATE</strong></li><li><strong id="b9842192372819"><a name="b9842192372819"></a><a name="b9842192372819"></a>PENDING_DELETE</strong></li><li><strong id="b8843323122814"><a name="b8843323122814"></a><a name="b8843323122814"></a>EIP_FREEZED</strong></li><li><strong id="b11844122313280"><a name="b11844122313280"></a><a name="b11844122313280"></a>INACTIVE</strong></li></ul>
</td>
</tr>
<tr id="row118085236280"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1684522311280"><a name="p1684522311280"></a><a name="p1684522311280"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p188461723162810"><a name="p188461723162810"></a><a name="p188461723162810"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11846142382810"><a name="p11846142382810"></a><a name="p11846142382810"></a>SNAT规则的创建时间，遵循UTC时间，格式是yyyy-mm-ddThh:mm:ssZ。</p>
<p id="p684792372817"><a name="p684792372817"></a><a name="p684792372817"></a>最小长度：<strong id="b68472235283"><a name="b68472235283"></a><a name="b68472235283"></a>1</strong></p>
<p id="p4847192317286"><a name="p4847192317286"></a><a name="p4847192317286"></a>最大长度：<strong id="b20848192392813"><a name="b20848192392813"></a><a name="b20848192392813"></a>36</strong></p>
</td>
</tr>
<tr id="row6808182315286"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1848523192816"><a name="p1848523192816"></a><a name="p1848523192816"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p88491923132813"><a name="p88491923132813"></a><a name="p88491923132813"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p13850152362819"><a name="p13850152362819"></a><a name="p13850152362819"></a>规则使用的网络id。与cidr参数二选一。</p>
<p id="p118501923142814"><a name="p118501923142814"></a><a name="p118501923142814"></a>长度：<strong id="b18851152362819"><a name="b18851152362819"></a><a name="b18851152362819"></a>36</strong></p>
</td>
</tr>
<tr id="row880972332816"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p12852192302819"><a name="p12852192302819"></a><a name="p12852192302819"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p685202312814"><a name="p685202312814"></a><a name="p685202312814"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p20853102342813"><a name="p20853102342813"></a><a name="p20853102342813"></a>解冻/冻结状态。取值范围：</p>
<a name="ul485311234288"></a><a name="ul485311234288"></a><ul id="ul485311234288"><li>"true"：解冻</li><li>"false"：冻结</li></ul>
</td>
</tr>
<tr id="row88091723122812"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p5855182317287"><a name="p5855182317287"></a><a name="p5855182317287"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1785615239289"><a name="p1785615239289"></a><a name="p1785615239289"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1085662312819"><a name="p1085662312819"></a><a name="p1085662312819"></a>功能说明：弹性公网IP，多个弹性公网IP使用逗号分隔。取值范围：最大长度1024字节。</p>
</td>
</tr>
<tr id="row2809142322818"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p178571423192819"><a name="p178571423192819"></a><a name="p178571423192819"></a>freezed_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p3858623122813"><a name="p3858623122813"></a><a name="p3858623122813"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p9858172311286"><a name="p9858172311286"></a><a name="p9858172311286"></a>功能说明：冻结的弹性公网IP，多个冻结的弹性公网IP使用逗号分隔。取值范围：最大长度1024字节。</p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section185992302810"></a>

```
GET https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/snat_rules?limit=2

   
```

## 响应示例<a name="section2867172318289"></a>

**状态码： 200**

查询SNAT规则列表成功。

```
{
  "snat_rules" : [ {
    "floating_ip_id" : "bf99c679-9f41-4dac-8513-9c9228e713e1",
    "status" : "ACTIVE",
    "nat_gateway_id" : "cda3a125-2406-456c-a11f-598e10578541",
    "admin_state_up" : true,
    "network_id" : "9a469561-daac-4c94-88f5-39366e5ea193",
    "source_type" : 0,
    "tenant_id" : "d199ba7e0ba64899b2e81518104b1526",
    "created_at" : "2017-11-15 15:44:42.595173",
    "id" : "79195d50-0271-41f1-bded-4c089b2502ff",
    "floating_ip_address" : "5.21.11.242",
    "freezed_ip_address" : "",
    "description" : "my snat rule 01"
  }, {
    "floating_ip_id" : "6e496fba-abe9-4f5e-9406-2ad8c809ac8c",
    "status" : "ACTIVE",
    "nat_gateway_id" : "e824f1b4-4290-4ebc-8322-cfff370dbd1e",
    "admin_state_up" : true,
    "network_id" : "97e89905-f9c8-4ae3-9856-392b0b2fbe7f",
    "source_type" : 0,
    "tenant_id" : "d199ba7e0ba64899b2e81518104b1526",
    "created_at" : "2017-11-17 07:43:44.830845",
    "id" : "4a1a10d7-0d9f-4846-8cda-24cffeffef5c",
    "floating_ip_address" : "5.21.11.142,5.21.11.143",
    "freezed_ip_address" : "5.21.11.142",
    "description" : "my snat rule 01"
  } ]
}
```

## 状态码<a name="section41882420282"></a>

<a name="zh-cn_topic_0297140338_status_code"></a>
<table><thead align="left"><tr id="row388312372814"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p1418524192812"><a name="p1418524192812"></a><a name="p1418524192812"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p319192442817"><a name="p319192442817"></a><a name="p319192442817"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row11883223142811"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p31932482812"><a name="p31932482812"></a><a name="p31932482812"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p819824142815"><a name="p819824142815"></a><a name="p819824142815"></a>查询SNAT规则列表成功。</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section12202247287"></a>

请参见[错误码](错误码.md)。

