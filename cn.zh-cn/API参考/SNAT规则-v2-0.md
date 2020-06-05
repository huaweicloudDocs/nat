# SNAT规则 v2.0<a name="nat_api_0033"></a>

<a name="table1351682493510"></a>
<table><thead align="left"><tr id="row1759512463518"><th class="cellrowborder" valign="top" width="17.411741174117413%" id="mcps1.1.6.1.1"><p id="p6174435204812"><a name="p6174435204812"></a><a name="p6174435204812"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="28.032803280328032%" id="mcps1.1.6.1.2"><p id="p8174113504816"><a name="p8174113504816"></a><a name="p8174113504816"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="21.442144214421443%" id="mcps1.1.6.1.3"><p id="p8701346133717"><a name="p8701346133717"></a><a name="p8701346133717"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="15.941594159415938%" id="mcps1.1.6.1.4"><p id="p5985736163016"><a name="p5985736163016"></a><a name="p5985736163016"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.1.6.1.5"><p id="p8985133619300"><a name="p8985133619300"></a><a name="p8985133619300"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="row15595192412355"><td class="cellrowborder" valign="top" width="17.411741174117413%" headers="mcps1.1.6.1.1 "><p id="p44831228105013"><a name="p44831228105013"></a><a name="p44831228105013"></a>创建SNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="28.032803280328032%" headers="mcps1.1.6.1.2 "><p id="p66631741105015"><a name="p66631741105015"></a><a name="p66631741105015"></a>POST /v2.0/snat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="21.442144214421443%" headers="mcps1.1.6.1.3 "><p id="p248392805015"><a name="p248392805015"></a><a name="p248392805015"></a>nat:snatRules:create</p>
</td>
<td class="cellrowborder" valign="top" width="15.941594159415938%" headers="mcps1.1.6.1.4 "><p id="p15756115919276"><a name="p15756115919276"></a><a name="p15756115919276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.1.6.1.5 "><p id="p54871102411"><a name="p54871102411"></a><a name="p54871102411"></a>×</p>
</td>
</tr>
<tr id="row959782416351"><td class="cellrowborder" valign="top" width="17.411741174117413%" headers="mcps1.1.6.1.1 "><p id="p154832284502"><a name="p154832284502"></a><a name="p154832284502"></a>查询SNAT规则列表</p>
</td>
<td class="cellrowborder" valign="top" width="28.032803280328032%" headers="mcps1.1.6.1.2 "><p id="p2066320415503"><a name="p2066320415503"></a><a name="p2066320415503"></a>GET /v2.0/snat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="21.442144214421443%" headers="mcps1.1.6.1.3 "><p id="p1448392825014"><a name="p1448392825014"></a><a name="p1448392825014"></a>nat:snatRules:list</p>
</td>
<td class="cellrowborder" valign="top" width="15.941594159415938%" headers="mcps1.1.6.1.4 "><p id="p1475655902719"><a name="p1475655902719"></a><a name="p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.1.6.1.5 "><p id="p153706545313"><a name="p153706545313"></a><a name="p153706545313"></a>×</p>
</td>
</tr>
<tr id="row459717246353"><td class="cellrowborder" valign="top" width="17.411741174117413%" headers="mcps1.1.6.1.1 "><p id="p174831828165019"><a name="p174831828165019"></a><a name="p174831828165019"></a>查询SNAT规则详情</p>
</td>
<td class="cellrowborder" valign="top" width="28.032803280328032%" headers="mcps1.1.6.1.2 "><p id="p206631141155012"><a name="p206631141155012"></a><a name="p206631141155012"></a>GET /v2.0/snat_rules/{snat_rule_id }</p>
</td>
<td class="cellrowborder" valign="top" width="21.442144214421443%" headers="mcps1.1.6.1.3 "><p id="p1748392819501"><a name="p1748392819501"></a><a name="p1748392819501"></a>nat:snatRules:get</p>
</td>
<td class="cellrowborder" valign="top" width="15.941594159415938%" headers="mcps1.1.6.1.4 "><p id="p167561459142711"><a name="p167561459142711"></a><a name="p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.1.6.1.5 "><p id="p1370175418319"><a name="p1370175418319"></a><a name="p1370175418319"></a>×</p>
</td>
</tr>
<tr id="row1159792493517"><td class="cellrowborder" valign="top" width="17.411741174117413%" headers="mcps1.1.6.1.1 "><p id="p1448317280505"><a name="p1448317280505"></a><a name="p1448317280505"></a>删除SNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="28.032803280328032%" headers="mcps1.1.6.1.2 "><p id="p1766310412500"><a name="p1766310412500"></a><a name="p1766310412500"></a>DELETE /v2.0/snat_rules/{snat_rule_id}</p>
</td>
<td class="cellrowborder" valign="top" width="21.442144214421443%" headers="mcps1.1.6.1.3 "><p id="p3483142810508"><a name="p3483142810508"></a><a name="p3483142810508"></a>nat:snatRules:delete</p>
</td>
<td class="cellrowborder" valign="top" width="15.941594159415938%" headers="mcps1.1.6.1.4 "><p id="p9757145912271"><a name="p9757145912271"></a><a name="p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.1.6.1.5 "><p id="p19370155411318"><a name="p19370155411318"></a><a name="p19370155411318"></a>×</p>
</td>
</tr>
</tbody>
</table>

