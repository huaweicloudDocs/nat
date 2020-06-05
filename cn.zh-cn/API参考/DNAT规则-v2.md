# DNAT规则 v2<a name="nat_api_0031"></a>

<a name="table1351682493510"></a>
<table><thead align="left"><tr id="row1759512463518"><th class="cellrowborder" valign="top" width="12.049999999999999%" id="mcps1.1.6.1.1"><p id="p6174435204812"><a name="p6174435204812"></a><a name="p6174435204812"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="26.82%" id="mcps1.1.6.1.2"><p id="p8174113504816"><a name="p8174113504816"></a><a name="p8174113504816"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="19.46%" id="mcps1.1.6.1.3"><p id="p8701346133717"><a name="p8701346133717"></a><a name="p8701346133717"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="23.14%" id="mcps1.1.6.1.4"><p id="p5985736163016"><a name="p5985736163016"></a><a name="p5985736163016"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="18.529999999999998%" id="mcps1.1.6.1.5"><p id="p8985133619300"><a name="p8985133619300"></a><a name="p8985133619300"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="row15595192412355"><td class="cellrowborder" valign="top" width="12.049999999999999%" headers="mcps1.1.6.1.1 "><p id="p1469881155416"><a name="p1469881155416"></a><a name="p1469881155416"></a>创建DNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="26.82%" headers="mcps1.1.6.1.2 "><p id="p12107227135419"><a name="p12107227135419"></a><a name="p12107227135419"></a>POST /v2/{project_id}/dnat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.1.6.1.3 "><p id="p469815111542"><a name="p469815111542"></a><a name="p469815111542"></a>nat:dnatRules:create</p>
</td>
<td class="cellrowborder" valign="top" width="23.14%" headers="mcps1.1.6.1.4 "><p id="p15756115919276"><a name="p15756115919276"></a><a name="p15756115919276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.529999999999998%" headers="mcps1.1.6.1.5 "><p id="p193691154133112"><a name="p193691154133112"></a><a name="p193691154133112"></a>√</p>
</td>
</tr>
<tr id="row959782416351"><td class="cellrowborder" valign="top" width="12.049999999999999%" headers="mcps1.1.6.1.1 "><p id="p8956184112814"><a name="p8956184112814"></a><a name="p8956184112814"></a>批量创建DNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="26.82%" headers="mcps1.1.6.1.2 "><p id="p1957114117285"><a name="p1957114117285"></a><a name="p1957114117285"></a>POST /v2/{project_id}/dnat_rules/batch</p>
</td>
<td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.1.6.1.3 "><p id="p159567411282"><a name="p159567411282"></a><a name="p159567411282"></a>nat:dnatRules:create</p>
</td>
<td class="cellrowborder" valign="top" width="23.14%" headers="mcps1.1.6.1.4 "><p id="p1475655902719"><a name="p1475655902719"></a><a name="p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.529999999999998%" headers="mcps1.1.6.1.5 "><p id="p153706545313"><a name="p153706545313"></a><a name="p153706545313"></a>√</p>
</td>
</tr>
<tr id="row459717246353"><td class="cellrowborder" valign="top" width="12.049999999999999%" headers="mcps1.1.6.1.1 "><p id="p769941205420"><a name="p769941205420"></a><a name="p769941205420"></a>查询DNAT规则列表</p>
</td>
<td class="cellrowborder" valign="top" width="26.82%" headers="mcps1.1.6.1.2 "><p id="p8107172795418"><a name="p8107172795418"></a><a name="p8107172795418"></a>GET /v2/{project_id}/dnat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.1.6.1.3 "><p id="p156991912543"><a name="p156991912543"></a><a name="p156991912543"></a>nat:dnatRules:list</p>
</td>
<td class="cellrowborder" valign="top" width="23.14%" headers="mcps1.1.6.1.4 "><p id="p167561459142711"><a name="p167561459142711"></a><a name="p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.529999999999998%" headers="mcps1.1.6.1.5 "><p id="p1370175418319"><a name="p1370175418319"></a><a name="p1370175418319"></a>√</p>
</td>
</tr>
<tr id="row1159792493517"><td class="cellrowborder" valign="top" width="12.049999999999999%" headers="mcps1.1.6.1.1 "><p id="p1769917115410"><a name="p1769917115410"></a><a name="p1769917115410"></a>查询DNAT规则详情</p>
</td>
<td class="cellrowborder" valign="top" width="26.82%" headers="mcps1.1.6.1.2 "><p id="p5107182715545"><a name="p5107182715545"></a><a name="p5107182715545"></a>GET /v2/{project_id}/dnat_rules/{dnat_rule_id }</p>
</td>
<td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.1.6.1.3 "><p id="p969914175412"><a name="p969914175412"></a><a name="p969914175412"></a>nat:dnatRules:get</p>
</td>
<td class="cellrowborder" valign="top" width="23.14%" headers="mcps1.1.6.1.4 "><p id="p9757145912271"><a name="p9757145912271"></a><a name="p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.529999999999998%" headers="mcps1.1.6.1.5 "><p id="p19370155411318"><a name="p19370155411318"></a><a name="p19370155411318"></a>√</p>
</td>
</tr>
<tr id="row85979249353"><td class="cellrowborder" valign="top" width="12.049999999999999%" headers="mcps1.1.6.1.1 "><p id="p10699191195410"><a name="p10699191195410"></a><a name="p10699191195410"></a>删除DNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="26.82%" headers="mcps1.1.6.1.2 "><p id="p121073271543"><a name="p121073271543"></a><a name="p121073271543"></a>DELETE /v2/{project_id}/dnat_rules/{dnat_rule_id}</p>
</td>
<td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.1.6.1.3 "><p id="p369914116546"><a name="p369914116546"></a><a name="p369914116546"></a>nat:dnatRules:delete</p>
</td>
<td class="cellrowborder" valign="top" width="23.14%" headers="mcps1.1.6.1.4 "><p id="p187577594276"><a name="p187577594276"></a><a name="p187577594276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.529999999999998%" headers="mcps1.1.6.1.5 "><p id="p10370105493116"><a name="p10370105493116"></a><a name="p10370105493116"></a>√</p>
</td>
</tr>
<tr id="row1972564511415"><td class="cellrowborder" valign="top" width="12.049999999999999%" headers="mcps1.1.6.1.1 "><p id="p469991165420"><a name="p469991165420"></a><a name="p469991165420"></a>更新DNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="26.82%" headers="mcps1.1.6.1.2 "><p id="p101071927185418"><a name="p101071927185418"></a><a name="p101071927185418"></a>PUT /v2/{project_id}/dnat_rules/{dnat_rule_id}</p>
</td>
<td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.1.6.1.3 "><p id="p269914195411"><a name="p269914195411"></a><a name="p269914195411"></a>nat:dnatRules:update</p>
</td>
<td class="cellrowborder" valign="top" width="23.14%" headers="mcps1.1.6.1.4 "><p id="p135358527174"><a name="p135358527174"></a><a name="p135358527174"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.529999999999998%" headers="mcps1.1.6.1.5 "><p id="p1853519528177"><a name="p1853519528177"></a><a name="p1853519528177"></a>√</p>
</td>
</tr>
</tbody>
</table>

