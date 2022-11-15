# 查询公网NAT网关列表<a name="ListNatGateways"></a>

## 功能介绍<a name="section83721204465"></a>

查询公网NAT网关实例列表。

## 接口约束<a name="section113731720184615"></a>

可以在URI后面用'?'和'&'添加不同的查询条件组合。支持参数说明中所有非必选参数过滤，请参考请求样例。

## 调试<a name="section63731320194614"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=nat&api=ListNatGateways)中调试该接口。

## URI<a name="section637432011464"></a>

GET /v2/\{project\_id\}/nat\_gateways

**表 1**  路径参数

<a name="table17376182034619"></a>
<table><thead align="left"><tr id="row14375122094612"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p0376172064614"><a name="p0376172064614"></a><a name="p0376172064614"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p33771120154619"><a name="p33771120154619"></a><a name="p33771120154619"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p137732014467"><a name="p137732014467"></a><a name="p137732014467"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p1737742011468"><a name="p1737742011468"></a><a name="p1737742011468"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row11375142094610"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p123781020124612"><a name="p123781020124612"></a><a name="p123781020124612"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p73781720104618"><a name="p73781720104618"></a><a name="p73781720104618"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p17379820164614"><a name="p17379820164614"></a><a name="p17379820164614"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p5379202034618"><a name="p5379202034618"></a><a name="p5379202034618"></a>项目的ID。</p>
<p id="p137962074618"><a name="p137962074618"></a><a name="p137962074618"></a>最小长度：<strong id="b838018205463"><a name="b838018205463"></a><a name="b838018205463"></a>1</strong></p>
<p id="p1238013209466"><a name="p1238013209466"></a><a name="p1238013209466"></a>最大长度：<strong id="b12380152074619"><a name="b12380152074619"></a><a name="b12380152074619"></a>36</strong></p>
<p id="p2562026131319"><a name="p2562026131319"></a><a name="p2562026131319"></a>获取方法详见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  Query参数

