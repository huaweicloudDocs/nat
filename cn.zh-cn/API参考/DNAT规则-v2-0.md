# DNAT规则 v2.0<a name="nat_api_0034"></a>

<a name="table1351682493510"></a>
<table><thead align="left"><tr id="row1759512463518"><th class="cellrowborder" valign="top" width="15.688431156884308%" id="mcps1.1.6.1.1"><p id="p6174435204812"><a name="p6174435204812"></a><a name="p6174435204812"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="29.547045295470447%" id="mcps1.1.6.1.2"><p id="p8174113504816"><a name="p8174113504816"></a><a name="p8174113504816"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="15.808419158084186%" id="mcps1.1.6.1.3"><p id="p8701346133717"><a name="p8701346133717"></a><a name="p8701346133717"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="20.707929207079285%" id="mcps1.1.6.1.4"><p id="p5985736163016"><a name="p5985736163016"></a><a name="p5985736163016"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="18.248175182481745%" id="mcps1.1.6.1.5"><p id="p8985133619300"><a name="p8985133619300"></a><a name="p8985133619300"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="row15595192412355"><td class="cellrowborder" valign="top" width="15.688431156884308%" headers="mcps1.1.6.1.1 "><p id="p9809687533"><a name="p9809687533"></a><a name="p9809687533"></a>创建DNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="29.547045295470447%" headers="mcps1.1.6.1.2 "><p id="p172561417115312"><a name="p172561417115312"></a><a name="p172561417115312"></a>POST /v2.0/dnat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="15.808419158084186%" headers="mcps1.1.6.1.3 "><p id="p98091989538"><a name="p98091989538"></a><a name="p98091989538"></a>nat:dnatRules:create</p>
</td>
<td class="cellrowborder" valign="top" width="20.707929207079285%" headers="mcps1.1.6.1.4 "><p id="p15756115919276"><a name="p15756115919276"></a><a name="p15756115919276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.248175182481745%" headers="mcps1.1.6.1.5 "><p id="p54871102411"><a name="p54871102411"></a><a name="p54871102411"></a>×</p>
</td>
</tr>
<tr id="row959782416351"><td class="cellrowborder" valign="top" width="15.688431156884308%" headers="mcps1.1.6.1.1 "><p id="p1880938125310"><a name="p1880938125310"></a><a name="p1880938125310"></a>查询DNAT规则列表</p>
</td>
<td class="cellrowborder" valign="top" width="29.547045295470447%" headers="mcps1.1.6.1.2 "><p id="p12256517165318"><a name="p12256517165318"></a><a name="p12256517165318"></a>GET /v2.0/dnat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="15.808419158084186%" headers="mcps1.1.6.1.3 "><p id="p1380958145313"><a name="p1380958145313"></a><a name="p1380958145313"></a>nat:dnatRules:list</p>
</td>
<td class="cellrowborder" valign="top" width="20.707929207079285%" headers="mcps1.1.6.1.4 "><p id="p1475655902719"><a name="p1475655902719"></a><a name="p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.248175182481745%" headers="mcps1.1.6.1.5 "><p id="p153706545313"><a name="p153706545313"></a><a name="p153706545313"></a>×</p>
</td>
</tr>
<tr id="row459717246353"><td class="cellrowborder" valign="top" width="15.688431156884308%" headers="mcps1.1.6.1.1 "><p id="p58091683536"><a name="p58091683536"></a><a name="p58091683536"></a>查询DNAT规则详情</p>
</td>
<td class="cellrowborder" valign="top" width="29.547045295470447%" headers="mcps1.1.6.1.2 "><p id="p1925641775311"><a name="p1925641775311"></a><a name="p1925641775311"></a>GET /v2.0/dnat_rules/{dnat_rule_id }</p>
</td>
<td class="cellrowborder" valign="top" width="15.808419158084186%" headers="mcps1.1.6.1.3 "><p id="p178090816533"><a name="p178090816533"></a><a name="p178090816533"></a>nat:dnatRules:get</p>
</td>
<td class="cellrowborder" valign="top" width="20.707929207079285%" headers="mcps1.1.6.1.4 "><p id="p167561459142711"><a name="p167561459142711"></a><a name="p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.248175182481745%" headers="mcps1.1.6.1.5 "><p id="p1370175418319"><a name="p1370175418319"></a><a name="p1370175418319"></a>×</p>
</td>
</tr>
<tr id="row1159792493517"><td class="cellrowborder" valign="top" width="15.688431156884308%" headers="mcps1.1.6.1.1 "><p id="p3809286538"><a name="p3809286538"></a><a name="p3809286538"></a>删除DNAT规则</p>
</td>
<td class="cellrowborder" valign="top" width="29.547045295470447%" headers="mcps1.1.6.1.2 "><p id="p1725610177530"><a name="p1725610177530"></a><a name="p1725610177530"></a>DELETE /v2.0/dnat_rules/{dnat_rule_id}</p>
</td>
<td class="cellrowborder" valign="top" width="15.808419158084186%" headers="mcps1.1.6.1.3 "><p id="p128091082532"><a name="p128091082532"></a><a name="p128091082532"></a>nat:dnat_rules:delete</p>
</td>
<td class="cellrowborder" valign="top" width="20.707929207079285%" headers="mcps1.1.6.1.4 "><p id="p9757145912271"><a name="p9757145912271"></a><a name="p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.248175182481745%" headers="mcps1.1.6.1.5 "><p id="p19370155411318"><a name="p19370155411318"></a><a name="p19370155411318"></a>×</p>
</td>
</tr>
</tbody>
</table>

