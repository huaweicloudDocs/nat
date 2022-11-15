# 查询指定的DNAT规则详情<a name="ShowNatGatewayDnatRule"></a>

## 功能介绍<a name="section049185432612"></a>

查询指定的DNAT规则详情。

## 调试<a name="section1656254182619"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=nat&api=ShowNatGatewayDnatRule)中调试该接口。

## URI<a name="section965354152612"></a>

GET /v2/\{project\_id\}/dnat\_rules/\{dnat\_rule\_id\}

**表 1**  路径参数

<a name="table9731254152612"></a>
<table><thead align="left"><tr id="row271254102620"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p876454152620"><a name="p876454152620"></a><a name="p876454152620"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p177911543261"><a name="p177911543261"></a><a name="p177911543261"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p128417545261"><a name="p128417545261"></a><a name="p128417545261"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p13881054172618"><a name="p13881054172618"></a><a name="p13881054172618"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row972145472618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p129165411264"><a name="p129165411264"></a><a name="p129165411264"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1595115413267"><a name="p1595115413267"></a><a name="p1595115413267"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p399135422610"><a name="p399135422610"></a><a name="p399135422610"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p3103135419262"><a name="p3103135419262"></a><a name="p3103135419262"></a>项目的ID。</p>
<p id="p101062054132614"><a name="p101062054132614"></a><a name="p101062054132614"></a>最小长度：<strong id="b010745416261"><a name="b010745416261"></a><a name="b010745416261"></a>1</strong></p>
<p id="p310955412618"><a name="p310955412618"></a><a name="p310955412618"></a>最大长度：<strong id="b3110115422616"><a name="b3110115422616"></a><a name="b3110115422616"></a>36</strong></p>
<p id="p2562026131319"><a name="p2562026131319"></a><a name="p2562026131319"></a>获取方法详见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row8728548265"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p13112554152617"><a name="p13112554152617"></a><a name="p13112554152617"></a>dnat_rule_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p41167548267"><a name="p41167548267"></a><a name="p41167548267"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p911945412266"><a name="p911945412266"></a><a name="p911945412266"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1312305472620"><a name="p1312305472620"></a><a name="p1312305472620"></a>DNAT规则的ID。</p>
<p id="p181261854182618"><a name="p181261854182618"></a><a name="p181261854182618"></a>长度：<strong id="b9128165419263"><a name="b9128165419263"></a><a name="b9128165419263"></a>36</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section19133125432614"></a>

**表 2**  请求Header参数

<a name="zh-cn_topic_0297140335_HeaderParameter"></a>
<table><thead align="left"><tr id="row1138554102617"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p614315547262"><a name="p614315547262"></a><a name="p614315547262"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p151469542261"><a name="p151469542261"></a><a name="p151469542261"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p161498548264"><a name="p161498548264"></a><a name="p161498548264"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p16152175402615"><a name="p16152175402615"></a><a name="p16152175402615"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row171383548264"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1115616540265"><a name="p1115616540265"></a><a name="p1115616540265"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p416125412618"><a name="p416125412618"></a><a name="p416125412618"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p61647547268"><a name="p61647547268"></a><a name="p61647547268"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p416895411264"><a name="p416895411264"></a><a name="p416895411264"></a>用户Token。用户Token也就是调用获取用户Token获取请求认证接口的响应值，该接口是唯一不需要认证的接口。请求响应成功后在响应消息头中包含的“X-Subject-Token”的值即为Token值。</p>
<p id="p16171185411265"><a name="p16171185411265"></a><a name="p16171185411265"></a>最小长度：<strong id="b1917365472613"><a name="b1917365472613"></a><a name="b1917365472613"></a>1</strong></p>
<p id="p18175254112619"><a name="p18175254112619"></a><a name="p18175254112619"></a>最大长度：<strong id="b161781554112613"><a name="b161781554112613"></a><a name="b161781554112613"></a>10240</strong></p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section17182454112615"></a>

**状态码： 200**

**表 3**  响应Body参数

<a name="zh-cn_topic_0297140335_responseParameter"></a>
<table><thead align="left"><tr id="row13189135417261"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p141931054112612"><a name="p141931054112612"></a><a name="p141931054112612"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p219635417268"><a name="p219635417268"></a><a name="p219635417268"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p01991554122615"><a name="p01991554122615"></a><a name="p01991554122615"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row71891554112617"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1520245422615"><a name="p1520245422615"></a><a name="p1520245422615"></a>dnat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1320820543264"><a name="p1320820543264"></a><a name="p1320820543264"></a><a href="#zh-cn_topic_0297140335_response_NatGatewayDnatRuleResponseBody">NatGatewayDnatRuleResponseBody</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p192111054152616"><a name="p192111054152616"></a><a name="p192111054152616"></a>DNAT规则的响应体。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  NatGatewayDnatRuleResponseBody

