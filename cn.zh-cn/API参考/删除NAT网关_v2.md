# 删除NAT网关<a name="nat_apiv2_0009"></a>

## 功能介绍<a name="zh-cn_topic_0168797273_section23460301"></a>

删除NAT网关。

## URI<a name="zh-cn_topic_0168797273_section9816121"></a>

DELETE /v2/\{project\_id\}/nat\_gateways/\{nat\_gateway\_id\}

**表 1**  参数说明

<a name="zh-cn_topic_0168797273_table285161395713"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797273_row12912101317577"><th class="cellrowborder" valign="top" width="23.57%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797273_p791271313579"><a name="zh-cn_topic_0168797273_p791271313579"></a><a name="zh-cn_topic_0168797273_p791271313579"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.59%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797273_p1391221355716"><a name="zh-cn_topic_0168797273_p1391221355716"></a><a name="zh-cn_topic_0168797273_p1391221355716"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.11%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797273_p12201257142917"><a name="zh-cn_topic_0168797273_p12201257142917"></a><a name="zh-cn_topic_0168797273_p12201257142917"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="53.73%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797273_p1191216131572"><a name="zh-cn_topic_0168797273_p1191216131572"></a><a name="zh-cn_topic_0168797273_p1191216131572"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797273_row1617152217541"><td class="cellrowborder" valign="top" width="23.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797273_p938911272549"><a name="zh-cn_topic_0168797273_p938911272549"></a><a name="zh-cn_topic_0168797273_p938911272549"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.59%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797273_p1638962717545"><a name="zh-cn_topic_0168797273_p1638962717545"></a><a name="zh-cn_topic_0168797273_p1638962717545"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.11%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797273_p15202165719294"><a name="zh-cn_topic_0168797273_p15202165719294"></a><a name="zh-cn_topic_0168797273_p15202165719294"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.73%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797273_p638962775415"><a name="zh-cn_topic_0168797273_p638962775415"></a><a name="zh-cn_topic_0168797273_p638962775415"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797273_row1591281345717"><td class="cellrowborder" valign="top" width="23.57%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797273_p69121213115717"><a name="zh-cn_topic_0168797273_p69121213115717"></a><a name="zh-cn_topic_0168797273_p69121213115717"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.59%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797273_p1291281325710"><a name="zh-cn_topic_0168797273_p1291281325710"></a><a name="zh-cn_topic_0168797273_p1291281325710"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.11%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797273_p6202165712297"><a name="zh-cn_topic_0168797273_p6202165712297"></a><a name="zh-cn_topic_0168797273_p6202165712297"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.73%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797273_p20912111395719"><a name="zh-cn_topic_0168797273_p20912111395719"></a><a name="zh-cn_topic_0168797273_p20912111395719"></a>NAT网关的id。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0168797273_section56908304"></a>

无

## 响应消息<a name="zh-cn_topic_0168797273_section42412694"></a>

无

## 示例<a name="zh-cn_topic_0168797273_section46169932"></a>

-   请求样例

    ```
    DELETE https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/nat_gateways/a78fb3eb-1654-4710-8742-3fc49d5f04f8
    ```


-   响应样例

    ```
    无（STATUS CODE 204）
    ```


## 状态码<a name="zh-cn_topic_0168797273_section48777045"></a>

请参考[状态码](状态码.md)。

