# 公网NAT网关SNAT规则<a name="nat_api_0030"></a>

<a name="table1351682493510"></a>
<table><thead align="left"><tr id="row1759512463518"><th class="cellrowborder" valign="top" width="16.951695169516952%" id="mcps1.1.6.1.1"><p id="p6174435204812"><a name="p6174435204812"></a><a name="p6174435204812"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="30.583058305830583%" id="mcps1.1.6.1.2"><p id="p8174113504816"><a name="p8174113504816"></a><a name="p8174113504816"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="21.632163216321633%" id="mcps1.1.6.1.3"><p id="p8701346133717"><a name="p8701346133717"></a><a name="p8701346133717"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="16.271627162716275%" id="mcps1.1.6.1.4"><p id="p5985736163016"><a name="p5985736163016"></a><a name="p5985736163016"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="14.561456145614562%" id="mcps1.1.6.1.5"><p id="p8985133619300"><a name="p8985133619300"></a><a name="p8985133619300"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="row15595192412355"><td class="cellrowborder" valign="top" width="16.951695169516952%" headers="mcps1.1.6.1.1 "><p id="p18200102818515"><a name="p18200102818515"></a><a name="p18200102818515"></a>创建SNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="30.583058305830583%" headers="mcps1.1.6.1.2 "><p id="p11212134219518"><a name="p11212134219518"></a><a name="p11212134219518"></a>POST /v2/{project_id}/snat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="21.632163216321633%" headers="mcps1.1.6.1.3 "><p id="p9200928135113"><a name="p9200928135113"></a><a name="p9200928135113"></a>nat:snatRules:create</p>
</td>
<td class="cellrowborder" valign="top" width="16.271627162716275%" headers="mcps1.1.6.1.4 "><p id="p15756115919276"><a name="p15756115919276"></a><a name="p15756115919276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="14.561456145614562%" headers="mcps1.1.6.1.5 "><p id="p193691154133112"><a name="p193691154133112"></a><a name="p193691154133112"></a>√</p>
</td>
</tr>
<tr id="row959782416351"><td class="cellrowborder" valign="top" width="16.951695169516952%" headers="mcps1.1.6.1.1 "><p id="p320012810516"><a name="p320012810516"></a><a name="p320012810516"></a>查询SNAT规则列表</p>
</td>
<td class="cellrowborder" valign="top" width="30.583058305830583%" headers="mcps1.1.6.1.2 "><p id="p821214215118"><a name="p821214215118"></a><a name="p821214215118"></a>GET /v2/{project_id}/snat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="21.632163216321633%" headers="mcps1.1.6.1.3 "><p id="p102002281512"><a name="p102002281512"></a><a name="p102002281512"></a>nat:snatRules:list</p>
</td>
<td class="cellrowborder" valign="top" width="16.271627162716275%" headers="mcps1.1.6.1.4 "><p id="p1475655902719"><a name="p1475655902719"></a><a name="p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="14.561456145614562%" headers="mcps1.1.6.1.5 "><p id="p153706545313"><a name="p153706545313"></a><a name="p153706545313"></a>√</p>
</td>
</tr>
<tr id="row459717246353"><td class="cellrowborder" valign="top" width="16.951695169516952%" headers="mcps1.1.6.1.1 "><p id="p3200132813513"><a name="p3200132813513"></a><a name="p3200132813513"></a>查询SNAT规则详情</p>
</td>
<td class="cellrowborder" valign="top" width="30.583058305830583%" headers="mcps1.1.6.1.2 "><p id="p321224215512"><a name="p321224215512"></a><a name="p321224215512"></a>GET /v2/{project_id}/snat_rules/{snat_rule_id }</p>
</td>
<td class="cellrowborder" valign="top" width="21.632163216321633%" headers="mcps1.1.6.1.3 "><p id="p1920019289511"><a name="p1920019289511"></a><a name="p1920019289511"></a>nat:snatRules:get</p>
</td>
<td class="cellrowborder" valign="top" width="16.271627162716275%" headers="mcps1.1.6.1.4 "><p id="p167561459142711"><a name="p167561459142711"></a><a name="p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="14.561456145614562%" headers="mcps1.1.6.1.5 "><p id="p1370175418319"><a name="p1370175418319"></a><a name="p1370175418319"></a>√</p>
</td>
</tr>
<tr id="row1159792493517"><td class="cellrowborder" valign="top" width="16.951695169516952%" headers="mcps1.1.6.1.1 "><p id="p17200192835117"><a name="p17200192835117"></a><a name="p17200192835117"></a>删除SNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="30.583058305830583%" headers="mcps1.1.6.1.2 "><p id="p15363181413112"><a name="p15363181413112"></a><a name="p15363181413112"></a>DELETE /v2/{project_id}/nat_gateways/{nat_gateway_id}/snat_rules/{snat_rule_id}</p>
</td>
<td class="cellrowborder" valign="top" width="21.632163216321633%" headers="mcps1.1.6.1.3 "><p id="p220062819517"><a name="p220062819517"></a><a name="p220062819517"></a>nat:snatRules:delete</p>
</td>
<td class="cellrowborder" valign="top" width="16.271627162716275%" headers="mcps1.1.6.1.4 "><p id="p9757145912271"><a name="p9757145912271"></a><a name="p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="14.561456145614562%" headers="mcps1.1.6.1.5 "><p id="p19370155411318"><a name="p19370155411318"></a><a name="p19370155411318"></a>√</p>
</td>
</tr>
<tr id="row85979249353"><td class="cellrowborder" valign="top" width="16.951695169516952%" headers="mcps1.1.6.1.1 "><p id="p20200112816513"><a name="p20200112816513"></a><a name="p20200112816513"></a>更新SNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="30.583058305830583%" headers="mcps1.1.6.1.2 "><p id="p1213742185114"><a name="p1213742185114"></a><a name="p1213742185114"></a>PUT /v2/{project_id}/snat_rules/{snat_rule_id}</p>
</td>
<td class="cellrowborder" valign="top" width="21.632163216321633%" headers="mcps1.1.6.1.3 "><p id="p3200028125112"><a name="p3200028125112"></a><a name="p3200028125112"></a>nat:snatRules:update</p>
</td>
<td class="cellrowborder" valign="top" width="16.271627162716275%" headers="mcps1.1.6.1.4 "><p id="p187577594276"><a name="p187577594276"></a><a name="p187577594276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="14.561456145614562%" headers="mcps1.1.6.1.5 "><p id="p10370105493116"><a name="p10370105493116"></a><a name="p10370105493116"></a>√</p>
</td>
</tr>
</tbody>
</table>