<a name="table103851620184618"></a>
<table><thead align="left"><tr id="row53831220134616"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p18385192004617"><a name="p18385192004617"></a><a name="p18385192004617"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p538616205463"><a name="p538616205463"></a><a name="p538616205463"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1538602044616"><a name="p1538602044616"></a><a name="p1538602044616"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p15387420174612"><a name="p15387420174612"></a><a name="p15387420174612"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row8383182019469"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p8387520124616"><a name="p8387520124616"></a><a name="p8387520124616"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p16387320124612"><a name="p16387320124612"></a><a name="p16387320124612"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p3388020164611"><a name="p3388020164611"></a><a name="p3388020164611"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p16388112013469"><a name="p16388112013469"></a><a name="p16388112013469"></a>项目的ID。</p>
<p id="p199086515158"><a name="p199086515158"></a><a name="p199086515158"></a>获取方法详见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row138322044618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p133896206463"><a name="p133896206463"></a><a name="p133896206463"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p163893207463"><a name="p163893207463"></a><a name="p163893207463"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p16389142011464"><a name="p16389142011464"></a><a name="p16389142011464"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1639012018465"><a name="p1639012018465"></a><a name="p1639012018465"></a>公网NAT网关实例的ID。</p>
<p id="p63904205468"><a name="p63904205468"></a><a name="p63904205468"></a>最小长度：<strong id="b1039010202467"><a name="b1039010202467"></a><a name="b1039010202467"></a>1</strong></p>
<p id="p19390132054618"><a name="p19390132054618"></a><a name="p19390132054618"></a>最大长度：<strong id="b16390142024617"><a name="b16390142024617"></a><a name="b16390142024617"></a>36</strong></p>
</td>
</tr>
<tr id="row438322019464"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1139142011469"><a name="p1139142011469"></a><a name="p1139142011469"></a>enterprise_project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p239132012465"><a name="p239132012465"></a><a name="p239132012465"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p83921120134620"><a name="p83921120134620"></a><a name="p83921120134620"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1339262014466"><a name="p1339262014466"></a><a name="p1339262014466"></a>企业项目ID。创建公网NAT网关实例时，关联的企业项目ID。</p>
<p id="p8392192011464"><a name="p8392192011464"></a><a name="p8392192011464"></a>最大长度：<strong id="b1639215206469"><a name="b1639215206469"></a><a name="b1639215206469"></a>36</strong></p>
</td>
</tr>
<tr id="row183841920134615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p16393820184617"><a name="p16393820184617"></a><a name="p16393820184617"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1439322034619"><a name="p1439322034619"></a><a name="p1439322034619"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p15393192019469"><a name="p15393192019469"></a><a name="p15393192019469"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p639412202467"><a name="p639412202467"></a><a name="p639412202467"></a>公网NAT网关实例的描述，长度限制为255。</p>
<p id="p439410209462"><a name="p439410209462"></a><a name="p439410209462"></a>最大长度：<strong id="b1739412204468"><a name="b1739412204468"></a><a name="b1739412204468"></a>255</strong></p>
</td>
</tr>
<tr id="row83849200461"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p12394172017467"><a name="p12394172017467"></a><a name="p12394172017467"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p4395112044612"><a name="p4395112044612"></a><a name="p4395112044612"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p18395192014462"><a name="p18395192014462"></a><a name="p18395192014462"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p839614202465"><a name="p839614202465"></a><a name="p839614202465"></a>公网NAT网关实例的创建时间，遵循UTC时间，格式是yyyy-mm-ddThh:mm:ssZ。</p>
<p id="p43961920174620"><a name="p43961920174620"></a><a name="p43961920174620"></a>最小长度：<strong id="b8396202011468"><a name="b8396202011468"></a><a name="b8396202011468"></a>1</strong></p>
<p id="p14396920154611"><a name="p14396920154611"></a><a name="p14396920154611"></a>最大长度：<strong id="b539762044615"><a name="b539762044615"></a><a name="b539762044615"></a>36</strong></p>
</td>
</tr>
<tr id="row5384182012465"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p0397720134618"><a name="p0397720134618"></a><a name="p0397720134618"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1039812011467"><a name="p1039812011467"></a><a name="p1039812011467"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p7398142017467"><a name="p7398142017467"></a><a name="p7398142017467"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p113991620194615"><a name="p113991620194615"></a><a name="p113991620194615"></a>公网NAT网关实例的名字，长度限制为64。公网NAT网关实例的名字仅支持数字、字母、_（下划线）、-（中划线）、中文</p>
<p id="p83992201464"><a name="p83992201464"></a><a name="p83992201464"></a>最小长度：<strong id="b239962014469"><a name="b239962014469"></a><a name="b239962014469"></a>1</strong></p>
<p id="p17399162064611"><a name="p17399162064611"></a><a name="p17399162064611"></a>最大长度：<strong id="b1339920202468"><a name="b1339920202468"></a><a name="b1339920202468"></a>64</strong></p>
</td>
</tr>
<tr id="row193843209466"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p94009204467"><a name="p94009204467"></a><a name="p94009204467"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p24001820184610"><a name="p24001820184610"></a><a name="p24001820184610"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p9401192014465"><a name="p9401192014465"></a><a name="p9401192014465"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p640112013461"><a name="p640112013461"></a><a name="p640112013461"></a>公网NAT网关实例的状态。</p>
<p id="p24011420194617"><a name="p24011420194617"></a><a name="p24011420194617"></a>枚举值：</p>
<a name="ul14402420114611"></a><a name="ul14402420114611"></a><ul id="ul14402420114611"><li><strong id="b16402820104617"><a name="b16402820104617"></a><a name="b16402820104617"></a>ACTIVE</strong></li><li><strong id="b124031520124620"><a name="b124031520124620"></a><a name="b124031520124620"></a>PENDING_CREATE</strong></li><li><strong id="b4403202017462"><a name="b4403202017462"></a><a name="b4403202017462"></a>PENDING_UPDATE</strong></li><li><strong id="b0403132020466"><a name="b0403132020466"></a><a name="b0403132020466"></a>PENDING_DELETE</strong></li><li><strong id="b7404420164619"><a name="b7404420164619"></a><a name="b7404420164619"></a>INACTIVE</strong></li></ul>
</td>
</tr>
<tr id="row93848209465"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1340415203467"><a name="p1340415203467"></a><a name="p1340415203467"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p4405132011465"><a name="p4405132011465"></a><a name="p4405132011465"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p3405142034611"><a name="p3405142034611"></a><a name="p3405142034611"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p7406202044619"><a name="p7406202044619"></a><a name="p7406202044619"></a>公网NAT网关实例的规格。取值为： "1"：小型，SNAT最大连接数10000；"2"：中型，SNAT最大连接数50000；"3"：大型，SNAT最大连接数200000；"4"：超大型，SNAT最大连接数1000000</p>
<p id="p740612015468"><a name="p740612015468"></a><a name="p740612015468"></a>枚举值：</p>
<a name="ul134069208465"></a><a name="ul134069208465"></a><ul id="ul134069208465"><li><strong id="b124071220124616"><a name="b124071220124616"></a><a name="b124071220124616"></a>1</strong></li><li><strong id="b44075207462"><a name="b44075207462"></a><a name="b44075207462"></a>2</strong></li><li><strong id="b4407132084615"><a name="b4407132084615"></a><a name="b4407132084615"></a>3</strong></li><li><strong id="b11408142010466"><a name="b11408142010466"></a><a name="b11408142010466"></a>4</strong></li></ul>
</td>
</tr>
<tr id="row8384192014463"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1740892034614"><a name="p1740892034614"></a><a name="p1740892034614"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p4409152054616"><a name="p4409152054616"></a><a name="p4409152054616"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p9409112018469"><a name="p9409112018469"></a><a name="p9409112018469"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p13721521182813"><a name="p13721521182813"></a><a name="p13721521182813"></a>解冻/冻结状态。取值范围：</p>
<a name="ul3371163418288"></a><a name="ul3371163418288"></a><ul id="ul3371163418288"><li>"true"：解冻</li><li>"false"：冻结</li></ul>
</td>
</tr>
<tr id="row73842020164616"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p241322044616"><a name="p241322044616"></a><a name="p241322044616"></a>internal_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p941392010463"><a name="p941392010463"></a><a name="p941392010463"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p2414820194612"><a name="p2414820194612"></a><a name="p2414820194612"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p841412016462"><a name="p841412016462"></a><a name="p841412016462"></a>公网NAT网关下行口（DVR的下一跳）所属的network id。</p>
<p id="p4415520114615"><a name="p4415520114615"></a><a name="p4415520114615"></a>长度：<strong id="b124151120154618"><a name="b124151120154618"></a><a name="b124151120154618"></a>36</strong></p>
</td>
</tr>
<tr id="row1138442034612"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p74154206466"><a name="p74154206466"></a><a name="p74154206466"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p54168209468"><a name="p54168209468"></a><a name="p54168209468"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p13416132074610"><a name="p13416132074610"></a><a name="p13416132074610"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p2041862044616"><a name="p2041862044616"></a><a name="p2041862044616"></a>VPC的id。</p>
<p id="p1241842084618"><a name="p1241842084618"></a><a name="p1241842084618"></a>长度：<strong id="b34181320154615"><a name="b34181320154615"></a><a name="b34181320154615"></a>36</strong></p>
</td>
</tr>
<tr id="row1838411206466"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1841972014463"><a name="p1841972014463"></a><a name="p1841972014463"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p164205203462"><a name="p164205203462"></a><a name="p164205203462"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p9421132012465"><a name="p9421132012465"></a><a name="p9421132012465"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p542122012465"><a name="p542122012465"></a><a name="p542122012465"></a>功能说明：每页返回的个数。取值范围：0~2000。默认值：2000。</p>
<p id="p5421202094618"><a name="p5421202094618"></a><a name="p5421202094618"></a>最小值：<strong id="b0371142055417"><a name="b0371142055417"></a><a name="b0371142055417"></a>0</strong></p>
<p id="p2422192018468"><a name="p2422192018468"></a><a name="p2422192018468"></a>最大值：<strong id="b12422102011465"><a name="b12422102011465"></a><a name="b12422102011465"></a>2000</strong></p>
<p id="p17422920134610"><a name="p17422920134610"></a><a name="p17422920134610"></a>缺省值：<strong id="b124231320194616"><a name="b124231320194616"></a><a name="b124231320194616"></a>2000</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section13423112016467"></a>

