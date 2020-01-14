# 删除DNAT规则<a name="nat_apiv2_0022"></a>

## 功能介绍<a name="zh-cn_topic_0168797267_section133765317113"></a>

删除DNAT规则。

## URI<a name="zh-cn_topic_0168797267_section57269908171124"></a>

DELETE /v2/\{project\_id\}/nat\_gateways/\{nat\_gateway\_id\}/dnat\_rules/\{dnat\_rule\_id\}

**表 1**  参数说明

<a name="zh-cn_topic_0168797267_table41603310017"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797267_row323012314017"><th class="cellrowborder" valign="top" width="25.55%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797267_p1023043508"><a name="zh-cn_topic_0168797267_p1023043508"></a><a name="zh-cn_topic_0168797267_p1023043508"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="9.5%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797267_p52301036011"><a name="zh-cn_topic_0168797267_p52301036011"></a><a name="zh-cn_topic_0168797267_p52301036011"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20.630000000000003%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797267_p13639165734619"><a name="zh-cn_topic_0168797267_p13639165734619"></a><a name="zh-cn_topic_0168797267_p13639165734619"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.32%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797267_p7230330014"><a name="zh-cn_topic_0168797267_p7230330014"></a><a name="zh-cn_topic_0168797267_p7230330014"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797267_row191481149171112"><td class="cellrowborder" valign="top" width="25.55%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797267_p381314552117"><a name="zh-cn_topic_0168797267_p381314552117"></a><a name="zh-cn_topic_0168797267_p381314552117"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="9.5%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797267_p1981365501117"><a name="zh-cn_topic_0168797267_p1981365501117"></a><a name="zh-cn_topic_0168797267_p1981365501117"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797267_p126394578462"><a name="zh-cn_topic_0168797267_p126394578462"></a><a name="zh-cn_topic_0168797267_p126394578462"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.32%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797267_p13813655151118"><a name="zh-cn_topic_0168797267_p13813655151118"></a><a name="zh-cn_topic_0168797267_p13813655151118"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797267_row14294845131111"><td class="cellrowborder" valign="top" width="25.55%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797267_p6813115551112"><a name="zh-cn_topic_0168797267_p6813115551112"></a><a name="zh-cn_topic_0168797267_p6813115551112"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="9.5%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797267_p3813355191119"><a name="zh-cn_topic_0168797267_p3813355191119"></a><a name="zh-cn_topic_0168797267_p3813355191119"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797267_p26391457114619"><a name="zh-cn_topic_0168797267_p26391457114619"></a><a name="zh-cn_topic_0168797267_p26391457114619"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.32%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797267_p1281375581118"><a name="zh-cn_topic_0168797267_p1281375581118"></a><a name="zh-cn_topic_0168797267_p1281375581118"></a>DNAT规则所在NAT网关的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797267_row9230031106"><td class="cellrowborder" valign="top" width="25.55%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797267_p1823033907"><a name="zh-cn_topic_0168797267_p1823033907"></a><a name="zh-cn_topic_0168797267_p1823033907"></a>dnat_rule_id</p>
</td>
<td class="cellrowborder" valign="top" width="9.5%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797267_p623013311018"><a name="zh-cn_topic_0168797267_p623013311018"></a><a name="zh-cn_topic_0168797267_p623013311018"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.630000000000003%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797267_p116391257174619"><a name="zh-cn_topic_0168797267_p116391257174619"></a><a name="zh-cn_topic_0168797267_p116391257174619"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.32%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797267_p5230735019"><a name="zh-cn_topic_0168797267_p5230735019"></a><a name="zh-cn_topic_0168797267_p5230735019"></a>DNAT规则的id。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0168797267_section57861162171148"></a>

无

## 响应消息<a name="zh-cn_topic_0168797267_section1248980417125"></a>

无

## 示例<a name="zh-cn_topic_0168797267_section16888175171218"></a>

-   请求样例

    ```
    DELETE https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526d/nat_gateways/f4dfea98-874a-46f7-aa2a-fb348d0ceb02/dnat_rules/a78fb3eb-1654-4710-8742-3fc49d5f04f8
    ```


-   响应样例

    ```
    无（STATUS CODE 204）
    ```


## 状态码<a name="zh-cn_topic_0168797267_section21780566171318"></a>

请参考[状态码](状态码.md)。

