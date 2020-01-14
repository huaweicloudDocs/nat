# 删除SNAT规则<a name="nat_apiv2_0015"></a>

## 功能介绍<a name="zh-cn_topic_0168797236_section20675657"></a>

删除SNAT规则。

## URI<a name="zh-cn_topic_0168797236_section51863185"></a>

DELETE /v2/\{project\_id\}/nat\_gateways/\{nat\_gateway\_id\}/snat\_rules/\{snat\_rule\_id\}

**表 1**  参数说明

<a name="zh-cn_topic_0168797236_table1910716134591"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797236_row3169413135915"><th class="cellrowborder" valign="top" width="20.75%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797236_p16169131375910"><a name="zh-cn_topic_0168797236_p16169131375910"></a><a name="zh-cn_topic_0168797236_p16169131375910"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797236_p151699135593"><a name="zh-cn_topic_0168797236_p151699135593"></a><a name="zh-cn_topic_0168797236_p151699135593"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="19.42%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797236_p2919583389"><a name="zh-cn_topic_0168797236_p2919583389"></a><a name="zh-cn_topic_0168797236_p2919583389"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.68%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797236_p016991320594"><a name="zh-cn_topic_0168797236_p016991320594"></a><a name="zh-cn_topic_0168797236_p016991320594"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797236_row1662462434616"><td class="cellrowborder" valign="top" width="20.75%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797236_p889163014617"><a name="zh-cn_topic_0168797236_p889163014617"></a><a name="zh-cn_topic_0168797236_p889163014617"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797236_p889173064612"><a name="zh-cn_topic_0168797236_p889173064612"></a><a name="zh-cn_topic_0168797236_p889173064612"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.42%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797236_p189145803817"><a name="zh-cn_topic_0168797236_p189145803817"></a><a name="zh-cn_topic_0168797236_p189145803817"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.68%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797236_p38903084617"><a name="zh-cn_topic_0168797236_p38903084617"></a><a name="zh-cn_topic_0168797236_p38903084617"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797236_row1474692034616"><td class="cellrowborder" valign="top" width="20.75%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797236_p489330124612"><a name="zh-cn_topic_0168797236_p489330124612"></a><a name="zh-cn_topic_0168797236_p489330124612"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797236_p14891530184617"><a name="zh-cn_topic_0168797236_p14891530184617"></a><a name="zh-cn_topic_0168797236_p14891530184617"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.42%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797236_p16917589384"><a name="zh-cn_topic_0168797236_p16917589384"></a><a name="zh-cn_topic_0168797236_p16917589384"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.68%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797236_p12896306461"><a name="zh-cn_topic_0168797236_p12896306461"></a><a name="zh-cn_topic_0168797236_p12896306461"></a>SNAT规则所属的NAT网关id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797236_row131691913145916"><td class="cellrowborder" valign="top" width="20.75%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797236_p116919133595"><a name="zh-cn_topic_0168797236_p116919133595"></a><a name="zh-cn_topic_0168797236_p116919133595"></a>snat_rule_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797236_p6169171310597"><a name="zh-cn_topic_0168797236_p6169171310597"></a><a name="zh-cn_topic_0168797236_p6169171310597"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.42%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797236_p391658113818"><a name="zh-cn_topic_0168797236_p391658113818"></a><a name="zh-cn_topic_0168797236_p391658113818"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.68%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797236_p31691313145913"><a name="zh-cn_topic_0168797236_p31691313145913"></a><a name="zh-cn_topic_0168797236_p31691313145913"></a>SNAT规则的id。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0168797236_section40168441"></a>

无

## 响应消息<a name="zh-cn_topic_0168797236_section25971650"></a>

无

## 示例<a name="zh-cn_topic_0168797236_section32418265"></a>

-   请求样例

    ```
    DELETE https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526/nat_gateways/f4dfea98-874a-46f7-aa2a-fb348d0ceb02/snat_rules/a78fb3eb-1654-4710-8742-3fc49d5f04f8
    ```


-   响应样例

    ```
    无（STATUS CODE 204）
    ```


## 状态码<a name="zh-cn_topic_0168797236_section8633818"></a>

请参考[状态码](状态码.md)。

