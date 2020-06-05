# NAT网关 v2.0<a name="nat_api_0032"></a>

<a name="table1351682493510"></a>
<table><thead align="left"><tr id="row1759512463518"><th class="cellrowborder" valign="top" width="17.41%" id="mcps1.1.6.1.1"><p id="p6174435204812"><a name="p6174435204812"></a><a name="p6174435204812"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="26.229999999999997%" id="mcps1.1.6.1.2"><p id="p8174113504816"><a name="p8174113504816"></a><a name="p8174113504816"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="24.62%" id="mcps1.1.6.1.3"><p id="p8701346133717"><a name="p8701346133717"></a><a name="p8701346133717"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="17.53%" id="mcps1.1.6.1.4"><p id="p5985736163016"><a name="p5985736163016"></a><a name="p5985736163016"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="14.21%" id="mcps1.1.6.1.5"><p id="p8985133619300"><a name="p8985133619300"></a><a name="p8985133619300"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="row15595192412355"><td class="cellrowborder" valign="top" width="17.41%" headers="mcps1.1.6.1.1 "><p id="p99845386429"><a name="p99845386429"></a><a name="p99845386429"></a>创建NAT网关</p>
</td>
<td class="cellrowborder" valign="top" width="26.229999999999997%" headers="mcps1.1.6.1.2 "><p id="p872832315425"><a name="p872832315425"></a><a name="p872832315425"></a>POST /v2.0/nat_gateways</p>
</td>
<td class="cellrowborder" valign="top" width="24.62%" headers="mcps1.1.6.1.3 "><p id="p6984138104220"><a name="p6984138104220"></a><a name="p6984138104220"></a>nat:natGateways:create</p>
</td>
<td class="cellrowborder" valign="top" width="17.53%" headers="mcps1.1.6.1.4 "><p id="p15756115919276"><a name="p15756115919276"></a><a name="p15756115919276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="14.21%" headers="mcps1.1.6.1.5 "><p id="p54871102411"><a name="p54871102411"></a><a name="p54871102411"></a>×</p>
</td>
</tr>
<tr id="row959782416351"><td class="cellrowborder" valign="top" width="17.41%" headers="mcps1.1.6.1.1 "><p id="p3984173819420"><a name="p3984173819420"></a><a name="p3984173819420"></a>查询NAT网关列表</p>
</td>
<td class="cellrowborder" valign="top" width="26.229999999999997%" headers="mcps1.1.6.1.2 "><p id="p9728202354219"><a name="p9728202354219"></a><a name="p9728202354219"></a>GET /v2.0/nat_gateways</p>
</td>
<td class="cellrowborder" valign="top" width="24.62%" headers="mcps1.1.6.1.3 "><p id="p1984938134215"><a name="p1984938134215"></a><a name="p1984938134215"></a>nat:natGateways:list</p>
</td>
<td class="cellrowborder" valign="top" width="17.53%" headers="mcps1.1.6.1.4 "><p id="p1475655902719"><a name="p1475655902719"></a><a name="p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="14.21%" headers="mcps1.1.6.1.5 "><p id="p153706545313"><a name="p153706545313"></a><a name="p153706545313"></a>×</p>
</td>
</tr>
<tr id="row459717246353"><td class="cellrowborder" valign="top" width="17.41%" headers="mcps1.1.6.1.1 "><p id="p5984938194212"><a name="p5984938194212"></a><a name="p5984938194212"></a>查询NAT网关详情</p>
</td>
<td class="cellrowborder" valign="top" width="26.229999999999997%" headers="mcps1.1.6.1.2 "><p id="p7728123134218"><a name="p7728123134218"></a><a name="p7728123134218"></a>GET /v2.0/nat_gateways/{nat_gateway_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24.62%" headers="mcps1.1.6.1.3 "><p id="p5984938184220"><a name="p5984938184220"></a><a name="p5984938184220"></a>nat:natGateways:get</p>
</td>
<td class="cellrowborder" valign="top" width="17.53%" headers="mcps1.1.6.1.4 "><p id="p167561459142711"><a name="p167561459142711"></a><a name="p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="14.21%" headers="mcps1.1.6.1.5 "><p id="p1370175418319"><a name="p1370175418319"></a><a name="p1370175418319"></a>×</p>
</td>
</tr>
<tr id="row1159792493517"><td class="cellrowborder" valign="top" width="17.41%" headers="mcps1.1.6.1.1 "><p id="p16984123820424"><a name="p16984123820424"></a><a name="p16984123820424"></a>更新NAT网关</p>
</td>
<td class="cellrowborder" valign="top" width="26.229999999999997%" headers="mcps1.1.6.1.2 "><p id="p0728122304213"><a name="p0728122304213"></a><a name="p0728122304213"></a>PUT /v2.0/nat_gateways/{nat_gateway_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24.62%" headers="mcps1.1.6.1.3 "><p id="p0984163810422"><a name="p0984163810422"></a><a name="p0984163810422"></a>nat:natGateways:update</p>
</td>
<td class="cellrowborder" valign="top" width="17.53%" headers="mcps1.1.6.1.4 "><p id="p9757145912271"><a name="p9757145912271"></a><a name="p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="14.21%" headers="mcps1.1.6.1.5 "><p id="p19370155411318"><a name="p19370155411318"></a><a name="p19370155411318"></a>×</p>
</td>
</tr>
<tr id="row85979249353"><td class="cellrowborder" valign="top" width="17.41%" headers="mcps1.1.6.1.1 "><p id="p1598453824219"><a name="p1598453824219"></a><a name="p1598453824219"></a>删除NAT网关</p>
</td>
<td class="cellrowborder" valign="top" width="26.229999999999997%" headers="mcps1.1.6.1.2 "><p id="p1872962320422"><a name="p1872962320422"></a><a name="p1872962320422"></a>DELETE /v2.0/nat_gateways/{nat_gateway_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24.62%" headers="mcps1.1.6.1.3 "><p id="p89843387426"><a name="p89843387426"></a><a name="p89843387426"></a>nat:natGateways:delete</p>
</td>
<td class="cellrowborder" valign="top" width="17.53%" headers="mcps1.1.6.1.4 "><p id="p187577594276"><a name="p187577594276"></a><a name="p187577594276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="14.21%" headers="mcps1.1.6.1.5 "><p id="p190572017235"><a name="p190572017235"></a><a name="p190572017235"></a>×</p>
</td>
</tr>
</tbody>
</table>

