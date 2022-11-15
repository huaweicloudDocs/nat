# 查询指定的公网NAT网关详情<a name="ShowNatGateway"></a>

## 功能介绍<a name="section055012011462"></a>

查询指定的公网NAT网关实例详情。

## 调试<a name="section4551142018463"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=nat&api=ShowNatGateway)中调试该接口。

## URI<a name="section3552142010461"></a>

GET /v2/\{project\_id\}/nat\_gateways/\{nat\_gateway\_id\}

**表 1**  路径参数

<a name="table855462016467"></a>
<table><thead align="left"><tr id="row12553182018462"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p125551120154611"><a name="p125551120154611"></a><a name="p125551120154611"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p17555720144613"><a name="p17555720144613"></a><a name="p17555720144613"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1255602010460"><a name="p1255602010460"></a><a name="p1255602010460"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p35561620104612"><a name="p35561620104612"></a><a name="p35561620104612"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row15534206468"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1155672016465"><a name="p1155672016465"></a><a name="p1155672016465"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p25571208464"><a name="p25571208464"></a><a name="p25571208464"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p9557172094617"><a name="p9557172094617"></a><a name="p9557172094617"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p145581420174617"><a name="p145581420174617"></a><a name="p145581420174617"></a>项目的ID。</p>
<p id="p1255822004618"><a name="p1255822004618"></a><a name="p1255822004618"></a>最小长度：<strong id="b25581520174613"><a name="b25581520174613"></a><a name="b25581520174613"></a>1</strong></p>
<p id="p14558162015464"><a name="p14558162015464"></a><a name="p14558162015464"></a>最大长度：<strong id="b7558172011466"><a name="b7558172011466"></a><a name="b7558172011466"></a>36</strong></p>
<p id="p2562026131319"><a name="p2562026131319"></a><a name="p2562026131319"></a>获取方法详见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row195533201460"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p45598203466"><a name="p45598203466"></a><a name="p45598203466"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p355912208469"><a name="p355912208469"></a><a name="p355912208469"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1455912019467"><a name="p1455912019467"></a><a name="p1455912019467"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1356019201468"><a name="p1356019201468"></a><a name="p1356019201468"></a>公网NAT网关实例的ID。</p>
<p id="p115601720164614"><a name="p115601720164614"></a><a name="p115601720164614"></a>长度：<strong id="b1056072034616"><a name="b1056072034616"></a><a name="b1056072034616"></a>36</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section2561152013467"></a>

**表 2**  请求Header参数

<a name="zh-cn_topic_0297140331_HeaderParameter"></a>
<table><thead align="left"><tr id="row1656252054615"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p205649203467"><a name="p205649203467"></a><a name="p205649203467"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p16564720124619"><a name="p16564720124619"></a><a name="p16564720124619"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p185656206465"><a name="p185656206465"></a><a name="p185656206465"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p456515207466"><a name="p456515207466"></a><a name="p456515207466"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1456311204464"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p35651120134615"><a name="p35651120134615"></a><a name="p35651120134615"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p15661520144611"><a name="p15661520144611"></a><a name="p15661520144611"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1256682074619"><a name="p1256682074619"></a><a name="p1256682074619"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p20567920134616"><a name="p20567920134616"></a><a name="p20567920134616"></a>用户Token。用户Token也就是调用获取用户Token获取请求认证接口的响应值，该接口是唯一不需要认证的接口。请求响应成功后在响应消息头中包含的“X-Subject-Token”的值即为Token值。</p>
<p id="p11567720144616"><a name="p11567720144616"></a><a name="p11567720144616"></a>最小长度：<strong id="b1456772044616"><a name="b1456772044616"></a><a name="b1456772044616"></a>1</strong></p>
<p id="p7567122084612"><a name="p7567122084612"></a><a name="p7567122084612"></a>最大长度：<strong id="b256762074613"><a name="b256762074613"></a><a name="b256762074613"></a>10240</strong></p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section1356832012463"></a>

**状态码： 200**

**表 3**  响应Body参数

<a name="zh-cn_topic_0297140331_responseParameter"></a>
<table><thead align="left"><tr id="row11569162012463"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p0570102024615"><a name="p0570102024615"></a><a name="p0570102024615"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p165705200469"><a name="p165705200469"></a><a name="p165705200469"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p18571620134618"><a name="p18571620134618"></a><a name="p18571620134618"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row185696204461"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p7571520134618"><a name="p7571520134618"></a><a name="p7571520134618"></a>nat_gateway</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p125721820154617"><a name="p125721820154617"></a><a name="p125721820154617"></a><a href="#zh-cn_topic_0297140331_response_NatGatewayResponseBody">NatGatewayResponseBody</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p16573920114610"><a name="p16573920114610"></a><a name="p16573920114610"></a>公网NAT网关实例的响应体。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  NatGatewayResponseBody