<a name="zh-cn_topic_0297140335_response_NatGatewayDnatRuleResponseBody"></a>
<table><thead align="left"><tr id="row15215254122614"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p162242549269"><a name="p162242549269"></a><a name="p162242549269"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p422805412614"><a name="p422805412614"></a><a name="p422805412614"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p132321354162616"><a name="p132321354162616"></a><a name="p132321354162616"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1321675411264"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p152364548261"><a name="p152364548261"></a><a name="p152364548261"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p152401854152618"><a name="p152401854152618"></a><a name="p152401854152618"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2244145472611"><a name="p2244145472611"></a><a name="p2244145472611"></a>DNAT规则的ID。</p>
<p id="p102471254162612"><a name="p102471254162612"></a><a name="p102471254162612"></a>长度：<strong id="b1624815414261"><a name="b1624815414261"></a><a name="b1624815414261"></a>36</strong></p>
</td>
</tr>
<tr id="row6216454202615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p825519548268"><a name="p825519548268"></a><a name="p825519548268"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p9262115482620"><a name="p9262115482620"></a><a name="p9262115482620"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p526605492613"><a name="p526605492613"></a><a name="p526605492613"></a>项目的ID。</p>
</td>
</tr>
<tr id="row22164547263"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1527255418265"><a name="p1527255418265"></a><a name="p1527255418265"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p927515452617"><a name="p927515452617"></a><a name="p927515452617"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p9279105492617"><a name="p9279105492617"></a><a name="p9279105492617"></a>DNAT规则的描述。长度限制为255。</p>
<p id="p4282105412265"><a name="p4282105412265"></a><a name="p4282105412265"></a>最大长度：<strong id="b1028315452617"><a name="b1028315452617"></a><a name="b1028315452617"></a>255</strong></p>
</td>
</tr>
<tr id="row22161954122615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p228675452614"><a name="p228675452614"></a><a name="p228675452614"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19289115410263"><a name="p19289115410263"></a><a name="p19289115410263"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1529435416267"><a name="p1529435416267"></a><a name="p1529435416267"></a>虚拟机或者裸机的Port ID，与private_ip参数二选一。</p>
<p id="p142986544265"><a name="p142986544265"></a><a name="p142986544265"></a>长度：<strong id="b13299205482612"><a name="b13299205482612"></a><a name="b13299205482612"></a>36</strong></p>
</td>
</tr>
<tr id="row15216105472611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p53060549265"><a name="p53060549265"></a><a name="p53060549265"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12311185492617"><a name="p12311185492617"></a><a name="p12311185492617"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p13314175432612"><a name="p13314175432612"></a><a name="p13314175432612"></a>用户私有IP地址，例如专线连接的私有云地址，与port_id参数二选一。</p>
</td>
</tr>
<tr id="row1216854202612"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1431845418268"><a name="p1431845418268"></a><a name="p1431845418268"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1632115410262"><a name="p1632115410262"></a><a name="p1632115410262"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p63261254182614"><a name="p63261254182614"></a><a name="p63261254182614"></a>虚拟机或者裸机对外提供服务的协议端口号。取值范围：0~65535。</p>
<p id="p1232913547268"><a name="p1232913547268"></a><a name="p1232913547268"></a>最小值：<strong id="b1533015442615"><a name="b1533015442615"></a><a name="b1533015442615"></a>0</strong></p>
<p id="p233315492612"><a name="p233315492612"></a><a name="p233315492612"></a>最大值：<strong id="b1733565411260"><a name="b1733565411260"></a><a name="b1733565411260"></a>65535</strong></p>
<p id="p113371154122617"><a name="p113371154122617"></a><a name="p113371154122617"></a>最小长度：<strong id="b1933916549264"><a name="b1933916549264"></a><a name="b1933916549264"></a>1</strong></p>
<p id="p1534195419266"><a name="p1534195419266"></a><a name="p1534195419266"></a>最大长度：<strong id="b63421454132619"><a name="b63421454132619"></a><a name="b63421454132619"></a>5</strong></p>
</td>
</tr>
<tr id="row1121615422615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11345175482615"><a name="p11345175482615"></a><a name="p11345175482615"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p18348254202612"><a name="p18348254202612"></a><a name="p18348254202612"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1535316549260"><a name="p1535316549260"></a><a name="p1535316549260"></a>公网NAT网关实例的ID。</p>
<p id="p2355165415263"><a name="p2355165415263"></a><a name="p2355165415263"></a>最小长度：<strong id="b7357145413260"><a name="b7357145413260"></a><a name="b7357145413260"></a>1</strong></p>
<p id="p6359125422618"><a name="p6359125422618"></a><a name="p6359125422618"></a>最大长度：<strong id="b143601154142619"><a name="b143601154142619"></a><a name="b143601154142619"></a>36</strong></p>
</td>
</tr>
<tr id="row20216145412614"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p5364115420267"><a name="p5364115420267"></a><a name="p5364115420267"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p173688546260"><a name="p173688546260"></a><a name="p173688546260"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p193734543263"><a name="p193734543263"></a><a name="p193734543263"></a>弹性公网IP的id。</p>
<p id="p133755549260"><a name="p133755549260"></a><a name="p133755549260"></a>最小长度：<strong id="b163771154152612"><a name="b163771154152612"></a><a name="b163771154152612"></a>1</strong></p>
<p id="p1338016545268"><a name="p1338016545268"></a><a name="p1338016545268"></a>最大长度：<strong id="b4381185482616"><a name="b4381185482616"></a><a name="b4381185482616"></a>36</strong></p>
</td>
</tr>
<tr id="row14216105482620"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p10384195482611"><a name="p10384195482611"></a><a name="p10384195482611"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p103871543262"><a name="p103871543262"></a><a name="p103871543262"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p339075412262"><a name="p339075412262"></a><a name="p339075412262"></a>弹性公网IP的IP地址。</p>
</td>
</tr>
<tr id="row621665411265"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p139625410268"><a name="p139625410268"></a><a name="p139625410268"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p539925402611"><a name="p539925402611"></a><a name="p539925402611"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p540210549263"><a name="p540210549263"></a><a name="p540210549263"></a>Floatingip对外提供服务的端口号。取值范围：0~65535。</p>
</td>
</tr>
<tr id="row0216185418265"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p16406354102619"><a name="p16406354102619"></a><a name="p16406354102619"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1941065415264"><a name="p1941065415264"></a><a name="p1941065415264"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1041405432615"><a name="p1041405432615"></a><a name="p1041405432615"></a>功能说明：DNAT规则的状态。</p>
<p id="p641795492612"><a name="p641795492612"></a><a name="p641795492612"></a>枚举值：</p>
<a name="ul20422754122619"></a><a name="ul20422754122619"></a><ul id="ul20422754122619"><li><strong id="b19427954132612"><a name="b19427954132612"></a><a name="b19427954132612"></a>ACTIVE</strong></li><li><strong id="b124327549262"><a name="b124327549262"></a><a name="b124327549262"></a>PENDING_CREATE</strong></li><li><strong id="b7435115413265"><a name="b7435115413265"></a><a name="b7435115413265"></a>PENDING_UPDATE</strong></li><li><strong id="b13439135419267"><a name="b13439135419267"></a><a name="b13439135419267"></a>PENDING_DELETE</strong></li><li><strong id="b1144285422618"><a name="b1144285422618"></a><a name="b1144285422618"></a>EIP_FREEZED</strong></li><li><strong id="b144710547265"><a name="b144710547265"></a><a name="b144710547265"></a>INACTIVE</strong></li></ul>
</td>
</tr>
<tr id="row1216754182610"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p114498546266"><a name="p114498546266"></a><a name="p114498546266"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p34541054102619"><a name="p34541054102619"></a><a name="p34541054102619"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1845915542268"><a name="p1845915542268"></a><a name="p1845915542268"></a>解冻/冻结状态。取值范围：</p>
<a name="ul195721758266"></a><a name="ul195721758266"></a><ul id="ul195721758266"><li>"true"： 解冻</li><li>"false"： 冻结</li></ul>
</td>
</tr>
<tr id="row2217135414267"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p146445420269"><a name="p146445420269"></a><a name="p146445420269"></a>internal_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1046805414261"><a name="p1046805414261"></a><a name="p1046805414261"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p15472654102615"><a name="p15472654102615"></a><a name="p15472654102615"></a>虚拟机或者裸机对外提供服务的协议端口号范围。功能说明：该端口范围与external _service_port_range按顺序实现1:1映射。取值范围：1~65535。约束：只能以’-’字符连接端口范围。</p>
</td>
</tr>
<tr id="row18217195417260"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p18475654172611"><a name="p18475654172611"></a><a name="p18475654172611"></a>external_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p848085414269"><a name="p848085414269"></a><a name="p848085414269"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p7484145411263"><a name="p7484145411263"></a><a name="p7484145411263"></a>Floatingip对外提供服务的端口号范围。功能说明：该端口范围与internal _service_port_range按顺序实现1:1映射。取值范围：1~65535。约束：只能以’-’字符连接端口范围</p>
</td>
</tr>
<tr id="row15217185418266"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1148825411265"><a name="p1148825411265"></a><a name="p1148825411265"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1549265416260"><a name="p1549265416260"></a><a name="p1549265416260"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1749785414262"><a name="p1749785414262"></a><a name="p1749785414262"></a>协议类型，目前支持TCP/tcp、UDP/udp、ANY/any。对应协议号6、17、0。</p>
<p id="p1350045452613"><a name="p1350045452613"></a><a name="p1350045452613"></a>最小长度：<strong id="b13501205442619"><a name="b13501205442619"></a><a name="b13501205442619"></a>1</strong></p>
<p id="p185041854162620"><a name="p185041854162620"></a><a name="p185041854162620"></a>最大长度：<strong id="b550513545262"><a name="b550513545262"></a><a name="b550513545262"></a>3</strong></p>
<p id="p13507165419260"><a name="p13507165419260"></a><a name="p13507165419260"></a>枚举值：</p>
<a name="ul13511155420269"></a><a name="ul13511155420269"></a><ul id="ul13511155420269"><li><strong id="b0514105462615"><a name="b0514105462615"></a><a name="b0514105462615"></a>tcp</strong></li><li><strong id="b15173549263"><a name="b15173549263"></a><a name="b15173549263"></a>udp</strong></li><li><strong id="b19521954182611"><a name="b19521954182611"></a><a name="b19521954182611"></a>any</strong></li></ul>
</td>
</tr>
<tr id="row22179549262"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p052316548267"><a name="p052316548267"></a><a name="p052316548267"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p252720543263"><a name="p252720543263"></a><a name="p252720543263"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1053395422620"><a name="p1053395422620"></a><a name="p1053395422620"></a>DNAT规则的创建时间，遵循UTC时间，格式是yyyy-mm-ddThh:mm:ssZ。</p>
<p id="p6536155416264"><a name="p6536155416264"></a><a name="p6536155416264"></a>最小长度：<strong id="b1353795418267"><a name="b1353795418267"></a><a name="b1353795418267"></a>1</strong></p>
<p id="p175401154142618"><a name="p175401154142618"></a><a name="p175401154142618"></a>最大长度：<strong id="b16542105412614"><a name="b16542105412614"></a><a name="b16542105412614"></a>36</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section754575413266"></a>

