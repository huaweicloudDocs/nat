# 批量创建DNAT规则<a name="nat_apiv2_0018"></a>

## 功能介绍<a name="zh-cn_topic_0168797283_section0452742144417"></a>

批量创建DNAT规则。

>![](public_sys-resources/icon-note.gif) **说明：**   
>批量创建规则时，要求网关状态status = "ACTIVE"，要求网关管理员状态admin\_state\_up = True。port\_id和private\_ip不能同时生效。对于all port类型的规则，要求internal\_service\_port = 0，external\_service\_port = 0，protocol = ANY.  

## URI<a name="zh-cn_topic_0168797283_section5452174294414"></a>

POST /v2/\{project\_id\}/dnat\_rules/batch

**表 1**  参数说明

<a name="zh-cn_topic_0168797283_table1545294210449"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797283_row12811184215442"><th class="cellrowborder" valign="top" width="22.939999999999998%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797283_p98111542184413"><a name="zh-cn_topic_0168797283_p98111542184413"></a><a name="zh-cn_topic_0168797283_p98111542184413"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.39%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797283_p9811114218449"><a name="zh-cn_topic_0168797283_p9811114218449"></a><a name="zh-cn_topic_0168797283_p9811114218449"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="11.799999999999999%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797283_p1328082133316"><a name="zh-cn_topic_0168797283_p1328082133316"></a><a name="zh-cn_topic_0168797283_p1328082133316"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="56.87%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797283_p38111642164412"><a name="zh-cn_topic_0168797283_p38111642164412"></a><a name="zh-cn_topic_0168797283_p38111642164412"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797283_row9811442104417"><td class="cellrowborder" valign="top" width="22.939999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797283_p68111142174417"><a name="zh-cn_topic_0168797283_p68111142174417"></a><a name="zh-cn_topic_0168797283_p68111142174417"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.39%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797283_p14811124234414"><a name="zh-cn_topic_0168797283_p14811124234414"></a><a name="zh-cn_topic_0168797283_p14811124234414"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="11.799999999999999%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797283_p6280182110334"><a name="zh-cn_topic_0168797283_p6280182110334"></a><a name="zh-cn_topic_0168797283_p6280182110334"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.87%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797283_p178111342174414"><a name="zh-cn_topic_0168797283_p178111342174414"></a><a name="zh-cn_topic_0168797283_p178111342174414"></a>项目ID。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0168797283_section1946816423448"></a>