<a name="zh-cn_topic_0297140331_response_NatGatewayResponseBody"></a>
<table><thead align="left"><tr id="row1357419207462"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p14583182011463"><a name="p14583182011463"></a><a name="p14583182011463"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p13583320124611"><a name="p13583320124611"></a><a name="p13583320124611"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p0584172024617"><a name="p0584172024617"></a><a name="p0584172024617"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row2057442018469"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11584112014464"><a name="p11584112014464"></a><a name="p11584112014464"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p158532010468"><a name="p158532010468"></a><a name="p158532010468"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p14585182014617"><a name="p14585182014617"></a><a name="p14585182014617"></a>公网NAT网关实例的ID。</p>
<p id="p1058582020460"><a name="p1058582020460"></a><a name="p1058582020460"></a>长度：<strong id="b165851220114610"><a name="b165851220114610"></a><a name="b165851220114610"></a>36</strong></p>
</td>
</tr>
<tr id="row5574720104618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p115866206465"><a name="p115866206465"></a><a name="p115866206465"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16587152018466"><a name="p16587152018466"></a><a name="p16587152018466"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p8587162064616"><a name="p8587162064616"></a><a name="p8587162064616"></a>项目的ID。</p>
</td>
</tr>
<tr id="row13575162020467"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p105881020184610"><a name="p105881020184610"></a><a name="p105881020184610"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1358818202465"><a name="p1358818202465"></a><a name="p1358818202465"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1458882044617"><a name="p1458882044617"></a><a name="p1458882044617"></a>公网NAT网关实例的名字，长度限制为64。</p>
<p id="p17588122018466"><a name="p17588122018466"></a><a name="p17588122018466"></a>最小长度：<strong id="b17589620194612"><a name="b17589620194612"></a><a name="b17589620194612"></a>1</strong></p>
<p id="p10589920204612"><a name="p10589920204612"></a><a name="p10589920204612"></a>最大长度：<strong id="b15589172012460"><a name="b15589172012460"></a><a name="b15589172012460"></a>64</strong></p>
</td>
</tr>
<tr id="row857514206468"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1958982054614"><a name="p1958982054614"></a><a name="p1958982054614"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p15589120154610"><a name="p15589120154610"></a><a name="p15589120154610"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p16590320184618"><a name="p16590320184618"></a><a name="p16590320184618"></a>公网NAT网关实例的描述，长度限制为255。</p>
<p id="p759092004610"><a name="p759092004610"></a><a name="p759092004610"></a>最大长度：<strong id="b1559152015467"><a name="b1559152015467"></a><a name="b1559152015467"></a>255</strong></p>
</td>
</tr>
<tr id="row95756201467"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1459102004616"><a name="p1459102004616"></a><a name="p1459102004616"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p14592172054618"><a name="p14592172054618"></a><a name="p14592172054618"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p059362024615"><a name="p059362024615"></a><a name="p059362024615"></a>公网NAT网关的规格。取值为： “1”：小型，SNAT最大连接数10000；“2”：中型，SNAT最大连接数50000；“3”：大型，SNAT最大连接数200000；“4”：超大型，SNAT最大连接数1000000</p>
<p id="p359332064613"><a name="p359332064613"></a><a name="p359332064613"></a>枚举值：</p>
<a name="ul15593102054618"></a><a name="ul15593102054618"></a><ul id="ul15593102054618"><li><strong id="b155941520174619"><a name="b155941520174619"></a><a name="b155941520174619"></a>1</strong></li><li><strong id="b165941020194614"><a name="b165941020194614"></a><a name="b165941020194614"></a>2</strong></li><li><strong id="b459422064618"><a name="b459422064618"></a><a name="b459422064618"></a>3</strong></li><li><strong id="b6595192013462"><a name="b6595192013462"></a><a name="b6595192013462"></a>4</strong></li></ul>
</td>
</tr>
<tr id="row1575182034618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p14595152012463"><a name="p14595152012463"></a><a name="p14595152012463"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p17596202018463"><a name="p17596202018463"></a><a name="p17596202018463"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p559716203466"><a name="p559716203466"></a><a name="p559716203466"></a>公网NAT网关实例的状态。</p>
<p id="p859742014616"><a name="p859742014616"></a><a name="p859742014616"></a>枚举值：</p>
<a name="ul135974205464"></a><a name="ul135974205464"></a><ul id="ul135974205464"><li><strong id="b11597122034611"><a name="b11597122034611"></a><a name="b11597122034611"></a>ACTIVE</strong></li><li><strong id="b1759811202462"><a name="b1759811202462"></a><a name="b1759811202462"></a>PENDING_CREATE</strong></li><li><strong id="b10598162012466"><a name="b10598162012466"></a><a name="b10598162012466"></a>PENDING_UPDATE</strong></li><li><strong id="b15599202019464"><a name="b15599202019464"></a><a name="b15599202019464"></a>PENDING_DELETE</strong></li><li><strong id="b1259932013465"><a name="b1259932013465"></a><a name="b1259932013465"></a>INACTIVE</strong></li></ul>
</td>
</tr>
<tr id="row557552014614"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p175994202464"><a name="p175994202464"></a><a name="p175994202464"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p116007202469"><a name="p116007202469"></a><a name="p116007202469"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p7600162094611"><a name="p7600162094611"></a><a name="p7600162094611"></a>解冻/冻结状态。取值范围：</p>
<a name="ul14600152018461"></a><a name="ul14600152018461"></a><ul id="ul14600152018461"><li>"true"：解冻</li><li>"false"：冻结</li></ul>
</td>
</tr>
<tr id="row1575192016466"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11602102011461"><a name="p11602102011461"></a><a name="p11602102011461"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p06023203469"><a name="p06023203469"></a><a name="p06023203469"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p06022209467"><a name="p06022209467"></a><a name="p06022209467"></a>公网NAT网关实例的创建时间，遵循UTC时间，格式是yyyy-mm-ddThh:mm:ssZ。</p>
</td>
</tr>
<tr id="row55751920184611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p9603920154610"><a name="p9603920154610"></a><a name="p9603920154610"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p10603182018464"><a name="p10603182018464"></a><a name="p10603182018464"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p146049201469"><a name="p146049201469"></a><a name="p146049201469"></a>VPC的id。</p>
</td>
</tr>
<tr id="row85758204465"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15604132010467"><a name="p15604132010467"></a><a name="p15604132010467"></a>internal_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p166054208463"><a name="p166054208463"></a><a name="p166054208463"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p66051920124619"><a name="p66051920124619"></a><a name="p66051920124619"></a>公网NAT网关下行口（DVR的下一跳）所属的network id。</p>
</td>
</tr>
<tr id="row14581162074617"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p16606820104616"><a name="p16606820104616"></a><a name="p16606820104616"></a>enterprise_project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1960792084613"><a name="p1960792084613"></a><a name="p1960792084613"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12607142024616"><a name="p12607142024616"></a><a name="p12607142024616"></a>企业项目ID。创建公网NAT网关实例时，关联的企业项目ID。</p>
<p id="p56076209468"><a name="p56076209468"></a><a name="p56076209468"></a>最大长度：<strong id="b19608132094611"><a name="b19608132094611"></a><a name="b19608132094611"></a>36</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section1160816205460"></a>

