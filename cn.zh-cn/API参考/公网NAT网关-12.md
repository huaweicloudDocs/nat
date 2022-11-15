# 公网NAT网关<a name="nat_api_0029"></a>

<a name="table1351682493510"></a>
<table><thead align="left"><tr id="row1759512463518"><th class="cellrowborder" valign="top" width="14.64853514648535%" id="mcps1.1.6.1.1"><p id="p6174435204812"><a name="p6174435204812"></a><a name="p6174435204812"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="36.61633836616339%" id="mcps1.1.6.1.2"><p id="p8174113504816"><a name="p8174113504816"></a><a name="p8174113504816"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="19.08809119088091%" id="mcps1.1.6.1.3"><p id="p8701346133717"><a name="p8701346133717"></a><a name="p8701346133717"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="13.558644135586443%" id="mcps1.1.6.1.4"><p id="p5985736163016"><a name="p5985736163016"></a><a name="p5985736163016"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="16.088391160883912%" id="mcps1.1.6.1.5"><p id="p8985133619300"><a name="p8985133619300"></a><a name="p8985133619300"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="row15595192412355"><td class="cellrowborder" valign="top" width="14.64853514648535%" headers="mcps1.1.6.1.1 "><p id="p193521881492"><a name="p193521881492"></a><a name="p193521881492"></a>创建公网NAT网关</p>
</td>
<td class="cellrowborder" valign="top" width="36.61633836616339%" headers="mcps1.1.6.1.2 "><p id="p11421836144718"><a name="p11421836144718"></a><a name="p11421836144718"></a>POST /v2/{project_id}/nat_gateways</p>
</td>
<td class="cellrowborder" valign="top" width="19.08809119088091%" headers="mcps1.1.6.1.3 "><p id="p163527824914"><a name="p163527824914"></a><a name="p163527824914"></a>nat:natGateways:create</p>
</td>
<td class="cellrowborder" valign="top" width="13.558644135586443%" headers="mcps1.1.6.1.4 "><p id="p15756115919276"><a name="p15756115919276"></a><a name="p15756115919276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="16.088391160883912%" headers="mcps1.1.6.1.5 "><p id="p193691154133112"><a name="p193691154133112"></a><a name="p193691154133112"></a>√</p>
</td>
</tr>
<tr id="row959782416351"><td class="cellrowborder" valign="top" width="14.64853514648535%" headers="mcps1.1.6.1.1 "><p id="p1435268194916"><a name="p1435268194916"></a><a name="p1435268194916"></a>查询公网NAT网关列表</p>
</td>
<td class="cellrowborder" valign="top" width="36.61633836616339%" headers="mcps1.1.6.1.2 "><p id="p2421153674717"><a name="p2421153674717"></a><a name="p2421153674717"></a>GET /v2/{project_id}/nat_gateways</p>
</td>
<td class="cellrowborder" valign="top" width="19.08809119088091%" headers="mcps1.1.6.1.3 "><p id="p1635298114910"><a name="p1635298114910"></a><a name="p1635298114910"></a>nat:natGateways:list</p>
</td>
<td class="cellrowborder" valign="top" width="13.558644135586443%" headers="mcps1.1.6.1.4 "><p id="p1475655902719"><a name="p1475655902719"></a><a name="p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="16.088391160883912%" headers="mcps1.1.6.1.5 "><p id="p153706545313"><a name="p153706545313"></a><a name="p153706545313"></a>√</p>
</td>
</tr>
<tr id="row459717246353"><td class="cellrowborder" valign="top" width="14.64853514648535%" headers="mcps1.1.6.1.1 "><p id="p1235216864917"><a name="p1235216864917"></a><a name="p1235216864917"></a>查询公网NAT网关详情</p>
</td>
<td class="cellrowborder" valign="top" width="36.61633836616339%" headers="mcps1.1.6.1.2 "><p id="p1942117368475"><a name="p1942117368475"></a><a name="p1942117368475"></a>GET /v2/{project_id}/nat_gateways/{nat_gateway_id}</p>
</td>
<td class="cellrowborder" valign="top" width="19.08809119088091%" headers="mcps1.1.6.1.3 "><p id="p735214824916"><a name="p735214824916"></a><a name="p735214824916"></a>nat:natGateways:get</p>
</td>
<td class="cellrowborder" valign="top" width="13.558644135586443%" headers="mcps1.1.6.1.4 "><p id="p167561459142711"><a name="p167561459142711"></a><a name="p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="16.088391160883912%" headers="mcps1.1.6.1.5 "><p id="p1370175418319"><a name="p1370175418319"></a><a name="p1370175418319"></a>√</p>
</td>
</tr>
<tr id="row1159792493517"><td class="cellrowborder" valign="top" width="14.64853514648535%" headers="mcps1.1.6.1.1 "><p id="p23521985496"><a name="p23521985496"></a><a name="p23521985496"></a>更新公网NAT网关</p>
</td>
<td class="cellrowborder" valign="top" width="36.61633836616339%" headers="mcps1.1.6.1.2 "><p id="p144211236114712"><a name="p144211236114712"></a><a name="p144211236114712"></a>PUT /v2/{project_id}/nat_gateways/{nat_gateway_id}</p>
</td>
<td class="cellrowborder" valign="top" width="19.08809119088091%" headers="mcps1.1.6.1.3 "><p id="p1535219874915"><a name="p1535219874915"></a><a name="p1535219874915"></a>nat:natGateways:update</p>
</td>
<td class="cellrowborder" valign="top" width="13.558644135586443%" headers="mcps1.1.6.1.4 "><p id="p9757145912271"><a name="p9757145912271"></a><a name="p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="16.088391160883912%" headers="mcps1.1.6.1.5 "><p id="p19370155411318"><a name="p19370155411318"></a><a name="p19370155411318"></a>√</p>
</td>
</tr>
<tr id="row85979249353"><td class="cellrowborder" valign="top" width="14.64853514648535%" headers="mcps1.1.6.1.1 "><p id="p1335228124918"><a name="p1335228124918"></a><a name="p1335228124918"></a>删除公网NAT网关</p>
</td>
<td class="cellrowborder" valign="top" width="36.61633836616339%" headers="mcps1.1.6.1.2 "><p id="p154211236104714"><a name="p154211236104714"></a><a name="p154211236104714"></a>DELETE /v2/{project_id}/nat_gateways/{nat_gateway_id}</p>
</td>
<td class="cellrowborder" valign="top" width="19.08809119088091%" headers="mcps1.1.6.1.3 "><p id="p6352887494"><a name="p6352887494"></a><a name="p6352887494"></a>nat:natGateways:delete</p>
</td>
<td class="cellrowborder" valign="top" width="13.558644135586443%" headers="mcps1.1.6.1.4 "><p id="p187577594276"><a name="p187577594276"></a><a name="p187577594276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="16.088391160883912%" headers="mcps1.1.6.1.5 "><p id="p10370105493116"><a name="p10370105493116"></a><a name="p10370105493116"></a>√</p>
</td>
</tr>
</tbody>
</table>