**表 3**  请求Header参数

<a name="zh-cn_topic_0297140339_HeaderParameter"></a>
<table><thead align="left"><tr id="row14424152034615"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p18426120104616"><a name="p18426120104616"></a><a name="p18426120104616"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p1042682013469"><a name="p1042682013469"></a><a name="p1042682013469"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p7426162016465"><a name="p7426162016465"></a><a name="p7426162016465"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p8427142034611"><a name="p8427142034611"></a><a name="p8427142034611"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row64241120134618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1042702074610"><a name="p1042702074610"></a><a name="p1042702074610"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p194281420164610"><a name="p194281420164610"></a><a name="p194281420164610"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1042819200468"><a name="p1042819200468"></a><a name="p1042819200468"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p15428102016461"><a name="p15428102016461"></a><a name="p15428102016461"></a>用户Token。用户Token也就是调用获取用户Token获取请求认证接口的响应值，该接口是唯一不需要认证的接口。请求响应成功后在响应消息头中包含的“X-Subject-Token”的值即为Token值。</p>
<p id="p18429172074619"><a name="p18429172074619"></a><a name="p18429172074619"></a>最小长度：<strong id="b2042982010462"><a name="b2042982010462"></a><a name="b2042982010462"></a>1</strong></p>
<p id="p11429162015469"><a name="p11429162015469"></a><a name="p11429162015469"></a>最大长度：<strong id="b15429420154612"><a name="b15429420154612"></a><a name="b15429420154612"></a>10240</strong></p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section1742962015465"></a>

