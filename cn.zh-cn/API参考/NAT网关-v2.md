# NAT网关 v2<a name="nat_api_0029"></a>

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
<tbody><tr id="row15595192412355"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p11421836144718"><a name="p11421836144718"></a><a name="p11421836144718"></a>POST /v2/{project_id}/nat_gateways</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p193521881492"><a name="p193521881492"></a><a name="p193521881492"></a>创建NAT网关</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p163527824914"><a name="p163527824914"></a><a name="p163527824914"></a>nat:natGateways:create</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul5542718184316"></a><a name="ul5542718184316"></a><ul id="ul5542718184316"><li>支持：<a name="ul85758552477"></a><a name="ul85758552477"></a><ul id="ul85758552477"><li>项目 （Project）</li><li>企业项目（Enterprise Project）</li></ul>
</li><li>不支持：无</li></ul>
</td>
</tr>
<tr id="row959782416351"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p2421153674717"><a name="p2421153674717"></a><a name="p2421153674717"></a>GET /v2/{project_id}/nat_gateways</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p1435268194916"><a name="p1435268194916"></a><a name="p1435268194916"></a>查询NAT网关列表</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p1635298114910"><a name="p1635298114910"></a><a name="p1635298114910"></a>nat:natGateways:list</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul139841920114910"></a><a name="ul139841920114910"></a><ul id="ul139841920114910"><li>支持：<a name="ul7984132054916"></a><a name="ul7984132054916"></a><ul id="ul7984132054916"><li>项目 （Project）</li><li>企业项目（Enterprise Project）</li></ul>
</li><li>不支持：无</li></ul>
</td>
</tr>
<tr id="row459717246353"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p1942117368475"><a name="p1942117368475"></a><a name="p1942117368475"></a>GET /v2/{project_id}/nat_gateways/{nat_gateway_id}</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p1235216864917"><a name="p1235216864917"></a><a name="p1235216864917"></a>查询NAT网关详情</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p735214824916"><a name="p735214824916"></a><a name="p735214824916"></a>nat:natGateways:get</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul1899012201498"></a><a name="ul1899012201498"></a><ul id="ul1899012201498"><li>支持：<a name="ul1599012054911"></a><a name="ul1599012054911"></a><ul id="ul1599012054911"><li>项目 （Project）</li><li>企业项目（Enterprise Project）</li></ul>
</li><li>不支持：无</li></ul>
</td>
</tr>
<tr id="row1159792493517"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p144211236114712"><a name="p144211236114712"></a><a name="p144211236114712"></a>PUT /v2/{project_id}/nat_gateways/{nat_gateway_id}</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p23521985496"><a name="p23521985496"></a><a name="p23521985496"></a>更新NAT网关</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p1535219874915"><a name="p1535219874915"></a><a name="p1535219874915"></a>nat:natGateways:update</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul599742024914"></a><a name="ul599742024914"></a><ul id="ul599742024914"><li>支持：<a name="ul1199782064914"></a><a name="ul1199782064914"></a><ul id="ul1199782064914"><li>项目 （Project）</li><li>企业项目（Enterprise Project）</li></ul>
</li><li>不支持：无</li></ul>
</td>
</tr>
<tr id="row85979249353"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p154211236104714"><a name="p154211236104714"></a><a name="p154211236104714"></a>DELETE /v2/{project_id}/nat_gateways/{nat_gateway_id}</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.1.5.1.2 "><p id="p1335228124918"><a name="p1335228124918"></a><a name="p1335228124918"></a>删除NAT网关</p>
</td>
<td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.1.5.1.3 "><p id="p6352887494"><a name="p6352887494"></a><a name="p6352887494"></a>nat:natGateways:delete</p>
</td>
<td class="cellrowborder" valign="top" width="42.809999999999995%" headers="mcps1.1.5.1.4 "><a name="ul19352114492"></a><a name="ul19352114492"></a><ul id="ul19352114492"><li>支持：<a name="ul4392112492"></a><a name="ul4392112492"></a><ul id="ul4392112492"><li>项目 （Project）</li><li>企业项目（Enterprise Project）</li></ul>
</li><li>不支持：无</li></ul>
</td>
</tr>
</tbody>
</table>

