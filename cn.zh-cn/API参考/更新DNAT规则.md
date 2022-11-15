# 更新DNAT规则<a name="UpdateNatGatewayDnatRule"></a>

## 功能介绍<a name="section15266732142619"></a>

更新指定的DNAT规则。

## 接口约束<a name="section6274163212618"></a>

-   更新操作时，要求DNAT规则状态status = ACTIVE，要求网关管理员状态admin\_state\_up = True。
-   port\_id和private\_ip不能同时生效。
-   对于all port类型的规则，要求internal\_service\_port = 0，external\_service\_port = 0，protocol = ANY。
-   更新操作涉及以下字段更新时，要求这些字段必须一起更新。包括：port\_id、private\_ip、internal\_service\_port、external\_service\_port、floating\_ip\_id、protocol、internal\_service\_port\_range、external\_service\_port\_range。

## 调试<a name="section627818323261"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=nat&api=UpdateNatGatewayDnatRule)中调试该接口。

## URI<a name="section02849320265"></a>

PUT /v2/\{project\_id\}/dnat\_rules/\{dnat\_rule\_id\}

**表 1**  路径参数

<a name="table4291123214267"></a>
<table><thead align="left"><tr id="row182891132142612"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p19293132202618"><a name="p19293132202618"></a><a name="p19293132202618"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p172955327260"><a name="p172955327260"></a><a name="p172955327260"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p929711329262"><a name="p929711329262"></a><a name="p929711329262"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p11301183282613"><a name="p11301183282613"></a><a name="p11301183282613"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row6289153222617"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p183041432192619"><a name="p183041432192619"></a><a name="p183041432192619"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1030713292610"><a name="p1030713292610"></a><a name="p1030713292610"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p4310532112616"><a name="p4310532112616"></a><a name="p4310532112616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p17313732132618"><a name="p17313732132618"></a><a name="p17313732132618"></a>项目的ID。</p>
<p id="p1331623219268"><a name="p1331623219268"></a><a name="p1331623219268"></a>最小长度：<strong id="b931713320265"><a name="b931713320265"></a><a name="b931713320265"></a>1</strong></p>
<p id="p73181532172610"><a name="p73181532172610"></a><a name="p73181532172610"></a>最大长度：<strong id="b1931953218268"><a name="b1931953218268"></a><a name="b1931953218268"></a>36</strong></p>
<p id="p2562026131319"><a name="p2562026131319"></a><a name="p2562026131319"></a>获取方法详见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row14289163282619"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p63219325266"><a name="p63219325266"></a><a name="p63219325266"></a>dnat_rule_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p6324173252610"><a name="p6324173252610"></a><a name="p6324173252610"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p53261332172617"><a name="p53261332172617"></a><a name="p53261332172617"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p12329123216261"><a name="p12329123216261"></a><a name="p12329123216261"></a>DNAT规则的ID。</p>
<p id="p11332932152618"><a name="p11332932152618"></a><a name="p11332932152618"></a>长度：<strong id="b7333203262619"><a name="b7333203262619"></a><a name="b7333203262619"></a>36</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section1333863222615"></a>

**表 2**  请求Header参数

<a name="zh-cn_topic_0297140301_HeaderParameter"></a>
<table><thead align="left"><tr id="row13341732132617"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p4345123232610"><a name="p4345123232610"></a><a name="p4345123232610"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p234811329265"><a name="p234811329265"></a><a name="p234811329265"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p5351203232619"><a name="p5351203232619"></a><a name="p5351203232619"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p1135313324262"><a name="p1135313324262"></a><a name="p1135313324262"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row3341232112614"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p11356123212615"><a name="p11356123212615"></a><a name="p11356123212615"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p14358193210269"><a name="p14358193210269"></a><a name="p14358193210269"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p163601232182613"><a name="p163601232182613"></a><a name="p163601232182613"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p3363193219268"><a name="p3363193219268"></a><a name="p3363193219268"></a>用户Token。用户Token也就是调用获取用户Token获取请求认证接口的响应值，该接口是唯一不需要认证的接口。请求响应成功后在响应消息头中包含的“X-Subject-Token”的值即为Token值。</p>
<p id="p13366143212616"><a name="p13366143212616"></a><a name="p13366143212616"></a>最小长度：<strong id="b336793217265"><a name="b336793217265"></a><a name="b336793217265"></a>1</strong></p>
<p id="p1736815325268"><a name="p1736815325268"></a><a name="p1736815325268"></a>最大长度：<strong id="b133691932172615"><a name="b133691932172615"></a><a name="b133691932172615"></a>10240</strong></p>
</td>
</tr>
</tbody>
</table>