请求参数如[表2](#zh-cn_topic_0168797283_table28856916713)所示。

**表 2**  请求参数

<a name="zh-cn_topic_0168797283_table28856916713"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797283_row5885209570"><th class="cellrowborder" valign="top" width="23.02%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797283_p2049917435720"><a name="zh-cn_topic_0168797283_p2049917435720"></a><a name="zh-cn_topic_0168797283_p2049917435720"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.709999999999999%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797283_p14499243574"><a name="zh-cn_topic_0168797283_p14499243574"></a><a name="zh-cn_topic_0168797283_p14499243574"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.509999999999998%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797283_p1949919439710"><a name="zh-cn_topic_0168797283_p1949919439710"></a><a name="zh-cn_topic_0168797283_p1949919439710"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.76%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797283_p20499144315716"><a name="zh-cn_topic_0168797283_p20499144315716"></a><a name="zh-cn_topic_0168797283_p20499144315716"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797283_row388619912716"><td class="cellrowborder" valign="top" width="23.02%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797283_p24997431970"><a name="zh-cn_topic_0168797283_p24997431970"></a><a name="zh-cn_topic_0168797283_p24997431970"></a>dnat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="8.709999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797283_p049914431971"><a name="zh-cn_topic_0168797283_p049914431971"></a><a name="zh-cn_topic_0168797283_p049914431971"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.509999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797283_p13499184318717"><a name="zh-cn_topic_0168797283_p13499184318717"></a><a name="zh-cn_topic_0168797283_p13499184318717"></a>Array(dnat_rule)</p>
</td>
<td class="cellrowborder" valign="top" width="55.76%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797283_p17499154312711"><a name="zh-cn_topic_0168797283_p17499154312711"></a><a name="zh-cn_topic_0168797283_p17499154312711"></a>dnat_rule对象列表。请参考<a href="#zh-cn_topic_0168797283_table194681442154412">表dnat_rule字段说明。</a></p>
</td>
</tr>
</tbody>
</table>

**表 3**  dnat\_rule字段说明

<a name="zh-cn_topic_0168797283_table194681442154412"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797283_row68111242194416"><th class="cellrowborder" valign="top" width="22.57%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797283_p1581114234412"><a name="zh-cn_topic_0168797283_p1581114234412"></a><a name="zh-cn_topic_0168797283_p1581114234412"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.649999999999999%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797283_p168115422448"><a name="zh-cn_topic_0168797283_p168115422448"></a><a name="zh-cn_topic_0168797283_p168115422448"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.9%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797283_p1481118423443"><a name="zh-cn_topic_0168797283_p1481118423443"></a><a name="zh-cn_topic_0168797283_p1481118423443"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.879999999999995%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797283_p981124274420"><a name="zh-cn_topic_0168797283_p981124274420"></a><a name="zh-cn_topic_0168797283_p981124274420"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797283_row88114422445"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797283_p98111842144415"><a name="zh-cn_topic_0168797283_p98111842144415"></a><a name="zh-cn_topic_0168797283_p98111842144415"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797283_p4811134274412"><a name="zh-cn_topic_0168797283_p4811134274412"></a><a name="zh-cn_topic_0168797283_p4811134274412"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797283_p181115427445"><a name="zh-cn_topic_0168797283_p181115427445"></a><a name="zh-cn_topic_0168797283_p181115427445"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797283_p1781114211442"><a name="zh-cn_topic_0168797283_p1781114211442"></a><a name="zh-cn_topic_0168797283_p1781114211442"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row781154215441"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797283_p138111042164413"><a name="zh-cn_topic_0168797283_p138111042164413"></a><a name="zh-cn_topic_0168797283_p138111042164413"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797283_p16811542154414"><a name="zh-cn_topic_0168797283_p16811542154414"></a><a name="zh-cn_topic_0168797283_p16811542154414"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797283_p381144234413"><a name="zh-cn_topic_0168797283_p381144234413"></a><a name="zh-cn_topic_0168797283_p381144234413"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797283_p18811194244414"><a name="zh-cn_topic_0168797283_p18811194244414"></a><a name="zh-cn_topic_0168797283_p18811194244414"></a>虚拟机或者裸机的Port ID，与private_ip参数二选一。获取虚拟机Port ID的方法请参考<a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0077845908.html" target="_blank" rel="noopener noreferrer">查询云服务器网卡信息</a>，获取裸机Port ID的方法请参考<a href="https://support.huaweicloud.com/api-bms/bms_api_0723.html" target="_blank" rel="noopener noreferrer">查询裸金属服务器IP地址</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row1981117422449"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797283_p981104217448"><a name="zh-cn_topic_0168797283_p981104217448"></a><a name="zh-cn_topic_0168797283_p981104217448"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797283_p3811142184414"><a name="zh-cn_topic_0168797283_p3811142184414"></a><a name="zh-cn_topic_0168797283_p3811142184414"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797283_p5811134204410"><a name="zh-cn_topic_0168797283_p5811134204410"></a><a name="zh-cn_topic_0168797283_p5811134204410"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797283_p981110425443"><a name="zh-cn_topic_0168797283_p981110425443"></a><a name="zh-cn_topic_0168797283_p981110425443"></a>用户私有IP地址，例如专线连接的私有云地址，与port_id参数二选一。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row7811642184419"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797283_p9811164213443"><a name="zh-cn_topic_0168797283_p9811164213443"></a><a name="zh-cn_topic_0168797283_p9811164213443"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797283_p98111442104414"><a name="zh-cn_topic_0168797283_p98111442104414"></a><a name="zh-cn_topic_0168797283_p98111442104414"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797283_p176025189536"><a name="zh-cn_topic_0168797283_p176025189536"></a><a name="zh-cn_topic_0168797283_p176025189536"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797283_p19811742104413"><a name="zh-cn_topic_0168797283_p19811742104413"></a><a name="zh-cn_topic_0168797283_p19811742104413"></a>虚拟机或者裸机对外提供服务的协议端口号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row9811174244411"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797283_p981112425442"><a name="zh-cn_topic_0168797283_p981112425442"></a><a name="zh-cn_topic_0168797283_p981112425442"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797283_p10811742174418"><a name="zh-cn_topic_0168797283_p10811742174418"></a><a name="zh-cn_topic_0168797283_p10811742174418"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797283_p1481174210441"><a name="zh-cn_topic_0168797283_p1481174210441"></a><a name="zh-cn_topic_0168797283_p1481174210441"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797283_p5811542194410"><a name="zh-cn_topic_0168797283_p5811542194410"></a><a name="zh-cn_topic_0168797283_p5811542194410"></a>弹性公网IP的id。获取弹性公网IP的id的方法请参考<a href="https://support.huaweicloud.com/api-eip/eip_api_0003.html" target="_blank" rel="noopener noreferrer">查询弹性公网IP列表</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row1281118429443"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797283_p78111442184410"><a name="zh-cn_topic_0168797283_p78111442184410"></a><a name="zh-cn_topic_0168797283_p78111442184410"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797283_p1481113427442"><a name="zh-cn_topic_0168797283_p1481113427442"></a><a name="zh-cn_topic_0168797283_p1481113427442"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797283_p1533002015536"><a name="zh-cn_topic_0168797283_p1533002015536"></a><a name="zh-cn_topic_0168797283_p1533002015536"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797283_p6811742124417"><a name="zh-cn_topic_0168797283_p6811742124417"></a><a name="zh-cn_topic_0168797283_p6811742124417"></a>Floatingip对外提供服务的端口号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row1981174264414"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797283_p0811542144420"><a name="zh-cn_topic_0168797283_p0811542144420"></a><a name="zh-cn_topic_0168797283_p0811542144420"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797283_p16811164294417"><a name="zh-cn_topic_0168797283_p16811164294417"></a><a name="zh-cn_topic_0168797283_p16811164294417"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797283_p1160413391216"><a name="zh-cn_topic_0168797283_p1160413391216"></a><a name="zh-cn_topic_0168797283_p1160413391216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797283_p74511242439"><a name="zh-cn_topic_0168797283_p74511242439"></a><a name="zh-cn_topic_0168797283_p74511242439"></a>协议类型，目前支持TCP、UDP、ANY。</p>
<p id="zh-cn_topic_0168797283_p1445110421435"><a name="zh-cn_topic_0168797283_p1445110421435"></a><a name="zh-cn_topic_0168797283_p1445110421435"></a>对应协议号6、17、0。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row5811194214416"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797283_p1781174284413"><a name="zh-cn_topic_0168797283_p1781174284413"></a><a name="zh-cn_topic_0168797283_p1781174284413"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797283_p681110423445"><a name="zh-cn_topic_0168797283_p681110423445"></a><a name="zh-cn_topic_0168797283_p681110423445"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797283_p192611039133517"><a name="zh-cn_topic_0168797283_p192611039133517"></a><a name="zh-cn_topic_0168797283_p192611039133517"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797283_p138112423448"><a name="zh-cn_topic_0168797283_p138112423448"></a><a name="zh-cn_topic_0168797283_p138112423448"></a>DNAT规则的描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row2024002141215"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797283_p0883629151217"><a name="zh-cn_topic_0168797283_p0883629151217"></a><a name="zh-cn_topic_0168797283_p0883629151217"></a>internal_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797283_p9883172911121"><a name="zh-cn_topic_0168797283_p9883172911121"></a><a name="zh-cn_topic_0168797283_p9883172911121"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797283_p108831229161211"><a name="zh-cn_topic_0168797283_p108831229161211"></a><a name="zh-cn_topic_0168797283_p108831229161211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797283_p388316290125"><a name="zh-cn_topic_0168797283_p388316290125"></a><a name="zh-cn_topic_0168797283_p388316290125"></a>虚拟机或者裸机对外提供服务的协议端口号范围。</p>
<a name="zh-cn_topic_0168797283_ul1688310298125"></a><a name="zh-cn_topic_0168797283_ul1688310298125"></a><ul id="zh-cn_topic_0168797283_ul1688310298125"><li>功能说明：该端口范围与external _service_port_range按顺序实现1:1映射。</li><li>取值范围：1~65535。</li><li>约束：只能以’-’字符连接端口范围。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row5242132161212"><td class="cellrowborder" valign="top" width="22.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797283_p1988302901214"><a name="zh-cn_topic_0168797283_p1988302901214"></a><a name="zh-cn_topic_0168797283_p1988302901214"></a>external_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="8.649999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797283_p1588382991210"><a name="zh-cn_topic_0168797283_p1588382991210"></a><a name="zh-cn_topic_0168797283_p1588382991210"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797283_p1388342971215"><a name="zh-cn_topic_0168797283_p1388342971215"></a><a name="zh-cn_topic_0168797283_p1388342971215"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.879999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797283_p138836293128"><a name="zh-cn_topic_0168797283_p138836293128"></a><a name="zh-cn_topic_0168797283_p138836293128"></a>Floatingip对外提供服务的端口号范围。</p>
<a name="zh-cn_topic_0168797283_ul888342951215"></a><a name="zh-cn_topic_0168797283_ul888342951215"></a><ul id="zh-cn_topic_0168797283_ul888342951215"><li>功能说明：该端口范围与internal _service_port_range按顺序实现1:1映射。</li><li>取值范围：1~65535。</li><li>约束：只能以’-’字符连接端口范围。</li></ul>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="zh-cn_topic_0168797283_section54992424447"></a>

响应参数如[表4](#zh-cn_topic_0168797283_table449984264413)所示。

**表 4**  响应参数

<a name="zh-cn_topic_0168797283_table449984264413"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797283_row1811642144412"><th class="cellrowborder" valign="top" width="24%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797283_p1981118426445"><a name="zh-cn_topic_0168797283_p1981118426445"></a><a name="zh-cn_topic_0168797283_p1981118426445"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="14.360000000000001%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797283_p1381119425449"><a name="zh-cn_topic_0168797283_p1381119425449"></a><a name="zh-cn_topic_0168797283_p1381119425449"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.63999999999999%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797283_p6811124210448"><a name="zh-cn_topic_0168797283_p6811124210448"></a><a name="zh-cn_topic_0168797283_p6811124210448"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797283_row14811174212440"><td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797283_p681174234412"><a name="zh-cn_topic_0168797283_p681174234412"></a><a name="zh-cn_topic_0168797283_p681174234412"></a>dnat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="14.360000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797283_p1341514360311"><a name="zh-cn_topic_0168797283_p1341514360311"></a><a name="zh-cn_topic_0168797283_p1341514360311"></a>Array(dnat_rule)</p>
</td>
<td class="cellrowborder" valign="top" width="61.63999999999999%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797283_p158111142154416"><a name="zh-cn_topic_0168797283_p158111142154416"></a><a name="zh-cn_topic_0168797283_p158111142154416"></a>dnat_rule对象列表。请参考<a href="#zh-cn_topic_0168797283_table551454211441">表dnat_rule字段说明</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 5**  dnat\_rule字段说明

<a name="zh-cn_topic_0168797283_table551454211441"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797283_row1281124218446"><th class="cellrowborder" valign="top" width="24.240000000000002%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797283_p1381117426444"><a name="zh-cn_topic_0168797283_p1381117426444"></a><a name="zh-cn_topic_0168797283_p1381117426444"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797283_p15811104274413"><a name="zh-cn_topic_0168797283_p15811104274413"></a><a name="zh-cn_topic_0168797283_p15811104274413"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.62%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797283_p12811242134410"><a name="zh-cn_topic_0168797283_p12811242134410"></a><a name="zh-cn_topic_0168797283_p12811242134410"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797283_row9811042124416"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797283_p1181144217447"><a name="zh-cn_topic_0168797283_p1181144217447"></a><a name="zh-cn_topic_0168797283_p1181144217447"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797283_p118111742124416"><a name="zh-cn_topic_0168797283_p118111742124416"></a><a name="zh-cn_topic_0168797283_p118111742124416"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797283_p178111342124419"><a name="zh-cn_topic_0168797283_p178111342124419"></a><a name="zh-cn_topic_0168797283_p178111342124419"></a>DNAT规则的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row4811134294416"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797283_p1281110421440"><a name="zh-cn_topic_0168797283_p1281110421440"></a><a name="zh-cn_topic_0168797283_p1281110421440"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797283_p181174234410"><a name="zh-cn_topic_0168797283_p181174234410"></a><a name="zh-cn_topic_0168797283_p181174234410"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797283_p0811164215446"><a name="zh-cn_topic_0168797283_p0811164215446"></a><a name="zh-cn_topic_0168797283_p0811164215446"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row8811164274416"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797283_p2811124210449"><a name="zh-cn_topic_0168797283_p2811124210449"></a><a name="zh-cn_topic_0168797283_p2811124210449"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797283_p10811174220442"><a name="zh-cn_topic_0168797283_p10811174220442"></a><a name="zh-cn_topic_0168797283_p10811174220442"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797283_p108112421448"><a name="zh-cn_topic_0168797283_p108112421448"></a><a name="zh-cn_topic_0168797283_p108112421448"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row5811154254410"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797283_p1811124274411"><a name="zh-cn_topic_0168797283_p1811124274411"></a><a name="zh-cn_topic_0168797283_p1811124274411"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797283_p12811842164417"><a name="zh-cn_topic_0168797283_p12811842164417"></a><a name="zh-cn_topic_0168797283_p12811842164417"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797283_p178112042104414"><a name="zh-cn_topic_0168797283_p178112042104414"></a><a name="zh-cn_topic_0168797283_p178112042104414"></a>虚拟机或者裸机的Port ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row88111642204415"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797283_p18811642164413"><a name="zh-cn_topic_0168797283_p18811642164413"></a><a name="zh-cn_topic_0168797283_p18811642164413"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797283_p1881134294413"><a name="zh-cn_topic_0168797283_p1881134294413"></a><a name="zh-cn_topic_0168797283_p1881134294413"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797283_p38111642124415"><a name="zh-cn_topic_0168797283_p38111642124415"></a><a name="zh-cn_topic_0168797283_p38111642124415"></a>用户私有IP地址，例如专线连接的私有云地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row11811144274420"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797283_p2811742164417"><a name="zh-cn_topic_0168797283_p2811742164417"></a><a name="zh-cn_topic_0168797283_p2811742164417"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797283_p8775202545320"><a name="zh-cn_topic_0168797283_p8775202545320"></a><a name="zh-cn_topic_0168797283_p8775202545320"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797283_p15811104294411"><a name="zh-cn_topic_0168797283_p15811104294411"></a><a name="zh-cn_topic_0168797283_p15811104294411"></a>虚拟机或者裸机对外提供服务的协议端口号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row581113421445"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797283_p108111642164417"><a name="zh-cn_topic_0168797283_p108111642164417"></a><a name="zh-cn_topic_0168797283_p108111642164417"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797283_p58110424446"><a name="zh-cn_topic_0168797283_p58110424446"></a><a name="zh-cn_topic_0168797283_p58110424446"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797283_p1781110421443"><a name="zh-cn_topic_0168797283_p1781110421443"></a><a name="zh-cn_topic_0168797283_p1781110421443"></a>弹性公网IP的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row4811042194419"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797283_p15811174214444"><a name="zh-cn_topic_0168797283_p15811174214444"></a><a name="zh-cn_topic_0168797283_p15811174214444"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797283_p2811144214414"><a name="zh-cn_topic_0168797283_p2811144214414"></a><a name="zh-cn_topic_0168797283_p2811144214414"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797283_p1781194215445"><a name="zh-cn_topic_0168797283_p1781194215445"></a><a name="zh-cn_topic_0168797283_p1781194215445"></a>弹性公网的IP地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row981194215445"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797283_p1281194244411"><a name="zh-cn_topic_0168797283_p1281194244411"></a><a name="zh-cn_topic_0168797283_p1281194244411"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797283_p1317392714537"><a name="zh-cn_topic_0168797283_p1317392714537"></a><a name="zh-cn_topic_0168797283_p1317392714537"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797283_p1681114422448"><a name="zh-cn_topic_0168797283_p1681114422448"></a><a name="zh-cn_topic_0168797283_p1681114422448"></a>Floatingip对外提供服务的端口号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row6811114204416"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797283_p381134284415"><a name="zh-cn_topic_0168797283_p381134284415"></a><a name="zh-cn_topic_0168797283_p381134284415"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797283_p1681114210448"><a name="zh-cn_topic_0168797283_p1681114210448"></a><a name="zh-cn_topic_0168797283_p1681114210448"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797283_p381194224411"><a name="zh-cn_topic_0168797283_p381194224411"></a><a name="zh-cn_topic_0168797283_p381194224411"></a>协议类型，目前支持TCP、UDP、ANY。</p>
<p id="zh-cn_topic_0168797283_p17811742144417"><a name="zh-cn_topic_0168797283_p17811742144417"></a><a name="zh-cn_topic_0168797283_p17811742144417"></a>对应协议号6、17、0。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row20811104294411"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797283_p148110422441"><a name="zh-cn_topic_0168797283_p148110422441"></a><a name="zh-cn_topic_0168797283_p148110422441"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797283_p1221816301363"><a name="zh-cn_topic_0168797283_p1221816301363"></a><a name="zh-cn_topic_0168797283_p1221816301363"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797283_p14811542124419"><a name="zh-cn_topic_0168797283_p14811542124419"></a><a name="zh-cn_topic_0168797283_p14811542124419"></a>DNAT规则的描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row68111042134415"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797283_p1481164284412"><a name="zh-cn_topic_0168797283_p1481164284412"></a><a name="zh-cn_topic_0168797283_p1481164284412"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797283_p181112424447"><a name="zh-cn_topic_0168797283_p181112424447"></a><a name="zh-cn_topic_0168797283_p181112424447"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797283_ul8811194204410"></a><a name="zh-cn_topic_0168797283_ul8811194204410"></a><ul id="zh-cn_topic_0168797283_ul8811194204410"><li>功能说明：DNAT规则的状态。</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row4811124274415"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797283_p1181144294414"><a name="zh-cn_topic_0168797283_p1181144294414"></a><a name="zh-cn_topic_0168797283_p1181144294414"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797283_p1161154912716"><a name="zh-cn_topic_0168797283_p1161154912716"></a><a name="zh-cn_topic_0168797283_p1161154912716"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797283_ul71858556358"></a><a name="zh-cn_topic_0168797283_ul71858556358"></a><ul id="zh-cn_topic_0168797283_ul71858556358"><li>解冻/冻结状态。</li><li>取值范围：<a name="zh-cn_topic_0168797283_ul11838172814409"></a><a name="zh-cn_topic_0168797283_ul11838172814409"></a><ul id="zh-cn_topic_0168797283_ul11838172814409"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row181119428447"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797283_p158111142104417"><a name="zh-cn_topic_0168797283_p158111142104417"></a><a name="zh-cn_topic_0168797283_p158111142104417"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797283_p6811124219448"><a name="zh-cn_topic_0168797283_p6811124219448"></a><a name="zh-cn_topic_0168797283_p6811124219448"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797283_ul148111642104414"></a><a name="zh-cn_topic_0168797283_ul148111642104414"></a><ul id="zh-cn_topic_0168797283_ul148111642104414"><li>DNAT规则的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row3364321168"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797283_p05746112162"><a name="zh-cn_topic_0168797283_p05746112162"></a><a name="zh-cn_topic_0168797283_p05746112162"></a>internal_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797283_p9574101115163"><a name="zh-cn_topic_0168797283_p9574101115163"></a><a name="zh-cn_topic_0168797283_p9574101115163"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797283_p15574181115163"><a name="zh-cn_topic_0168797283_p15574181115163"></a><a name="zh-cn_topic_0168797283_p15574181115163"></a>虚拟机或者裸机对外提供服务的协议端口号范围。</p>
<a name="zh-cn_topic_0168797283_ul20574811131610"></a><a name="zh-cn_topic_0168797283_ul20574811131610"></a><ul id="zh-cn_topic_0168797283_ul20574811131610"><li>功能说明：该端口范围与external _service_port_range按顺序实现1:1映射。</li><li>取值范围：1~65535。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797283_row236482121615"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797283_p957431115161"><a name="zh-cn_topic_0168797283_p957431115161"></a><a name="zh-cn_topic_0168797283_p957431115161"></a>external_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797283_p8574101114163"><a name="zh-cn_topic_0168797283_p8574101114163"></a><a name="zh-cn_topic_0168797283_p8574101114163"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797283_p15574511181613"><a name="zh-cn_topic_0168797283_p15574511181613"></a><a name="zh-cn_topic_0168797283_p15574511181613"></a>Floatingip对外提供服务的端口号范围。</p>
<a name="zh-cn_topic_0168797283_ul1457418115166"></a><a name="zh-cn_topic_0168797283_ul1457418115166"></a><ul id="zh-cn_topic_0168797283_ul1457418115166"><li>功能说明：该端口范围与internal _service_port_range按顺序实现1:1映射。</li><li>取值范围：1~65535。</li></ul>
</td>
</tr>
</tbody>
</table>

## 示例<a name="zh-cn_topic_0168797283_section6577194234413"></a>

-   请求样例
    1.  批量创建规则\(第一条为指定端口的规则，第二条为all port类型的规则\)

        ```
        POST https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/dnat_rules/batch
        { 
             "dnat_rules": [{ 
                 "floating_ip_id": "bf99c679-9f41-4dac-8513-9c9228e713e1", 
                 "nat_gateway_id": "cda3a125-2406-456c-a11f-598e10578541", 
                 "port_id": "9a469561-daac-4c94-88f5-39366e5ea193", 
                 "internal_service_port": 993, 
                 "protocol": "tcp", 
                 "external_service_port": 242 
             },
            { 
                 "floating_ip_id": "cf99c679-9f41-4dac-8513-9c9228e713e1", 
                 "nat_gateway_id": "dda3a125-2406-456c-a11f-598e10578541", 
                 "private_ip": "192.168.1.100", 
                 "internal_service_port": 0, 
                 "protocol": "any", 
                 "external_service_port": 0 
             }]
         }
        ```


-   响应样例
    1.  批量创建规则的响应

        ```
        { 
             "dnat_rules": [{ 
                 "floating_ip_id": "bf99c679-9f41-4dac-8513-9c9228e713e1", 
                 "status": "ACTIVE", 
                 "nat_gateway_id": "cda3a125-2406-456c-a11f-598e10578541", 
                 "admin_state_up": true, 
                 "port_id": "9a469561-daac-4c94-88f5-39366e5ea193",
                 "private_ip": "",  
                 "internal_service_port": 993, 
                 "protocol": "tcp", 
                 "tenant_id": "abc", 
                 "created_at": "2017-11-15 15:44:42.595173", 
                 "id": "79195d50-0271-41f1-bded-4c089b2502ff", 
                 "floating_ip_address": "5.21.11.226", 
                 "external_service_port": 242,
                 "description": "my dnat rule 01"
             }，
        { 
                 "floating_ip_id": "cf99c679-9f41-4dac-8513-9c9228e713e1", 
                 "status": "ACTIVE", 
                 "nat_gateway_id": "dda3a125-2406-456c-a11f-598e10578541", 
                 "admin_state_up": true, 
                 "port_ID": "",
                 "private_ip": "192.168.1.100", 
                 "internal_service_port": 0, 
                 "protocol": "any", 
                 "tenant_id": "abc", 
                 "created_at": "2017-11-15 15:44:42.595173", 
                 "id": "79195d50-0271-41f1-bded-4c089b2502ff", 
                 "floating_ip_address": "5.21.11.227", 
                 "external_service_port": 0,
                 "description": "my dnat rule 01"
             }]
         }
        ```



## 状态码<a name="zh-cn_topic_0168797283_section9593134220447"></a>

请参考[状态码](状态码.md)。