**状态码： 200**

**表 4**  响应Body参数

<a name="zh-cn_topic_0297140339_responseParameter"></a>
<table><thead align="left"><tr id="row6430122074617"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p7431122018467"><a name="p7431122018467"></a><a name="p7431122018467"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p943215203462"><a name="p943215203462"></a><a name="p943215203462"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1643214209466"><a name="p1643214209466"></a><a name="p1643214209466"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row34313207468"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p5433220174614"><a name="p5433220174614"></a><a name="p5433220174614"></a>nat_gateways</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p64331720104611"><a name="p64331720104611"></a><a name="p64331720104611"></a>Array of <a href="#zh-cn_topic_0297140339_response_NatGatewayResponseBody">NatGatewayResponseBody</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1543411209463"><a name="p1543411209463"></a><a name="p1543411209463"></a>查询公网NAT网关实例列表的响应体。详见NatGateway字段说明。</p>
</td>
</tr>
</tbody>
</table>

**表 5**  NatGatewayResponseBody

<a name="zh-cn_topic_0297140339_response_NatGatewayResponseBody"></a>
<table><thead align="left"><tr id="row64366206461"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p143842013466"><a name="p143842013466"></a><a name="p143842013466"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p10438162015464"><a name="p10438162015464"></a><a name="p10438162015464"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1843911207461"><a name="p1843911207461"></a><a name="p1843911207461"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row9436172044620"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p16439182011461"><a name="p16439182011461"></a><a name="p16439182011461"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p9439142024614"><a name="p9439142024614"></a><a name="p9439142024614"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p144013203462"><a name="p144013203462"></a><a name="p144013203462"></a>公网NAT网关实例的ID。</p>
<p id="p2440162016465"><a name="p2440162016465"></a><a name="p2440162016465"></a>长度：<strong id="b14441112044620"><a name="b14441112044620"></a><a name="b14441112044620"></a>36</strong></p>
</td>
</tr>
<tr id="row7436192044617"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1944172094617"><a name="p1944172094617"></a><a name="p1944172094617"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p10442720184616"><a name="p10442720184616"></a><a name="p10442720184616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17442112013469"><a name="p17442112013469"></a><a name="p17442112013469"></a>项目的ID。</p>
</td>
</tr>
<tr id="row10436220104615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p184431020154612"><a name="p184431020154612"></a><a name="p184431020154612"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p044311205464"><a name="p044311205464"></a><a name="p044311205464"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p124441620114611"><a name="p124441620114611"></a><a name="p124441620114611"></a>公网NAT网关实例的名字，长度限制为64。</p>
<p id="p14441206465"><a name="p14441206465"></a><a name="p14441206465"></a>最小长度：<strong id="b94443206462"><a name="b94443206462"></a><a name="b94443206462"></a>1</strong></p>
<p id="p184442208469"><a name="p184442208469"></a><a name="p184442208469"></a>最大长度：<strong id="b1444415204468"><a name="b1444415204468"></a><a name="b1444415204468"></a>64</strong></p>
</td>
</tr>
<tr id="row17436172010464"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p174453206467"><a name="p174453206467"></a><a name="p174453206467"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1344522014618"><a name="p1344522014618"></a><a name="p1344522014618"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p194461820194611"><a name="p194461820194611"></a><a name="p194461820194611"></a>公网NAT网关实例的描述，长度限制为255。</p>
<p id="p184466202461"><a name="p184466202461"></a><a name="p184466202461"></a>最大长度：<strong id="b1446120134612"><a name="b1446120134612"></a><a name="b1446120134612"></a>255</strong></p>
</td>
</tr>
<tr id="row443682011468"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4447162019465"><a name="p4447162019465"></a><a name="p4447162019465"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1447192044613"><a name="p1447192044613"></a><a name="p1447192044613"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p73909583379"><a name="p73909583379"></a><a name="p73909583379"></a>公网NAT网关的规格。取值为：“1”：小型，SNAT最大连接数10000；“2”：中型，SNAT最大连接数50000；“3”：大型，SNAT最大连接数200000；“4”：超大型，SNAT最大连接数1000000</p>
<p id="p14448112010463"><a name="p14448112010463"></a><a name="p14448112010463"></a>枚举值：</p>
<a name="ul1644852074612"></a><a name="ul1644852074612"></a><ul id="ul1644852074612"><li><strong id="b11452182018460"><a name="b11452182018460"></a><a name="b11452182018460"></a>1</strong></li><li><strong id="b54538203467"><a name="b54538203467"></a><a name="b54538203467"></a>2</strong></li><li><strong id="b94531920174610"><a name="b94531920174610"></a><a name="b94531920174610"></a>3</strong></li><li><strong id="b124531420184613"><a name="b124531420184613"></a><a name="b124531420184613"></a>4</strong></li></ul>
</td>
</tr>
<tr id="row943611208468"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p24541120114616"><a name="p24541120114616"></a><a name="p24541120114616"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p545422014611"><a name="p545422014611"></a><a name="p545422014611"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p94551820104614"><a name="p94551820104614"></a><a name="p94551820104614"></a>公网NAT网关实例的状态。</p>
<p id="p164551420184614"><a name="p164551420184614"></a><a name="p164551420184614"></a>枚举值：</p>
<a name="ul1545512204466"></a><a name="ul1545512204466"></a><ul id="ul1545512204466"><li><strong id="b14455162064612"><a name="b14455162064612"></a><a name="b14455162064612"></a>ACTIVE</strong></li><li><strong id="b154569206460"><a name="b154569206460"></a><a name="b154569206460"></a>PENDING_CREATE</strong></li><li><strong id="b6456152017465"><a name="b6456152017465"></a><a name="b6456152017465"></a>PENDING_UPDATE</strong></li><li><strong id="b164561420134615"><a name="b164561420134615"></a><a name="b164561420134615"></a>PENDING_DELETE</strong></li><li><strong id="b20456162014460"><a name="b20456162014460"></a><a name="b20456162014460"></a>INACTIVE</strong></li></ul>
</td>
</tr>
<tr id="row1143616207461"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p44571220174618"><a name="p44571220174618"></a><a name="p44571220174618"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p9457192084618"><a name="p9457192084618"></a><a name="p9457192084618"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p134589206464"><a name="p134589206464"></a><a name="p134589206464"></a>解冻/冻结状态。取值范围：</p>
<a name="ul1945817202463"></a><a name="ul1945817202463"></a><ul id="ul1945817202463"><li>"true"：解冻</li><li>"false"：冻结</li></ul>
</td>
</tr>
<tr id="row1643616200463"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1745962012466"><a name="p1745962012466"></a><a name="p1745962012466"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1046072084617"><a name="p1046072084617"></a><a name="p1046072084617"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p14607206464"><a name="p14607206464"></a><a name="p14607206464"></a>公网NAT网关实例的创建时间，遵循UTC时间，格式是yyyy-mm-ddThh:mm:ssZ。</p>
</td>
</tr>
<tr id="row343610202463"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p124601220164616"><a name="p124601220164616"></a><a name="p124601220164616"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p154618203460"><a name="p154618203460"></a><a name="p154618203460"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1046111208462"><a name="p1046111208462"></a><a name="p1046111208462"></a>VPC的id。</p>
</td>
</tr>
<tr id="row13436320134618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p17462112019462"><a name="p17462112019462"></a><a name="p17462112019462"></a>internal_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p946232012462"><a name="p946232012462"></a><a name="p946232012462"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1246342010460"><a name="p1246342010460"></a><a name="p1246342010460"></a>公网NAT网关下行口（DVR的下一跳）所属的network id。</p>
</td>
</tr>
<tr id="row8436182064618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1446372044610"><a name="p1446372044610"></a><a name="p1446372044610"></a>enterprise_project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p17464112012468"><a name="p17464112012468"></a><a name="p17464112012468"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p16464120194618"><a name="p16464120194618"></a><a name="p16464120194618"></a>企业项目ID。创建公网NAT网关实例时，关联的企业项目ID。</p>
<p id="p11464182054610"><a name="p11464182054610"></a><a name="p11464182054610"></a>最大长度：<strong id="b5464420164611"><a name="b5464420164611"></a><a name="b5464420164611"></a>36</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section94651120194612"></a>