**表 3**  请求Body参数

<a name="zh-cn_topic_0297140301_requestParameter"></a>
<table><thead align="left"><tr id="row33718328268"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1937493211264"><a name="p1937493211264"></a><a name="p1937493211264"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p203771232122617"><a name="p203771232122617"></a><a name="p203771232122617"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p9380173219262"><a name="p9380173219262"></a><a name="p9380173219262"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p838214323265"><a name="p838214323265"></a><a name="p838214323265"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1137153210265"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p143841732142617"><a name="p143841732142617"></a><a name="p143841732142617"></a>dnat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p538613212613"><a name="p538613212613"></a><a name="p538613212613"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1138903262612"><a name="p1138903262612"></a><a name="p1138903262612"></a><a href="#zh-cn_topic_0297140301_request_UpdateNatGatewayDnatRuleOption">UpdateNatGatewayDnatRuleOption</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p183921732112611"><a name="p183921732112611"></a><a name="p183921732112611"></a>更新DNAT规则的请求体。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  UpdateNatGatewayDnatRuleOption

<a name="zh-cn_topic_0297140301_request_UpdateNatGatewayDnatRuleOption"></a>
<table><thead align="left"><tr id="row1139616329266"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p10400173219262"><a name="p10400173219262"></a><a name="p10400173219262"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p940343272613"><a name="p940343272613"></a><a name="p940343272613"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p540518321269"><a name="p540518321269"></a><a name="p540518321269"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p20407232182618"><a name="p20407232182618"></a><a name="p20407232182618"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row8396123211269"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p19409173216262"><a name="p19409173216262"></a><a name="p19409173216262"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1041143219263"><a name="p1041143219263"></a><a name="p1041143219263"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p9413133242615"><a name="p9413133242615"></a><a name="p9413133242615"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p13415332152616"><a name="p13415332152616"></a><a name="p13415332152616"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="row239603242614"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p541733282610"><a name="p541733282610"></a><a name="p541733282610"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p142023212614"><a name="p142023212614"></a><a name="p142023212614"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p4422133242612"><a name="p4422133242612"></a><a name="p4422133242612"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1942643262618"><a name="p1942643262618"></a><a name="p1942643262618"></a>DNAT规则的描述，长度限制为255。</p>
<p id="p34285324267"><a name="p34285324267"></a><a name="p34285324267"></a>最大长度：<strong id="b64291325269"><a name="b64291325269"></a><a name="b64291325269"></a>255</strong></p>
</td>
</tr>
<tr id="row639618321263"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p104317327267"><a name="p104317327267"></a><a name="p104317327267"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p54331532202619"><a name="p54331532202619"></a><a name="p54331532202619"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p6435183211268"><a name="p6435183211268"></a><a name="p6435183211268"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p14438132132619"><a name="p14438132132619"></a><a name="p14438132132619"></a>虚拟机或者裸机的Port ID，与private_ip参数二选一。</p>
</td>
</tr>
<tr id="row139611329263"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1944063217265"><a name="p1944063217265"></a><a name="p1944063217265"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p12443632172611"><a name="p12443632172611"></a><a name="p12443632172611"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p14445113213265"><a name="p14445113213265"></a><a name="p14445113213265"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1044883212610"><a name="p1044883212610"></a><a name="p1044883212610"></a>用户私有IP地址，例如专线连接的私有云地址，与port_id参数二选一。</p>
</td>
</tr>
<tr id="row239713217266"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1445083292612"><a name="p1445083292612"></a><a name="p1445083292612"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p7452932202614"><a name="p7452932202614"></a><a name="p7452932202614"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p44551432182610"><a name="p44551432182610"></a><a name="p44551432182610"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p94581832192612"><a name="p94581832192612"></a><a name="p94581832192612"></a>协议类型，目前支持TCP/tcp、UDP/udp、ANY/any。对应协议号6、17、0。</p>
<p id="p1446016328262"><a name="p1446016328262"></a><a name="p1446016328262"></a>最小长度：<strong id="b1346143220261"><a name="b1346143220261"></a><a name="b1346143220261"></a>1</strong></p>
<p id="p11462832152611"><a name="p11462832152611"></a><a name="p11462832152611"></a>最大长度：<strong id="b4463332172614"><a name="b4463332172614"></a><a name="b4463332172614"></a>3</strong></p>
<p id="p1646573212267"><a name="p1646573212267"></a><a name="p1646573212267"></a>枚举值：</p>
<a name="ul10467133252619"></a><a name="ul10467133252619"></a><ul id="ul10467133252619"><li><strong id="b194691732132610"><a name="b194691732132610"></a><a name="b194691732132610"></a>TCP</strong></li><li><strong id="b11472143292619"><a name="b11472143292619"></a><a name="b11472143292619"></a>UDP</strong></li><li><strong id="b1447423222614"><a name="b1447423222614"></a><a name="b1447423222614"></a>ANY</strong></li></ul>
</td>
</tr>
<tr id="row2397183216261"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p647553252617"><a name="p647553252617"></a><a name="p647553252617"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p4478153252616"><a name="p4478153252616"></a><a name="p4478153252616"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1548016324263"><a name="p1548016324263"></a><a name="p1548016324263"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p144831532192615"><a name="p144831532192615"></a><a name="p144831532192615"></a>弹性公网IP的id。</p>
</td>
</tr>
<tr id="row1397432192619"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p7485932172615"><a name="p7485932172615"></a><a name="p7485932172615"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p14487132112612"><a name="p14487132112612"></a><a name="p14487132112612"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1749017321265"><a name="p1749017321265"></a><a name="p1749017321265"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p2493203252617"><a name="p2493203252617"></a><a name="p2493203252617"></a>虚拟机或者裸机对外提供服务的协议端口号。取值范围：0~65535。</p>
<p id="p3495163252613"><a name="p3495163252613"></a><a name="p3495163252613"></a>最小值：<strong id="b64963329269"><a name="b64963329269"></a><a name="b64963329269"></a>0</strong></p>
<p id="p19497143210264"><a name="p19497143210264"></a><a name="p19497143210264"></a>最大值：<strong id="b4498163242610"><a name="b4498163242610"></a><a name="b4498163242610"></a>65535</strong></p>
<p id="p949903218266"><a name="p949903218266"></a><a name="p949903218266"></a>最小长度：<strong id="b165005323266"><a name="b165005323266"></a><a name="b165005323266"></a>1</strong></p>
<p id="p250273272616"><a name="p250273272616"></a><a name="p250273272616"></a>最大长度：<strong id="b250233282615"><a name="b250233282615"></a><a name="b250233282615"></a>5</strong></p>
</td>
</tr>
<tr id="row1739753216260"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p950433252620"><a name="p950433252620"></a><a name="p950433252620"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p165061332192616"><a name="p165061332192616"></a><a name="p165061332192616"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p950833262616"><a name="p950833262616"></a><a name="p950833262616"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p15111732162612"><a name="p15111732162612"></a><a name="p15111732162612"></a>Floatingip对外提供服务的端口号。取值范围：0~65535。</p>
<p id="p1513432162616"><a name="p1513432162616"></a><a name="p1513432162616"></a>最小值：<strong id="b6514143213265"><a name="b6514143213265"></a><a name="b6514143213265"></a>0</strong></p>
<p id="p151643211261"><a name="p151643211261"></a><a name="p151643211261"></a>最大值：<strong id="b05166326262"><a name="b05166326262"></a><a name="b05166326262"></a>65535</strong></p>
<p id="p55186321261"><a name="p55186321261"></a><a name="p55186321261"></a>最小长度：<strong id="b3518532142619"><a name="b3518532142619"></a><a name="b3518532142619"></a>1</strong></p>
<p id="p652083232612"><a name="p652083232612"></a><a name="p652083232612"></a>最大长度：<strong id="b852113329262"><a name="b852113329262"></a><a name="b852113329262"></a>10</strong></p>
</td>
</tr>
<tr id="row13397173214262"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p195236325263"><a name="p195236325263"></a><a name="p195236325263"></a>internal_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p952513262617"><a name="p952513262617"></a><a name="p952513262617"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p105281832102615"><a name="p105281832102615"></a><a name="p105281832102615"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p25301932122610"><a name="p25301932122610"></a><a name="p25301932122610"></a>虚拟机或者裸机对外提供服务的协议端口号范围。功能说明：该端口范围与external _service_port_range按顺序实现1:1映射。取值范围：1~65535。约束：只能以’-’字符连接端口范围。</p>
</td>
</tr>
<tr id="row15397932152620"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p19533132102617"><a name="p19533132102617"></a><a name="p19533132102617"></a>external_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p135351328261"><a name="p135351328261"></a><a name="p135351328261"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1537832142612"><a name="p1537832142612"></a><a name="p1537832142612"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p12539183219265"><a name="p12539183219265"></a><a name="p12539183219265"></a>Floatingip对外提供服务的端口号范围。功能说明：该端口范围与internal _service_port_range按顺序实现1:1映射。取值范围：1~65535。约束：只能以’-’字符连接端口范围。</p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section1554216324261"></a>