```
GET https://{Endpoint}/v2/70505c941b9b4dfd82fd351932328a2f/nat_gateways/14338426-6afe-4019-996b-3a9525296e11

  
```

## 响应示例<a name="section7609720154613"></a>

**状态码： 200**

查询公网NAT网关实例成功。

```
{
  "nat_gateway" : {
    "id" : "14338426-6afe-4019-996b-3a9525296e11",
    "name" : "nat-gateway-name",
    "description" : "nat-gateway-description",
    "spec" : "1",
    "router_id" : "d84f345c-80a1-4fa2-a39c-d0d397c3f09a",
    "tenant_id" : "70505c941b9b4dfd82fd351932328a2f",
    "enterprise_project_id" : "2759da7b-8015-404c-ae0a-a389007b0e2a",
    "internal_network_id" : "89d66639-aacb-4929-969d-07080b0f9fd9",
    "status" : "ACTIVE",
    "admin_state_up" : true,
    "created_at" : "2019-04-22T08:47:13"
  }
}
```

## 状态码<a name="section66144207468"></a>

<a name="zh-cn_topic_0297140331_status_code"></a>
<table><thead align="left"><tr id="row861517203469"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p11616112084610"><a name="p11616112084610"></a><a name="p11616112084610"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p1661782024615"><a name="p1661782024615"></a><a name="p1661782024615"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row13615120114618"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p176171720124613"><a name="p176171720124613"></a><a name="p176171720124613"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p461892044610"><a name="p461892044610"></a><a name="p461892044610"></a>查询公网NAT网关实例成功。</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section4618172084616"></a>

请参见[错误码](错误码.md)。