```
GET https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526d/dnat_rules/5b95c675-69c2-4656-ba06-58ff72e1d338

  
```

## 响应示例<a name="section256375411261"></a>

**状态码： 200**

查询DNAT规则成功。

```
{
  "dnat_rule" : {
    "floating_ip_id" : "bf99c679-9f41-4dac-8513-9c9228e713e1",
    "status" : "ACTIVE",
    "nat_gateway_id" : "cda3a125-2406-456c-a11f-598e10578541",
    "admin_state_up" : true,
    "port_id" : "9a469561-daac-4c94-88f5-39366e5ea193",
    "private_ip" : "",
    "internal_service_port" : 993,
    "protocol" : "tcp",
    "tenant_id" : "d199ba7e0ba64899b2e81518104b1526d",
    "created_at" : "2017-11-15 15:44:42.595173",
    "id" : "5b95c675-69c2-4656-ba06-58ff72e1d338",
    "floating_ip_address" : "5.21.11.226",
    "external_service_port" : 242,
    "description" : "my dnat rule 01"
  }
}
```

## 状态码<a name="section863585442610"></a>

<a name="zh-cn_topic_0297140335_status_code"></a>
<table><thead align="left"><tr id="row11639354132620"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p36421454122619"><a name="p36421454122619"></a><a name="p36421454122619"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p7645754172612"><a name="p7645754172612"></a><a name="p7645754172612"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row126394544268"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1764810549266"><a name="p1764810549266"></a><a name="p1764810549266"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p96514542265"><a name="p96514542265"></a><a name="p96514542265"></a>查询DNAT规则成功。</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section12655125415261"></a>

请参见[错误码](错误码.md)。