**状态码： 200**

**表 5**  响应Body参数

<a name="zh-cn_topic_0297140301_responseParameter"></a>
<table><thead align="left"><tr id="row6546193262616"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p2055243262617"><a name="p2055243262617"></a><a name="p2055243262617"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p55553321263"><a name="p55553321263"></a><a name="p55553321263"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p165571732192613"><a name="p165571732192613"></a><a name="p165571732192613"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row45472032152615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1655920328265"><a name="p1655920328265"></a><a name="p1655920328265"></a>dnat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1356211324268"><a name="p1356211324268"></a><a name="p1356211324268"></a><a href="#zh-cn_topic_0297140301_response_NatGatewayDnatRuleResponseBody">NatGatewayDnatRuleResponseBody</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1856683212262"><a name="p1856683212262"></a><a name="p1856683212262"></a>DNAT规则的响应体。</p>
</td>
</tr>
</tbody>
</table>

**表 6**  NatGatewayDnatRuleResponseBody

<a name="zh-cn_topic_0297140301_response_NatGatewayDnatRuleResponseBody"></a>
<table><thead align="left"><tr id="row1756963242610"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p3574103211266"><a name="p3574103211266"></a><a name="p3574103211266"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1577113214261"><a name="p1577113214261"></a><a name="p1577113214261"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p3579163215266"><a name="p3579163215266"></a><a name="p3579163215266"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row25691329265"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1958323216263"><a name="p1958323216263"></a><a name="p1958323216263"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p9585193219269"><a name="p9585193219269"></a><a name="p9585193219269"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p058813202619"><a name="p058813202619"></a><a name="p058813202619"></a>DNAT规则的ID。</p>
<p id="p1059017324262"><a name="p1059017324262"></a><a name="p1059017324262"></a>长度：<strong id="b25911532112614"><a name="b25911532112614"></a><a name="b25911532112614"></a>36</strong></p>
</td>
</tr>
<tr id="row155691632182618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1859643215266"><a name="p1859643215266"></a><a name="p1859643215266"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1659933232616"><a name="p1659933232616"></a><a name="p1659933232616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2601203211268"><a name="p2601203211268"></a><a name="p2601203211268"></a>项目的ID。</p>
</td>
</tr>
<tr id="row11570632182617"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1160393242617"><a name="p1160393242617"></a><a name="p1160393242617"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1560573292620"><a name="p1560573292620"></a><a name="p1560573292620"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p06081932102617"><a name="p06081932102617"></a><a name="p06081932102617"></a>DNAT规则的描述。长度限制为255。</p>
<p id="p2610113272613"><a name="p2610113272613"></a><a name="p2610113272613"></a>最大长度：<strong id="b126105321265"><a name="b126105321265"></a><a name="b126105321265"></a>255</strong></p>
</td>
</tr>
<tr id="row1157011322266"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p261217322267"><a name="p261217322267"></a><a name="p261217322267"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p196141632112610"><a name="p196141632112610"></a><a name="p196141632112610"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1617153213262"><a name="p1617153213262"></a><a name="p1617153213262"></a>虚拟机或者裸机的Port ID，与private_ip参数二选一。</p>
<p id="p2061911327268"><a name="p2061911327268"></a><a name="p2061911327268"></a>长度：<strong id="b36207321260"><a name="b36207321260"></a><a name="b36207321260"></a>36</strong></p>
</td>
</tr>
<tr id="row7570732152618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p3623113282613"><a name="p3623113282613"></a><a name="p3623113282613"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p662618322269"><a name="p662618322269"></a><a name="p662618322269"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11629432162612"><a name="p11629432162612"></a><a name="p11629432162612"></a>用户私有IP地址，例如专线连接的私有云地址，与port_id参数二选一。</p>
</td>
</tr>
<tr id="row19570133212610"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p2631153215261"><a name="p2631153215261"></a><a name="p2631153215261"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p4634193252618"><a name="p4634193252618"></a><a name="p4634193252618"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p18638123262619"><a name="p18638123262619"></a><a name="p18638123262619"></a>虚拟机或者裸机对外提供服务的协议端口号。取值范围：0~65535。</p>
<p id="p16416321269"><a name="p16416321269"></a><a name="p16416321269"></a>最小值：<strong id="b15642143282619"><a name="b15642143282619"></a><a name="b15642143282619"></a>0</strong></p>
<p id="p464483216269"><a name="p464483216269"></a><a name="p464483216269"></a>最大值：<strong id="b9645232122616"><a name="b9645232122616"></a><a name="b9645232122616"></a>65535</strong></p>
<p id="p12646632112610"><a name="p12646632112610"></a><a name="p12646632112610"></a>最小长度：<strong id="b3648113282610"><a name="b3648113282610"></a><a name="b3648113282610"></a>1</strong></p>
<p id="p1665118322267"><a name="p1665118322267"></a><a name="p1665118322267"></a>最大长度：<strong id="b19652932152618"><a name="b19652932152618"></a><a name="b19652932152618"></a>5</strong></p>
</td>
</tr>
<tr id="row1357093262610"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p146547323267"><a name="p146547323267"></a><a name="p146547323267"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p865714327269"><a name="p865714327269"></a><a name="p865714327269"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p46601932112619"><a name="p46601932112619"></a><a name="p46601932112619"></a>公网NAT网关实例的ID。</p>
<p id="p0661432192616"><a name="p0661432192616"></a><a name="p0661432192616"></a>最小长度：<strong id="b6662113213267"><a name="b6662113213267"></a><a name="b6662113213267"></a>1</strong></p>
<p id="p266423218261"><a name="p266423218261"></a><a name="p266423218261"></a>最大长度：<strong id="b3664732142618"><a name="b3664732142618"></a><a name="b3664732142618"></a>36</strong></p>
</td>
</tr>
<tr id="row145700325265"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p56661132112615"><a name="p56661132112615"></a><a name="p56661132112615"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p96691632182612"><a name="p96691632182612"></a><a name="p96691632182612"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p0672432192617"><a name="p0672432192617"></a><a name="p0672432192617"></a>弹性公网IP的id。</p>
<p id="p967493262612"><a name="p967493262612"></a><a name="p967493262612"></a>最小长度：<strong id="b15675203222618"><a name="b15675203222618"></a><a name="b15675203222618"></a>1</strong></p>
<p id="p467723211268"><a name="p467723211268"></a><a name="p467723211268"></a>最大长度：<strong id="b1967833202612"><a name="b1967833202612"></a><a name="b1967833202612"></a>36</strong></p>
</td>
</tr>
<tr id="row12570103212261"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p12680193222613"><a name="p12680193222613"></a><a name="p12680193222613"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p13682132172613"><a name="p13682132172613"></a><a name="p13682132172613"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p116851832102616"><a name="p116851832102616"></a><a name="p116851832102616"></a>弹性公网IP的IP地址。</p>
</td>
</tr>
<tr id="row8570193272612"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p156871232162619"><a name="p156871232162619"></a><a name="p156871232162619"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1969093222617"><a name="p1969093222617"></a><a name="p1969093222617"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p169333282620"><a name="p169333282620"></a><a name="p169333282620"></a>Floatingip对外提供服务的端口号。取值范围：0~65535。</p>
</td>
</tr>
<tr id="row17570932192620"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p669514326269"><a name="p669514326269"></a><a name="p669514326269"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p196976327261"><a name="p196976327261"></a><a name="p196976327261"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p970163214262"><a name="p970163214262"></a><a name="p970163214262"></a>功能说明：DNAT规则的状态。</p>
<p id="p207031432152612"><a name="p207031432152612"></a><a name="p207031432152612"></a>枚举值：</p>
<a name="ul127061332182615"></a><a name="ul127061332182615"></a><ul id="ul127061332182615"><li><strong id="b27091132142618"><a name="b27091132142618"></a><a name="b27091132142618"></a>ACTIVE</strong></li><li><strong id="b97113325265"><a name="b97113325265"></a><a name="b97113325265"></a>PENDING_CREATE</strong></li><li><strong id="b107137324269"><a name="b107137324269"></a><a name="b107137324269"></a>PENDING_UPDATE</strong></li><li><strong id="b371513282615"><a name="b371513282615"></a><a name="b371513282615"></a>PENDING_DELETE</strong></li><li><strong id="b107171532202611"><a name="b107171532202611"></a><a name="b107171532202611"></a>EIP_FREEZED</strong></li><li><strong id="b11720132142617"><a name="b11720132142617"></a><a name="b11720132142617"></a>INACTIVE</strong></li></ul>
</td>
</tr>
<tr id="row657073210267"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1372119323264"><a name="p1372119323264"></a><a name="p1372119323264"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p11723932112616"><a name="p11723932112616"></a><a name="p11723932112616"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p672617322261"><a name="p672617322261"></a><a name="p672617322261"></a>解冻/冻结状态。取值范围：</p>
<a name="ul195721758266"></a><a name="ul195721758266"></a><ul id="ul195721758266"><li>"true"： 解冻</li><li>"false"： 冻结</li></ul>
</td>
</tr>
<tr id="row165708324269"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p2729113262612"><a name="p2729113262612"></a><a name="p2729113262612"></a>internal_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p773133242615"><a name="p773133242615"></a><a name="p773133242615"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p3733173222616"><a name="p3733173222616"></a><a name="p3733173222616"></a>虚拟机或者裸机对外提供服务的协议端口号范围。功能说明：该端口范围与external _service_port_range按顺序实现1:1映射。取值范围：1~65535。约束：只能以’-’字符连接端口范围。</p>
</td>
</tr>
<tr id="row8571932112610"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1273643212617"><a name="p1273643212617"></a><a name="p1273643212617"></a>external_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p57382329263"><a name="p57382329263"></a><a name="p57382329263"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12740103220262"><a name="p12740103220262"></a><a name="p12740103220262"></a>Floatingip对外提供服务的端口号范围。功能说明：该端口范围与internal _service_port_range按顺序实现1:1映射。取值范围：1~65535。约束：只能以’-’字符连接端口范围</p>
</td>
</tr>
<tr id="row1357133252611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p12742123292611"><a name="p12742123292611"></a><a name="p12742123292611"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p074553214262"><a name="p074553214262"></a><a name="p074553214262"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2748173219261"><a name="p2748173219261"></a><a name="p2748173219261"></a>协议类型，目前支持TCP/tcp、UDP/udp、ANY/any。对应协议号6、17、0。</p>
<p id="p1375020326263"><a name="p1375020326263"></a><a name="p1375020326263"></a>最小长度：<strong id="b7750183292616"><a name="b7750183292616"></a><a name="b7750183292616"></a>1</strong></p>
<p id="p1175253216266"><a name="p1175253216266"></a><a name="p1175253216266"></a>最大长度：<strong id="b10752163218264"><a name="b10752163218264"></a><a name="b10752163218264"></a>3</strong></p>
<p id="p1475316327260"><a name="p1475316327260"></a><a name="p1475316327260"></a>枚举值：</p>
<a name="ul275519324264"></a><a name="ul275519324264"></a><ul id="ul275519324264"><li><strong id="b6757173215264"><a name="b6757173215264"></a><a name="b6757173215264"></a>tcp</strong></li><li><strong id="b1575918328261"><a name="b1575918328261"></a><a name="b1575918328261"></a>udp</strong></li><li><strong id="b1176143282617"><a name="b1176143282617"></a><a name="b1176143282617"></a>any</strong></li></ul>
</td>
</tr>
<tr id="row185711232172615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p6763032112618"><a name="p6763032112618"></a><a name="p6763032112618"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p18765143212260"><a name="p18765143212260"></a><a name="p18765143212260"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p476853212612"><a name="p476853212612"></a><a name="p476853212612"></a>DNAT规则的创建时间，遵循UTC时间，格式是yyyy-mm-ddThh:mm:ssZ。</p>
<p id="p1590123217266"><a name="p1590123217266"></a><a name="p1590123217266"></a>最小长度：<strong id="b49022326269"><a name="b49022326269"></a><a name="b49022326269"></a>1</strong></p>
<p id="p8903193219269"><a name="p8903193219269"></a><a name="p8903193219269"></a>最大长度：<strong id="b39031032172617"><a name="b39031032172617"></a><a name="b39031032172617"></a>36</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section6904532102617"></a>

