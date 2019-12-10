# 删除SNAT规则<a name="ZH-CN_TOPIC_0201533692"></a>

## 功能介绍<a name="section20675657"></a>

删除SNAT规则。

## URI<a name="section51863185"></a>

DELETE /v2.0/snat\_rules/\{snat\_rule\_id\}

**表 1**  参数说明

<a name="table1910716134591"></a>
<table><thead align="left"><tr id="row3169413135915"><th class="cellrowborder" valign="top" width="25.26252625262526%" id="mcps1.2.5.1.1"><p id="p16169131375910"><a name="p16169131375910"></a><a name="p16169131375910"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.431343134313432%" id="mcps1.2.5.1.2"><p id="p151699135593"><a name="p151699135593"></a><a name="p151699135593"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="19.2019201920192%" id="mcps1.2.5.1.3"><p id="p1716915133591"><a name="p1716915133591"></a><a name="p1716915133591"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.104210421042104%" id="mcps1.2.5.1.4"><p id="p016991320594"><a name="p016991320594"></a><a name="p016991320594"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row131691913145916"><td class="cellrowborder" valign="top" width="25.26252625262526%" headers="mcps1.2.5.1.1 "><p id="p116919133595"><a name="p116919133595"></a><a name="p116919133595"></a>snat_rule_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.431343134313432%" headers="mcps1.2.5.1.2 "><p id="p6169171310597"><a name="p6169171310597"></a><a name="p6169171310597"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.2019201920192%" headers="mcps1.2.5.1.3 "><p id="p101695138597"><a name="p101695138597"></a><a name="p101695138597"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.104210421042104%" headers="mcps1.2.5.1.4 "><p id="p31691313145913"><a name="p31691313145913"></a><a name="p31691313145913"></a>所属SNAT规则的id。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section40168441"></a>

无

## 响应消息<a name="section25971650"></a>

无

## 示例<a name="section32418265"></a>

-   请求样例

    ```
    DELETE https://{Endpoint}/v2.0/snat_rules/a78fb3eb-1654-4710-8742-3fc49d5f04f8
    ```


-   响应样例

    ```
    无（STATUS CODE 204）
    ```


## 状态码<a name="section8633818"></a>

请参考[状态码](状态码.md)。

