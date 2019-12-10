# 删除DNAT规则<a name="ZH-CN_TOPIC_0201533686"></a>

## 功能介绍<a name="section133765317113"></a>

删除DNAT规则。

## URI<a name="section57269908171124"></a>

DELETE /v2.0/dnat\_rules/\{dnat\_rule\_id\}

**表 1**  参数说明

<a name="table41603310017"></a>
<table><thead align="left"><tr id="row323012314017"><th class="cellrowborder" valign="top" width="23.54%" id="mcps1.2.5.1.1"><p id="p1023043508"><a name="p1023043508"></a><a name="p1023043508"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.939999999999998%" id="mcps1.2.5.1.2"><p id="p52301036011"><a name="p52301036011"></a><a name="p52301036011"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.029999999999998%" id="mcps1.2.5.1.3"><p id="p1823017318015"><a name="p1823017318015"></a><a name="p1823017318015"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="38.49%" id="mcps1.2.5.1.4"><p id="p7230330014"><a name="p7230330014"></a><a name="p7230330014"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row9230031106"><td class="cellrowborder" valign="top" width="23.54%" headers="mcps1.2.5.1.1 "><p id="p1823033907"><a name="p1823033907"></a><a name="p1823033907"></a>dnat_rule_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.939999999999998%" headers="mcps1.2.5.1.2 "><p id="p623013311018"><a name="p623013311018"></a><a name="p623013311018"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.029999999999998%" headers="mcps1.2.5.1.3 "><p id="p42301335017"><a name="p42301335017"></a><a name="p42301335017"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.49%" headers="mcps1.2.5.1.4 "><p id="p5230735019"><a name="p5230735019"></a><a name="p5230735019"></a>所属DNAT规则的id。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section57861162171148"></a>

无

## 响应消息<a name="section1248980417125"></a>

无

## 示例<a name="section16888175171218"></a>

-   请求样例

    ```
    DELETE https://{Endpoint}/v2.0/dnat_rules/a78fb3eb-1654-4710-8742-3fc49d5f04f8
    ```


-   响应样例

    ```
    无（STATUS CODE 204）
    ```


## 状态码<a name="section21780566171318"></a>

请参考[状态码](状态码.md)。