```
GET https://{Endpoint}/v2/27e25061336f4af590faeabeb7fcd9a3/nat_gateways?status=ACTIVE

  
```

## 响应示例<a name="section44671207465"></a>

**状态码： 200**

查询公网NAT网关实例列表成功

```
{
  "nat_gateways" : [ {
    "id" : "a253be25-ae7c-4013-978b-3c0785eccd63",
    "router_id" : "b1d81744-5165-48b8-916e-e56626feb88f",
    "status" : "ACTIVE",
    "description" : "nat01",
    "admin_state_up" : true,
    "tenant_id" : "27e25061336f4af590faeabeb7fcd9a3",
    "created_at" : "2017-11-15 14:50:39.505112",
    "spec" : "2",
    "internal_network_id" : "5930796a-6026-4d8b-8790-6c6bfc9f87e8",
    "name" : "wj3",
    "enterprise_project_id" : "0aad99bc-f5f6-4f78-8404-c598d76b0ed2"
  }, {
    "id" : "e824f1b4-4290-4ebc-8322-cfff370dbd1e",
    "router_id" : "305dc52f-13dd-429b-a2d4-444a1039ba0b",
    "status" : "ACTIVE",
    "description" : "1234",
    "admin_state_up" : true,
    "tenant_id" : "27e25061336f4af590faeabeb7fcd9a3",
    "created_at" : "2017-11-17 07:41:07.538062",
    "spec" : "2",
    "internal_network_id" : "fc09463b-4ef8-4c7a-93c8-92d9ca6daf9d",
    "name" : "lyl001",
    "enterprise_project_id" : "0"
  } ]
}
```

## 状态码<a name="section99203209461"></a>

<a name="zh-cn_topic_0297140339_status_code"></a>
<table><thead align="left"><tr id="row947610206467"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p1921920134616"><a name="p1921920134616"></a><a name="p1921920134616"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p792162054615"><a name="p792162054615"></a><a name="p792162054615"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row19476132014616"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p29213205465"><a name="p29213205465"></a><a name="p29213205465"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p139214206467"><a name="p139214206467"></a><a name="p139214206467"></a>查询公网NAT网关实例列表成功</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section2921132054617"></a>

请参见[错误码](错误码.md)。

