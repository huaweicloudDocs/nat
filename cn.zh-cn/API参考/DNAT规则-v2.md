# DNAT规则 v2<a name="nat_api_0031"></a>

<a name="table1351682493510"></a>
<table><thead align="left"><tr id="row1759512463518"><th class="cellrowborder" valign="top" width="26%" id="mcps1.1.5.1.1"><p id="p3595424163511"><a name="p3595424163511"></a><a name="p3595424163511"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="14.44%" id="mcps1.1.5.1.2"><p id="p19512155317473"><a name="p19512155317473"></a><a name="p19512155317473"></a>API功能</p>
</th>
<th class="cellrowborder" valign="top" width="16.75%" id="mcps1.1.5.1.3"><p id="p19595172413511"><a name="p19595172413511"></a><a name="p19595172413511"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="42.809999999999995%" id="mcps1.1.5.1.4"><p id="p1366363695811"><a name="p1366363695811"></a><a name="p1366363695811"></a>授权项作用域</p>
</th>
</tr>
</thead>
<tbody><tr id="row15595192412355"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p12107227135419"><a name="p12107227135419"></a><a name="p12107227135419"></a>POST /v2/{project_id}/dnat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p1469881155416"><a name="p1469881155416"></a><a name="p1469881155416"></a>创建DNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p469815111542"><a name="p469815111542"></a><a name="p469815111542"></a>nat:dnatRules:create</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul5542718184316"></a><a name="ul5542718184316"></a><ul id="ul5542718184316"><li>支持：<a name="ul85758552477"></a><a name="ul85758552477"></a><ul id="ul85758552477"><li>项目 （Project）</li><li>企业项目（Enterprise Project）</li></ul>
</li><li>不支持：无</li></ul>
</td>
</tr>
<tr id="row959782416351"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p1957114117285"><a name="p1957114117285"></a><a name="p1957114117285"></a>POST /v2/{project_id}/dnat_rules/batch</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p8956184112814"><a name="p8956184112814"></a><a name="p8956184112814"></a>批量创建DNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p159567411282"><a name="p159567411282"></a><a name="p159567411282"></a>nat:dnatRules:create</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul59572415289"></a><a name="ul59572415289"></a><ul id="ul59572415289"><li>支持：<a name="ul5957184162816"></a><a name="ul5957184162816"></a><ul id="ul5957184162816"><li>项目 （Project）</li><li>企业项目（Enterprise Project）</li></ul>
</li><li>不支持：无</li></ul>
</td>
</tr>
<tr id="row459717246353"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p8107172795418"><a name="p8107172795418"></a><a name="p8107172795418"></a>GET /v2/{project_id}/dnat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p769941205420"><a name="p769941205420"></a><a name="p769941205420"></a>查询DNAT规则列表</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p156991912543"><a name="p156991912543"></a><a name="p156991912543"></a>nat:dnatRules:list</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul139841920114910"></a><a name="ul139841920114910"></a><ul id="ul139841920114910"><li>支持：<a name="ul7984132054916"></a><a name="ul7984132054916"></a><ul id="ul7984132054916"><li>项目 （Project）</li><li>企业项目（Enterprise Project）</li></ul>
</li><li>不支持：无</li></ul>
</td>
</tr>
<tr id="row1159792493517"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p5107182715545"><a name="p5107182715545"></a><a name="p5107182715545"></a>GET /v2/{project_id}/dnat_rules/{dnat_rule_id }</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p1769917115410"><a name="p1769917115410"></a><a name="p1769917115410"></a>查询DNAT规则详情</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p969914175412"><a name="p969914175412"></a><a name="p969914175412"></a>nat:dnatRules:get</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul1899012201498"></a><a name="ul1899012201498"></a><ul id="ul1899012201498"><li>支持：<a name="ul1599012054911"></a><a name="ul1599012054911"></a><ul id="ul1599012054911"><li>项目 （Project）</li><li>企业项目（Enterprise Project）</li></ul>
</li><li>不支持：无</li></ul>
</td>
</tr>
<tr id="row85979249353"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p121073271543"><a name="p121073271543"></a><a name="p121073271543"></a>DELETE /v2/{project_id}/dnat_rules/{dnat_rule_id}</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p10699191195410"><a name="p10699191195410"></a><a name="p10699191195410"></a>删除DNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p369914116546"><a name="p369914116546"></a><a name="p369914116546"></a>nat:dnatRules:delete</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul599742024914"></a><a name="ul599742024914"></a><ul id="ul599742024914"><li>支持：<a name="ul1199782064914"></a><a name="ul1199782064914"></a><ul id="ul1199782064914"><li>项目 （Project）</li><li>企业项目（Enterprise Project）</li></ul>
</li><li>不支持：无</li></ul>
</td>
</tr>
<tr id="row1972564511415"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p101071927185418"><a name="p101071927185418"></a><a name="p101071927185418"></a>PUT /v2/{project_id}/dnat_rules/{dnat_rule_id}</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p469991165420"><a name="p469991165420"></a><a name="p469991165420"></a>更新DNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p269914195411"><a name="p269914195411"></a><a name="p269914195411"></a>nat:dnatRules:update</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul19352114492"></a><a name="ul19352114492"></a><ul id="ul19352114492"><li>支持：<a name="ul4392112492"></a><a name="ul4392112492"></a><ul id="ul4392112492"><li>项目 （Project）</li><li>企业项目（Enterprise Project）</li></ul>
</li><li>不支持：无</li></ul>
</td>
</tr>
</tbody>
</table>

