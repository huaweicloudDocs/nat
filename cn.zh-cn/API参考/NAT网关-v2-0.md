# NAT网关 v2.0<a name="ZH-CN_TOPIC_0201533679"></a>

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
<tbody><tr id="row15595192412355"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p872832315425"><a name="p872832315425"></a><a name="p872832315425"></a>POST /v2.0/nat_gateways</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p99845386429"><a name="p99845386429"></a><a name="p99845386429"></a>创建NAT网关</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p6984138104220"><a name="p6984138104220"></a><a name="p6984138104220"></a>nat:natGateways:create</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul5542718184316"></a><a name="ul5542718184316"></a><ul id="ul5542718184316"><li>支持：<p id="p121955518441"><a name="p121955518441"></a><a name="p121955518441"></a>项目 （Project）</p>
</li><li>不支持：<p id="p10579581448"><a name="p10579581448"></a><a name="p10579581448"></a>企业项目（Enterprise Project）</p>
</li></ul>
</td>
</tr>
<tr id="row959782416351"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p9728202354219"><a name="p9728202354219"></a><a name="p9728202354219"></a>GET /v2.0/nat_gateways</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p3984173819420"><a name="p3984173819420"></a><a name="p3984173819420"></a>查询NAT网关列表</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p1984938134215"><a name="p1984938134215"></a><a name="p1984938134215"></a>nat:natGateways:list</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul11656614204411"></a><a name="ul11656614204411"></a><ul id="ul11656614204411"><li>支持：<p id="p1565681418444"><a name="p1565681418444"></a><a name="p1565681418444"></a>项目 （Project）</p>
</li><li>不支持：<p id="p1765631464410"><a name="p1765631464410"></a><a name="p1765631464410"></a>企业项目（Enterprise Project）</p>
</li></ul>
</td>
</tr>
<tr id="row459717246353"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p7728123134218"><a name="p7728123134218"></a><a name="p7728123134218"></a>GET /v2.0/nat_gateways/{nat_gateway_id}</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p5984938194212"><a name="p5984938194212"></a><a name="p5984938194212"></a>查询NAT网关详情</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p5984938184220"><a name="p5984938184220"></a><a name="p5984938184220"></a>nat:natGateways:get</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul1566415149446"></a><a name="ul1566415149446"></a><ul id="ul1566415149446"><li>支持：<p id="p19664181418443"><a name="p19664181418443"></a><a name="p19664181418443"></a>项目 （Project）</p>
</li><li>不支持：<p id="p1566417148444"><a name="p1566417148444"></a><a name="p1566417148444"></a>企业项目（Enterprise Project）</p>
</li></ul>
</td>
</tr>
<tr id="row1159792493517"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p0728122304213"><a name="p0728122304213"></a><a name="p0728122304213"></a>PUT /v2.0/nat_gateways/{nat_gateway_id}</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p16984123820424"><a name="p16984123820424"></a><a name="p16984123820424"></a>更新NAT网关</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p0984163810422"><a name="p0984163810422"></a><a name="p0984163810422"></a>nat:natGateways:update</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul7672614104412"></a><a name="ul7672614104412"></a><ul id="ul7672614104412"><li>支持：<p id="p1767120145443"><a name="p1767120145443"></a><a name="p1767120145443"></a>项目 （Project）</p>
</li><li>不支持：<p id="p567231474414"><a name="p567231474414"></a><a name="p567231474414"></a>企业项目（Enterprise Project）</p>
</li></ul>
</td>
</tr>
<tr id="row85979249353"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p1872962320422"><a name="p1872962320422"></a><a name="p1872962320422"></a>DELETE /v2.0/nat_gateways/{nat_gateway_id}</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p1598453824219"><a name="p1598453824219"></a><a name="p1598453824219"></a>删除NAT网关</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p89843387426"><a name="p89843387426"></a><a name="p89843387426"></a>nat:natGateways:delete</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul0677201494413"></a><a name="ul0677201494413"></a><ul id="ul0677201494413"><li>支持：<p id="p5677111416443"><a name="p5677111416443"></a><a name="p5677111416443"></a>项目 （Project）</p>
</li><li>不支持：<p id="p4677614174414"><a name="p4677614174414"></a><a name="p4677614174414"></a>企业项目（Enterprise Project）</p>
</li></ul>
</td>
</tr>
</tbody>
</table>

