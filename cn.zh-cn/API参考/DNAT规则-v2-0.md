# DNAT规则 v2.0<a name="nat_api_0034"></a>

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
<tbody><tr id="row15595192412355"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p172561417115312"><a name="p172561417115312"></a><a name="p172561417115312"></a>POST /v2.0/dnat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p9809687533"><a name="p9809687533"></a><a name="p9809687533"></a>创建DNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p98091989538"><a name="p98091989538"></a><a name="p98091989538"></a>nat:dnatRules:create</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul11248145974920"></a><a name="ul11248145974920"></a><ul id="ul11248145974920"><li>支持：<p id="p5248135912498"><a name="p5248135912498"></a><a name="p5248135912498"></a>项目 （Project）</p>
</li><li>不支持：<p id="p724812594495"><a name="p724812594495"></a><a name="p724812594495"></a>企业项目（Enterprise Project）</p>
</li></ul>
</td>
</tr>
<tr id="row959782416351"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p12256517165318"><a name="p12256517165318"></a><a name="p12256517165318"></a>GET /v2.0/dnat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p1880938125310"><a name="p1880938125310"></a><a name="p1880938125310"></a>查询DNAT规则列表</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p1380958145313"><a name="p1380958145313"></a><a name="p1380958145313"></a>nat:dnatRules:list</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul1225311593490"></a><a name="ul1225311593490"></a><ul id="ul1225311593490"><li>支持：<p id="p7253185914914"><a name="p7253185914914"></a><a name="p7253185914914"></a>项目 （Project）</p>
</li><li>不支持：<p id="p12253059114912"><a name="p12253059114912"></a><a name="p12253059114912"></a>企业项目（Enterprise Project）</p>
</li></ul>
</td>
</tr>
<tr id="row459717246353"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p1925641775311"><a name="p1925641775311"></a><a name="p1925641775311"></a>GET /v2.0/dnat_rules/{dnat_rule_id }</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p58091683536"><a name="p58091683536"></a><a name="p58091683536"></a>查询DNAT规则详情</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p178090816533"><a name="p178090816533"></a><a name="p178090816533"></a>nat:dnatRules:get</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul1225885914917"></a><a name="ul1225885914917"></a><ul id="ul1225885914917"><li>支持：<p id="p1625812596491"><a name="p1625812596491"></a><a name="p1625812596491"></a>项目 （Project）</p>
</li><li>不支持：<p id="p152581359164915"><a name="p152581359164915"></a><a name="p152581359164915"></a>企业项目（Enterprise Project）</p>
</li></ul>
</td>
</tr>
<tr id="row1159792493517"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p1725610177530"><a name="p1725610177530"></a><a name="p1725610177530"></a>DELETE /v2.0/dnat_rules/{dnat_rule_id}</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p3809286538"><a name="p3809286538"></a><a name="p3809286538"></a>删除DNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p128091082532"><a name="p128091082532"></a><a name="p128091082532"></a>nat:dnat_rules:delete</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul12264155994914"></a><a name="ul12264155994914"></a><ul id="ul12264155994914"><li>支持：<p id="p22641459144917"><a name="p22641459144917"></a><a name="p22641459144917"></a>项目 （Project）</p>
</li><li>不支持：<p id="p10264159194912"><a name="p10264159194912"></a><a name="p10264159194912"></a>企业项目（Enterprise Project）</p>
</li></ul>
</td>
</tr>
</tbody>
</table>

