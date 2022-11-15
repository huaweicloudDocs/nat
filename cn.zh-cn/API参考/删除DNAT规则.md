# 删除DNAT规则<a name="DeleteNatGatewayDnatRule"></a>

## 功能介绍<a name="section12942113142617"></a>

删除指定的DNAT规则。

## 调试<a name="section39470316263"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=nat&api=DeleteNatGatewayDnatRule)中调试该接口。

## URI<a name="section09532031152614"></a>

DELETE /v2/\{project\_id\}/nat\_gateways/\{nat\_gateway\_id\}/dnat\_rules/\{dnat\_rule\_id\}

**表 1**  路径参数

<a name="table1596023192616"></a>
<table><thead align="left"><tr id="row1958631202612"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p17962203114265"><a name="p17962203114265"></a><a name="p17962203114265"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p15964931112611"><a name="p15964931112611"></a><a name="p15964931112611"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p11966031162610"><a name="p11966031162610"></a><a name="p11966031162610"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p59687315265"><a name="p59687315265"></a><a name="p59687315265"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row17958163132613"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p6970183112261"><a name="p6970183112261"></a><a name="p6970183112261"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p897353142619"><a name="p897353142619"></a><a name="p897353142619"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p19758310267"><a name="p19758310267"></a><a name="p19758310267"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p497863114266"><a name="p497863114266"></a><a name="p497863114266"></a>项目的ID。</p>
<p id="p698023182618"><a name="p698023182618"></a><a name="p698023182618"></a>最小长度：<strong id="b10981173114266"><a name="b10981173114266"></a><a name="b10981173114266"></a>1</strong></p>
<p id="p14982153111266"><a name="p14982153111266"></a><a name="p14982153111266"></a>最大长度：<strong id="b3983183162615"><a name="b3983183162615"></a><a name="b3983183162615"></a>36</strong></p>
<p id="p2562026131319"><a name="p2562026131319"></a><a name="p2562026131319"></a>获取方法详见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row6958431172615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p17985173110263"><a name="p17985173110263"></a><a name="p17985173110263"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1698713310267"><a name="p1698713310267"></a><a name="p1698713310267"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p139901131172612"><a name="p139901131172612"></a><a name="p139901131172612"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p799433117260"><a name="p799433117260"></a><a name="p799433117260"></a>公网NAT网关实例的ID。</p>
<p id="p199963311268"><a name="p199963311268"></a><a name="p199963311268"></a>长度：<strong id="b3997163113268"><a name="b3997163113268"></a><a name="b3997163113268"></a>36</strong></p>
</td>
</tr>
<tr id="row6958731132619"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p13073211265"><a name="p13073211265"></a><a name="p13073211265"></a>dnat_rule_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1021732182618"><a name="p1021732182618"></a><a name="p1021732182618"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p17417321265"><a name="p17417321265"></a><a name="p17417321265"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p77132142614"><a name="p77132142614"></a><a name="p77132142614"></a>DNAT规则的ID。</p>
<p id="p2973218261"><a name="p2973218261"></a><a name="p2973218261"></a>长度：<strong id="b1117324263"><a name="b1117324263"></a><a name="b1117324263"></a>36</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section714532122613"></a>

**表 2**  请求Header参数

<a name="zh-cn_topic_0297140337_HeaderParameter"></a>
<table><thead align="left"><tr id="row16161732172610"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p020103217269"><a name="p020103217269"></a><a name="p020103217269"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p6225323265"><a name="p6225323265"></a><a name="p6225323265"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1524832152619"><a name="p1524832152619"></a><a name="p1524832152619"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p62653218268"><a name="p62653218268"></a><a name="p62653218268"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1016203213269"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p12817321264"><a name="p12817321264"></a><a name="p12817321264"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p18301332172610"><a name="p18301332172610"></a><a name="p18301332172610"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p173243213262"><a name="p173243213262"></a><a name="p173243213262"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1536193292618"><a name="p1536193292618"></a><a name="p1536193292618"></a>用户Token。用户Token也就是调用获取用户Token获取请求认证接口的响应值，该接口是唯一不需要认证的接口。请求响应成功后在响应消息头中包含的“X-Subject-Token”的值即为Token值。</p>
<p id="p3379323266"><a name="p3379323266"></a><a name="p3379323266"></a>最小长度：<strong id="b203814324268"><a name="b203814324268"></a><a name="b203814324268"></a>1</strong></p>
<p id="p63903217266"><a name="p63903217266"></a><a name="p63903217266"></a>最大长度：<strong id="b940183252612"><a name="b940183252612"></a><a name="b940183252612"></a>10240</strong></p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section341732172613"></a>

无

## 请求示例<a name="section946103210266"></a>

```
DELETE https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526d/nat_gateways/f4dfea98-874a-46f7-aa2a-fb348d0ceb02/dnat_rules/a78fb3eb-1654-4710-8742-3fc49d5f04f8"

   
```

## 响应示例<a name="section85520328269"></a>

无

## 状态码<a name="section459332102616"></a>

<a name="zh-cn_topic_0297140337_status_code"></a>
<table><thead align="left"><tr id="row106143242610"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p156383242619"><a name="p156383242619"></a><a name="p156383242619"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p1565532132612"><a name="p1565532132612"></a><a name="p1565532132612"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row136216328267"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p7671432192618"><a name="p7671432192618"></a><a name="p7671432192618"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1569133212261"><a name="p1569133212261"></a><a name="p1569133212261"></a>删除DNAT规则成功。</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section4711332102616"></a>

请参见[错误码](错误码.md)。

