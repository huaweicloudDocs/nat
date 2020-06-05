# 创建NAT网关<a name="nat_apiv2_0005"></a>

## 功能介绍<a name="zh-cn_topic_0168797238_section19627306"></a>

创建NAT网关实例。

## URI<a name="zh-cn_topic_0168797238_section79426345357"></a>

POST /v2/\{project\_id\}/nat\_gateways

**表 1**  参数说明

<a name="zh-cn_topic_0168797238_table11383184310134"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797238_row1538394311134"><th class="cellrowborder" valign="top" width="22.869999999999997%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797238_p923129131416"><a name="zh-cn_topic_0168797238_p923129131416"></a><a name="zh-cn_topic_0168797238_p923129131416"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.34%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797238_p16231189101416"><a name="zh-cn_topic_0168797238_p16231189101416"></a><a name="zh-cn_topic_0168797238_p16231189101416"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.600000000000001%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797238_p15732422123112"><a name="zh-cn_topic_0168797238_p15732422123112"></a><a name="zh-cn_topic_0168797238_p15732422123112"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50.19%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797238_p5231139141414"><a name="zh-cn_topic_0168797238_p5231139141414"></a><a name="zh-cn_topic_0168797238_p5231139141414"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797238_row63834431139"><td class="cellrowborder" valign="top" width="22.869999999999997%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797238_p172314916147"><a name="zh-cn_topic_0168797238_p172314916147"></a><a name="zh-cn_topic_0168797238_p172314916147"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.34%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797238_p223112915144"><a name="zh-cn_topic_0168797238_p223112915144"></a><a name="zh-cn_topic_0168797238_p223112915144"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.600000000000001%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797238_p1173352212317"><a name="zh-cn_topic_0168797238_p1173352212317"></a><a name="zh-cn_topic_0168797238_p1173352212317"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.19%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797238_p1123115971410"><a name="zh-cn_topic_0168797238_p1123115971410"></a><a name="zh-cn_topic_0168797238_p1123115971410"></a>项目ID。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0168797238_section14118316"></a>

