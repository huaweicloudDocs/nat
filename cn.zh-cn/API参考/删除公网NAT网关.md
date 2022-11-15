# 删除公网NAT网关<a name="DeleteNatGateway"></a>

## 功能介绍<a name="section161092044617"></a>

删除公网NAT网关实例。

## 调试<a name="section18101220124619"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=nat&api=DeleteNatGateway)中调试该接口。

## URI<a name="section31172013462"></a>

DELETE /v2/\{project\_id\}/nat\_gateways/\{nat\_gateway\_id\}

**表 1**  路径参数

<a name="table18161320104618"></a>
<table><thead align="left"><tr id="row914820104611"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p61732016466"><a name="p61732016466"></a><a name="p61732016466"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p61832024610"><a name="p61832024610"></a><a name="p61832024610"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1518920104617"><a name="p1518920104617"></a><a name="p1518920104617"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p191952012469"><a name="p191952012469"></a><a name="p191952012469"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1415162084610"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p819102034618"><a name="p819102034618"></a><a name="p819102034618"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p9191820184616"><a name="p9191820184616"></a><a name="p9191820184616"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p2201920194617"><a name="p2201920194617"></a><a name="p2201920194617"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p7206202465"><a name="p7206202465"></a><a name="p7206202465"></a>公网NAT网关实例的ID。</p>
<p id="p52117203460"><a name="p52117203460"></a><a name="p52117203460"></a>长度：<strong id="b2211820194617"><a name="b2211820194617"></a><a name="b2211820194617"></a>36</strong></p>
</td>
</tr>
<tr id="row19151920174614"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p72152019462"><a name="p72152019462"></a><a name="p72152019462"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p5221020194611"><a name="p5221020194611"></a><a name="p5221020194611"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p522202094610"><a name="p522202094610"></a><a name="p522202094610"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1223132018464"><a name="p1223132018464"></a><a name="p1223132018464"></a>项目的ID。</p>
<p id="p22352074618"><a name="p22352074618"></a><a name="p22352074618"></a>最小长度：<strong id="b82332054612"><a name="b82332054612"></a><a name="b82332054612"></a>1</strong></p>
<p id="p1223220114611"><a name="p1223220114611"></a><a name="p1223220114611"></a>最大长度：<strong id="b423192064615"><a name="b423192064615"></a><a name="b423192064615"></a>36</strong></p>
<p id="p2562026131319"><a name="p2562026131319"></a><a name="p2562026131319"></a>获取方法详见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section182415206468"></a>

**表 2**  请求Header参数

<a name="zh-cn_topic_0297140325_HeaderParameter"></a>
<table><thead align="left"><tr id="row52552054618"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p5261420174618"><a name="p5261420174618"></a><a name="p5261420174618"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p627102016462"><a name="p627102016462"></a><a name="p627102016462"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p10272020144615"><a name="p10272020144615"></a><a name="p10272020144615"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p6272203462"><a name="p6272203462"></a><a name="p6272203462"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1251220114612"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p3281220124616"><a name="p3281220124616"></a><a name="p3281220124616"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p42972014469"><a name="p42972014469"></a><a name="p42972014469"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p14291207462"><a name="p14291207462"></a><a name="p14291207462"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p23013203462"><a name="p23013203462"></a><a name="p23013203462"></a>用户Token。用户Token也就是调用获取用户Token获取请求认证接口的响应值，该接口是唯一不需要认证的接口。请求响应成功后在响应消息头中包含的“X-Subject-Token”的值即为Token值。</p>
<p id="p1330202094614"><a name="p1330202094614"></a><a name="p1330202094614"></a>最小长度：<strong id="b4301120164618"><a name="b4301120164618"></a><a name="b4301120164618"></a>1</strong></p>
<p id="p430182011462"><a name="p430182011462"></a><a name="p430182011462"></a>最大长度：<strong id="b123052014617"><a name="b123052014617"></a><a name="b123052014617"></a>10240</strong></p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section43015204468"></a>

无

## 请求示例<a name="section163372018469"></a>

```
DELETE https://{NAT_endpoint}/v2/d199ba7e0ba64899b2e81518104b1526d/nat_gateways/a78fb3eb-1654-4710-8742-3fc49d5f04f8

  
```

## 响应示例<a name="section18341820194620"></a>

无

## 状态码<a name="section23522014614"></a>

<a name="zh-cn_topic_0297140325_status_code"></a>
<table><thead align="left"><tr id="row136162034614"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p1437102074610"><a name="p1437102074610"></a><a name="p1437102074610"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p123712016461"><a name="p123712016461"></a><a name="p123712016461"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row193652011463"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p2381920154611"><a name="p2381920154611"></a><a name="p2381920154611"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p193810202465"><a name="p193810202465"></a><a name="p193810202465"></a>删除公网NAT网关实例成功。</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section203911200466"></a>

请参见[错误码](错误码.md)。