```
PUT https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/dnat_rules/79195d50-0271-41f1-bded-4c089b2502ff

{
  "dnat_rule" : {
    "nat_gateway_id" : "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
    "description" : "my dnat-rules"
  }
}
```

## 响应示例<a name="section6913133282618"></a>

**状态码： 200**

更新DNAT规则成功。

```
{
  "dnat_rule" : {
    "status" : "ACTIVE",
    "nat_gateway_id" : "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
    "admin_state_up" : true,
    "port_id" : "9a469561-daac-4c94-88f5-39366e5ea193",
    "internal_service_port" : 993,
    "protocol" : "tcp",
    "tenant_id" : "d199ba7e0ba64899b2e81518104b1526",
    "floating_ip_id" : "cf99c679-9f41-4dac-8513-9c9228e713e1",
    "created_at" : "2017-11-15 15:44:42.595173",
    "id" : "79195d50-0271-41f1-bded-4c089b2502ff",
    "floating_ip_address" : "5.21.11.226",
    "external_service_port" : 242,
    "description" : "my dnat rule"
  }
}
```

## 状态码<a name="section1993193220263"></a>

<a name="zh-cn_topic_0297140301_status_code"></a>
<table><thead align="left"><tr id="row168111432162614"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p593317327262"><a name="p593317327262"></a><a name="p593317327262"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p11934153219265"><a name="p11934153219265"></a><a name="p11934153219265"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row88124329269"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p14934932182612"><a name="p14934932182612"></a><a name="p14934932182612"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1935153212269"><a name="p1935153212269"></a><a name="p1935153212269"></a>更新DNAT规则成功。</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section7936133215266"></a>

请参见[错误码](错误码.md)。