请求参数如[表2](#zh-cn_topic_0168797238_table531642713017)所示。

**表 2**  请求参数

<a name="zh-cn_topic_0168797238_table531642713017"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797238_row15519227163019"><th class="cellrowborder" valign="top" width="22.939999999999998%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797238_p1519927183015"><a name="zh-cn_topic_0168797238_p1519927183015"></a><a name="zh-cn_topic_0168797238_p1519927183015"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="14.04%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797238_p123411127103717"><a name="zh-cn_topic_0168797238_p123411127103717"></a><a name="zh-cn_topic_0168797238_p123411127103717"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.959999999999999%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797238_p622735214373"><a name="zh-cn_topic_0168797238_p622735214373"></a><a name="zh-cn_topic_0168797238_p622735214373"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50.06%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797238_p10519027113020"><a name="zh-cn_topic_0168797238_p10519027113020"></a><a name="zh-cn_topic_0168797238_p10519027113020"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797238_row12519162773014"><td class="cellrowborder" valign="top" width="22.939999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797238_p19519182710304"><a name="zh-cn_topic_0168797238_p19519182710304"></a><a name="zh-cn_topic_0168797238_p19519182710304"></a>nat_gateway</p>
</td>
<td class="cellrowborder" valign="top" width="14.04%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797238_p83412273376"><a name="zh-cn_topic_0168797238_p83412273376"></a><a name="zh-cn_topic_0168797238_p83412273376"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.959999999999999%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797238_p202276528373"><a name="zh-cn_topic_0168797238_p202276528373"></a><a name="zh-cn_topic_0168797238_p202276528373"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="50.06%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797238_p15519192743011"><a name="zh-cn_topic_0168797238_p15519192743011"></a><a name="zh-cn_topic_0168797238_p15519192743011"></a>NAT网关对象。请参考<a href="#zh-cn_topic_0168797238_table93481227153014">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  nat\_gateway字段说明

<a name="zh-cn_topic_0168797238_table93481227153014"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797238_row1051916278301"><th class="cellrowborder" valign="top" width="22.939999999999998%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797238_p10519132723015"><a name="zh-cn_topic_0168797238_p10519132723015"></a><a name="zh-cn_topic_0168797238_p10519132723015"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.69%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797238_p95191427163010"><a name="zh-cn_topic_0168797238_p95191427163010"></a><a name="zh-cn_topic_0168797238_p95191427163010"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.309999999999999%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797238_p195191927133019"><a name="zh-cn_topic_0168797238_p195191927133019"></a><a name="zh-cn_topic_0168797238_p195191927133019"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50.06%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797238_p85191127143015"><a name="zh-cn_topic_0168797238_p85191127143015"></a><a name="zh-cn_topic_0168797238_p85191127143015"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797238_row13519162717309"><td class="cellrowborder" valign="top" width="22.939999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797238_p8519142717306"><a name="zh-cn_topic_0168797238_p8519142717306"></a><a name="zh-cn_topic_0168797238_p8519142717306"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.69%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797238_p1519427203019"><a name="zh-cn_topic_0168797238_p1519427203019"></a><a name="zh-cn_topic_0168797238_p1519427203019"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.309999999999999%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797238_p7519227183020"><a name="zh-cn_topic_0168797238_p7519227183020"></a><a name="zh-cn_topic_0168797238_p7519227183020"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.06%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797238_p16519162711308"><a name="zh-cn_topic_0168797238_p16519162711308"></a><a name="zh-cn_topic_0168797238_p16519162711308"></a>项目的ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797238_row0519192793015"><td class="cellrowborder" valign="top" width="22.939999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797238_p8519142711302"><a name="zh-cn_topic_0168797238_p8519142711302"></a><a name="zh-cn_topic_0168797238_p8519142711302"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.69%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797238_p1151962733014"><a name="zh-cn_topic_0168797238_p1151962733014"></a><a name="zh-cn_topic_0168797238_p1151962733014"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.309999999999999%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797238_p13519112753013"><a name="zh-cn_topic_0168797238_p13519112753013"></a><a name="zh-cn_topic_0168797238_p13519112753013"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="50.06%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797238_p12519327113012"><a name="zh-cn_topic_0168797238_p12519327113012"></a><a name="zh-cn_topic_0168797238_p12519327113012"></a>NAT网关的名字。</p>
<p id="zh-cn_topic_0168797238_p15519227143015"><a name="zh-cn_topic_0168797238_p15519227143015"></a><a name="zh-cn_topic_0168797238_p15519227143015"></a>NAT网关的名字仅支持数字、字母、_（下划线）、-（中划线）、中文。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797238_row1651920271306"><td class="cellrowborder" valign="top" width="22.939999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797238_p65191327153018"><a name="zh-cn_topic_0168797238_p65191327153018"></a><a name="zh-cn_topic_0168797238_p65191327153018"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13.69%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797238_p5519122733012"><a name="zh-cn_topic_0168797238_p5519122733012"></a><a name="zh-cn_topic_0168797238_p5519122733012"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.309999999999999%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797238_p125191227203016"><a name="zh-cn_topic_0168797238_p125191227203016"></a><a name="zh-cn_topic_0168797238_p125191227203016"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="50.06%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797238_p6519152719306"><a name="zh-cn_topic_0168797238_p6519152719306"></a><a name="zh-cn_topic_0168797238_p6519152719306"></a>NAT网关的描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797238_row95191027143013"><td class="cellrowborder" valign="top" width="22.939999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797238_p95190271307"><a name="zh-cn_topic_0168797238_p95190271307"></a><a name="zh-cn_topic_0168797238_p95190271307"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="13.69%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797238_p195191927143014"><a name="zh-cn_topic_0168797238_p195191927143014"></a><a name="zh-cn_topic_0168797238_p195191927143014"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.309999999999999%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797238_p1859312144498"><a name="zh-cn_topic_0168797238_p1859312144498"></a><a name="zh-cn_topic_0168797238_p1859312144498"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.06%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797238_p251962719307"><a name="zh-cn_topic_0168797238_p251962719307"></a><a name="zh-cn_topic_0168797238_p251962719307"></a>NAT网关的规格。</p>
<p id="zh-cn_topic_0168797238_p15191327183013"><a name="zh-cn_topic_0168797238_p15191327183013"></a><a name="zh-cn_topic_0168797238_p15191327183013"></a>取值为：</p>
<a name="zh-cn_topic_0168797238_ul151911279307"></a><a name="zh-cn_topic_0168797238_ul151911279307"></a><ul id="zh-cn_topic_0168797238_ul151911279307"><li>“1”：小型，SNAT最大连接数10000</li><li>“2”：中型，SNAT最大连接数50000</li><li>“3”：大型，SNAT最大连接数200000</li><li>“4”：超大型，SNAT最大连接数1000000</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797238_row35192277306"><td class="cellrowborder" valign="top" width="22.939999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797238_p55191827103018"><a name="zh-cn_topic_0168797238_p55191827103018"></a><a name="zh-cn_topic_0168797238_p55191827103018"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.69%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797238_p1751942763015"><a name="zh-cn_topic_0168797238_p1751942763015"></a><a name="zh-cn_topic_0168797238_p1751942763015"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.309999999999999%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797238_p19519152720308"><a name="zh-cn_topic_0168797238_p19519152720308"></a><a name="zh-cn_topic_0168797238_p19519152720308"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.06%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797238_p151972713301"><a name="zh-cn_topic_0168797238_p151972713301"></a><a name="zh-cn_topic_0168797238_p151972713301"></a>VPC的id。获取 router_id 的方法请参考<a href="https://support.huaweicloud.com/api-vpc/vpc_route_0001.html" target="_blank" rel="noopener noreferrer">查询VPC路由列表</a>下的vpc_id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797238_row10519172753011"><td class="cellrowborder" valign="top" width="22.939999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797238_p45191127163011"><a name="zh-cn_topic_0168797238_p45191127163011"></a><a name="zh-cn_topic_0168797238_p45191127163011"></a>internal_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.69%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797238_p1051910279307"><a name="zh-cn_topic_0168797238_p1051910279307"></a><a name="zh-cn_topic_0168797238_p1051910279307"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.309999999999999%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797238_p85191527133017"><a name="zh-cn_topic_0168797238_p85191527133017"></a><a name="zh-cn_topic_0168797238_p85191527133017"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.06%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797238_p751917272301"><a name="zh-cn_topic_0168797238_p751917272301"></a><a name="zh-cn_topic_0168797238_p751917272301"></a>NAT网关下行口（DVR的下一跳）所属的network id。获取 network id 的方法请参考<a href="https://support.huaweicloud.com/api-vpc/vpc_subnet01_0003.html" target="_blank" rel="noopener noreferrer">查询子网列表</a>下的neutron_network_id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797238_row641351331917"><td class="cellrowborder" valign="top" width="22.939999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797238_p119337283196"><a name="zh-cn_topic_0168797238_p119337283196"></a><a name="zh-cn_topic_0168797238_p119337283196"></a>enterprise_project_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.69%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797238_p8933828161920"><a name="zh-cn_topic_0168797238_p8933828161920"></a><a name="zh-cn_topic_0168797238_p8933828161920"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.309999999999999%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797238_p193392815191"><a name="zh-cn_topic_0168797238_p193392815191"></a><a name="zh-cn_topic_0168797238_p193392815191"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.06%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0168797238_ul16934128181916"></a><a name="zh-cn_topic_0168797238_ul16934128181916"></a><ul id="zh-cn_topic_0168797238_ul16934128181916"><li>功能说明：企业项目ID。创建NAT网关时，给NAT网关绑定企业项目 ID。默认值：0，表示默认企业项目。</li><li>取值范围：最大长度36字节，带 “-”连字符的UUID格式，或者是字符串“0”。</li><li>说明：关于企业项目ID的获取及企业项目特性的详细信息，请参考<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0123692049.html" target="_blank" rel="noopener noreferrer">《企业管理用户指南》</a>。</li></ul>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="zh-cn_topic_0168797238_section59955987"></a>

响应参数如[表4](#zh-cn_topic_0168797238_table1899835483516)所示。

**表 4**  响应参数

<a name="zh-cn_topic_0168797238_table1899835483516"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797238_row7169955173518"><th class="cellrowborder" valign="top" width="22.759999999999998%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797238_p17169195519358"><a name="zh-cn_topic_0168797238_p17169195519358"></a><a name="zh-cn_topic_0168797238_p17169195519358"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.92%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797238_p5169105593518"><a name="zh-cn_topic_0168797238_p5169105593518"></a><a name="zh-cn_topic_0168797238_p5169105593518"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.32000000000001%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797238_p2169855193514"><a name="zh-cn_topic_0168797238_p2169855193514"></a><a name="zh-cn_topic_0168797238_p2169855193514"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797238_row316945543510"><td class="cellrowborder" valign="top" width="22.759999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797238_p161697551351"><a name="zh-cn_topic_0168797238_p161697551351"></a><a name="zh-cn_topic_0168797238_p161697551351"></a>nat_gateway</p>
</td>
<td class="cellrowborder" valign="top" width="18.92%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797238_p716916553359"><a name="zh-cn_topic_0168797238_p716916553359"></a><a name="zh-cn_topic_0168797238_p716916553359"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="58.32000000000001%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797238_p141693558351"><a name="zh-cn_topic_0168797238_p141693558351"></a><a name="zh-cn_topic_0168797238_p141693558351"></a>nat_gateway对象。请参考<a href="#zh-cn_topic_0168797238_table5998115418352">表5</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 5**  nat\_gateway字段说明

<a name="zh-cn_topic_0168797238_table5998115418352"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797238_row6169455113517"><th class="cellrowborder" valign="top" width="23.23%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797238_p18169125533511"><a name="zh-cn_topic_0168797238_p18169125533511"></a><a name="zh-cn_topic_0168797238_p18169125533511"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797238_p11692559359"><a name="zh-cn_topic_0168797238_p11692559359"></a><a name="zh-cn_topic_0168797238_p11692559359"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.589999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797238_p15169165515355"><a name="zh-cn_topic_0168797238_p15169165515355"></a><a name="zh-cn_topic_0168797238_p15169165515355"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797238_row16169555143516"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797238_p131697559351"><a name="zh-cn_topic_0168797238_p131697559351"></a><a name="zh-cn_topic_0168797238_p131697559351"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797238_p11169115553519"><a name="zh-cn_topic_0168797238_p11169115553519"></a><a name="zh-cn_topic_0168797238_p11169115553519"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797238_p16169195593517"><a name="zh-cn_topic_0168797238_p16169195593517"></a><a name="zh-cn_topic_0168797238_p16169195593517"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797238_row5169755193513"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797238_p141694552355"><a name="zh-cn_topic_0168797238_p141694552355"></a><a name="zh-cn_topic_0168797238_p141694552355"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797238_p816965583515"><a name="zh-cn_topic_0168797238_p816965583515"></a><a name="zh-cn_topic_0168797238_p816965583515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797238_p201693557359"><a name="zh-cn_topic_0168797238_p201693557359"></a><a name="zh-cn_topic_0168797238_p201693557359"></a>项目的ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797238_row91691755183512"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797238_p16169555143511"><a name="zh-cn_topic_0168797238_p16169555143511"></a><a name="zh-cn_topic_0168797238_p16169555143511"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797238_p14169155513358"><a name="zh-cn_topic_0168797238_p14169155513358"></a><a name="zh-cn_topic_0168797238_p14169155513358"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797238_p19169955183517"><a name="zh-cn_topic_0168797238_p19169955183517"></a><a name="zh-cn_topic_0168797238_p19169955183517"></a>NAT网关的名字。</p>
<p id="zh-cn_topic_0168797238_p15169055203514"><a name="zh-cn_topic_0168797238_p15169055203514"></a><a name="zh-cn_topic_0168797238_p15169055203514"></a>NAT网关的名字仅支持数字、字母、_（下划线）、-（中划线）、中文。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797238_row191691855183511"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797238_p1616925533510"><a name="zh-cn_topic_0168797238_p1616925533510"></a><a name="zh-cn_topic_0168797238_p1616925533510"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797238_p111692055193514"><a name="zh-cn_topic_0168797238_p111692055193514"></a><a name="zh-cn_topic_0168797238_p111692055193514"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797238_p181694559355"><a name="zh-cn_topic_0168797238_p181694559355"></a><a name="zh-cn_topic_0168797238_p181694559355"></a>NAT网关的描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797238_row1169655103519"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797238_p2016935510359"><a name="zh-cn_topic_0168797238_p2016935510359"></a><a name="zh-cn_topic_0168797238_p2016935510359"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797238_p1307181918498"><a name="zh-cn_topic_0168797238_p1307181918498"></a><a name="zh-cn_topic_0168797238_p1307181918498"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797238_p1216915518351"><a name="zh-cn_topic_0168797238_p1216915518351"></a><a name="zh-cn_topic_0168797238_p1216915518351"></a>NAT网关的规格。</p>
<p id="zh-cn_topic_0168797238_p19169115553517"><a name="zh-cn_topic_0168797238_p19169115553517"></a><a name="zh-cn_topic_0168797238_p19169115553517"></a>取值为：</p>
<a name="zh-cn_topic_0168797238_ul1216911558358"></a><a name="zh-cn_topic_0168797238_ul1216911558358"></a><ul id="zh-cn_topic_0168797238_ul1216911558358"><li>“1”：小型，SNAT最大连接数10000</li><li>“2”：中型，SNAT最大连接数50000</li><li>“3”：大型，SNAT最大连接数200000</li><li>“4”：超大型，SNAT最大连接数1000000</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797238_row1716985523510"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797238_p1016965563511"><a name="zh-cn_topic_0168797238_p1016965563511"></a><a name="zh-cn_topic_0168797238_p1016965563511"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797238_p1616917554354"><a name="zh-cn_topic_0168797238_p1616917554354"></a><a name="zh-cn_topic_0168797238_p1616917554354"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797238_p15169195517351"><a name="zh-cn_topic_0168797238_p15169195517351"></a><a name="zh-cn_topic_0168797238_p15169195517351"></a>路由器的UUID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797238_row10169355153512"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797238_p17169135563513"><a name="zh-cn_topic_0168797238_p17169135563513"></a><a name="zh-cn_topic_0168797238_p17169135563513"></a>internal_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797238_p10169125533515"><a name="zh-cn_topic_0168797238_p10169125533515"></a><a name="zh-cn_topic_0168797238_p10169125533515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797238_p8169195593518"><a name="zh-cn_topic_0168797238_p8169195593518"></a><a name="zh-cn_topic_0168797238_p8169195593518"></a>NAT网关下行口（DVR的下一跳）所属的network id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797238_row2169755143512"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797238_p121696555354"><a name="zh-cn_topic_0168797238_p121696555354"></a><a name="zh-cn_topic_0168797238_p121696555354"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797238_p171691355173516"><a name="zh-cn_topic_0168797238_p171691355173516"></a><a name="zh-cn_topic_0168797238_p171691355173516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797238_ul5169105563515"></a><a name="zh-cn_topic_0168797238_ul5169105563515"></a><ul id="zh-cn_topic_0168797238_ul5169105563515"><li>功能说明：NAT网关的状态。</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797238_row11169155517351"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797238_p6169755103520"><a name="zh-cn_topic_0168797238_p6169755103520"></a><a name="zh-cn_topic_0168797238_p6169755103520"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797238_p1261933192210"><a name="zh-cn_topic_0168797238_p1261933192210"></a><a name="zh-cn_topic_0168797238_p1261933192210"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797238_ul71858556358"></a><a name="zh-cn_topic_0168797238_ul71858556358"></a><ul id="zh-cn_topic_0168797238_ul71858556358"><li>解冻/冻结状态。</li><li>取值范围：<a name="zh-cn_topic_0168797238_ul11838172814409"></a><a name="zh-cn_topic_0168797238_ul11838172814409"></a><ul id="zh-cn_topic_0168797238_ul11838172814409"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797238_row13185255183510"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797238_p1418525573515"><a name="zh-cn_topic_0168797238_p1418525573515"></a><a name="zh-cn_topic_0168797238_p1418525573515"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797238_p101859557352"><a name="zh-cn_topic_0168797238_p101859557352"></a><a name="zh-cn_topic_0168797238_p101859557352"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797238_p85121028172918"><a name="zh-cn_topic_0168797238_p85121028172918"></a><a name="zh-cn_topic_0168797238_p85121028172918"></a>NAT网关的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797238_row718565553513"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797238_p7185105593510"><a name="zh-cn_topic_0168797238_p7185105593510"></a><a name="zh-cn_topic_0168797238_p7185105593510"></a>dnat_rules_limit</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797238_p81851355143510"><a name="zh-cn_topic_0168797238_p81851355143510"></a><a name="zh-cn_topic_0168797238_p81851355143510"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797238_p108473293292"><a name="zh-cn_topic_0168797238_p108473293292"></a><a name="zh-cn_topic_0168797238_p108473293292"></a>NAT网关的DNAT规则最多条数限制值</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797238_row191851555203514"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797238_p6185145512353"><a name="zh-cn_topic_0168797238_p6185145512353"></a><a name="zh-cn_topic_0168797238_p6185145512353"></a>snat_rule_public_ip_limit</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797238_p1218516552355"><a name="zh-cn_topic_0168797238_p1218516552355"></a><a name="zh-cn_topic_0168797238_p1218516552355"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797238_p317231132913"><a name="zh-cn_topic_0168797238_p317231132913"></a><a name="zh-cn_topic_0168797238_p317231132913"></a>NAT网关的任意一条SNAT规则最多绑定的弹性公网IP的数量最大限制值。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797238_row1810513612314"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797238_p1618344914238"><a name="zh-cn_topic_0168797238_p1618344914238"></a><a name="zh-cn_topic_0168797238_p1618344914238"></a>billing_info</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797238_p5183124922313"><a name="zh-cn_topic_0168797238_p5183124922313"></a><a name="zh-cn_topic_0168797238_p5183124922313"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797238_p1134321153012"><a name="zh-cn_topic_0168797238_p1134321153012"></a><a name="zh-cn_topic_0168797238_p1134321153012"></a>包周期NAT网关订单关联信息，按需值为空字符串。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797238_row166423450506"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797238_p11453195245015"><a name="zh-cn_topic_0168797238_p11453195245015"></a><a name="zh-cn_topic_0168797238_p11453195245015"></a>enterprise_project_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797238_p945345275018"><a name="zh-cn_topic_0168797238_p945345275018"></a><a name="zh-cn_topic_0168797238_p945345275018"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.589999999999996%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797238_ul14453652185018"></a><a name="zh-cn_topic_0168797238_ul14453652185018"></a><ul id="zh-cn_topic_0168797238_ul14453652185018"><li>功能说明：企业项目ID。创建NAT网关时，给NAT网关绑定企业项目 ID。默认值：0，表示默认企业项目。</li><li>取值范围：最大长度36字节，带 “-”连字符的UUID格式，或者是字符串“0”。</li><li>说明：关于企业项目ID的获取及企业项目特性的详细信息，请参考<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0123692049.html" target="_blank" rel="noopener noreferrer">《企业管理用户指南》</a>。</li></ul>
</td>
</tr>
</tbody>
</table>

## 示例<a name="zh-cn_topic_0168797238_section2732972"></a>

-   请求示例

    ```
    POST https://{Endpoint}/v2/27e25061336f4af590faeabeb7fcd9a3/nat_gateways 
    { 
            "nat_gateway": { 
            "name": "nat_001", 
            "description": "my nat gateway 01", 
            "router_id": "d84f345c-80a1-4fa2-a39c-d0d397c3f09a", 
            "internal_network_id": "89d66639-aacb-4929-969d-07080b0f9fd9", 
            "spec": "1",
            "enterprise_project_id": "0aad99bc-f5f6-4f78-8404-c598d76b0ed2"
        } 
    }
    ```


-   响应示例

    ```
    { 
        "nat_gateway": { 
            "router_id": "d84f345c-80a1-4fa2-a39c-d0d397c3f09a", 
            "status": "PENDING_CREATE", 
            "description": "my nat gateway 01", 
            "admin_state_up": true, 
            "tenant_id": "27e25061336f4af590faeabeb7fcd9a3", 
            "created_at": "2017-11-18 07:34:32.203044", 
            "spec": "1", 
            "internal_network_id": "89d66639-aacb-4929-969d-07080b0f9fd9", 
            "id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8", 
            "name": "nat_001",
            "dnat_rules_limit": "200",
            "snat_rule_public_ip_limit": "20",
            "enterprise_project_id"="0aad99bc-f5f6-4f78-8404-c598d76b0ed2",
            "billing_info": ""
        } 
    }
    ```


## 状态码<a name="zh-cn_topic_0168797238_section20044197"></a>

请参考[状态码](状态码.md)。

