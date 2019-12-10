# SNAT规则 v2.0<a name="ZH-CN_TOPIC_0201533663"></a>

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
<tbody><tr id="row15595192412355"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p66631741105015"><a name="p66631741105015"></a><a name="p66631741105015"></a>POST /v2.0/snat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p44831228105013"><a name="p44831228105013"></a><a name="p44831228105013"></a>创建SNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p248392805015"><a name="p248392805015"></a><a name="p248392805015"></a>nat:snatRules:create</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul11248145974920"></a><a name="ul11248145974920"></a><ul id="ul11248145974920"><li>支持：<p id="p5248135912498"><a name="p5248135912498"></a><a name="p5248135912498"></a>项目 （Project）</p>
</li><li>不支持：<p id="p724812594495"><a name="p724812594495"></a><a name="p724812594495"></a>企业项目（Enterprise Project）</p>
</li></ul>
</td>
</tr>
<tr id="row959782416351"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p2066320415503"><a name="p2066320415503"></a><a name="p2066320415503"></a>GET /v2.0/snat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p154832284502"><a name="p154832284502"></a><a name="p154832284502"></a>查询SNAT规则列表</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p1448392825014"><a name="p1448392825014"></a><a name="p1448392825014"></a>nat:snatRules:list</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul1225311593490"></a><a name="ul1225311593490"></a><ul id="ul1225311593490"><li>支持：<p id="p7253185914914"><a name="p7253185914914"></a><a name="p7253185914914"></a>项目 （Project）</p>
</li><li>不支持：<p id="p12253059114912"><a name="p12253059114912"></a><a name="p12253059114912"></a>企业项目（Enterprise Project）</p>
</li></ul>
</td>
</tr>
<tr id="row459717246353"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p206631141155012"><a name="p206631141155012"></a><a name="p206631141155012"></a>GET /v2.0/snat_rules/{snat_rule_id }</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p174831828165019"><a name="p174831828165019"></a><a name="p174831828165019"></a>查询SNAT规则详情</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p1748392819501"><a name="p1748392819501"></a><a name="p1748392819501"></a>nat:snatRules:get</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul1225885914917"></a><a name="ul1225885914917"></a><ul id="ul1225885914917"><li>支持：<p id="p1625812596491"><a name="p1625812596491"></a><a name="p1625812596491"></a>项目 （Project）</p>
</li><li>不支持：<p id="p152581359164915"><a name="p152581359164915"></a><a name="p152581359164915"></a>企业项目（Enterprise Project）</p>
</li></ul>
</td>
</tr>
<tr id="row1159792493517"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p1766310412500"><a name="p1766310412500"></a><a name="p1766310412500"></a>DELETE /v2.0/snat_rules/{snat_rule_id}</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p1448317280505"><a name="p1448317280505"></a><a name="p1448317280505"></a>删除SNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p3483142810508"><a name="p3483142810508"></a><a name="p3483142810508"></a>nat:snatRules:delete</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul12264155994914"></a><a name="ul12264155994914"></a><ul id="ul12264155994914"><li>支持：<p id="p22641459144917"><a name="p22641459144917"></a><a name="p22641459144917"></a>项目 （Project）</p>
</li><li>不支持：<p id="p10264159194912"><a name="p10264159194912"></a><a name="p10264159194912"></a>企业项目（Enterprise Project）</p>
</li></ul>
</td>
</tr>
</tbody>
</table>

