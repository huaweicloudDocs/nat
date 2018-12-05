# 查询NAT网关列表<a name="ZH-CN_TOPIC_0130808153"></a>

## 功能介绍<a name="section21650537"></a>

查询NAT网关列表。

## URI<a name="section60637113"></a>

GET /v2.0/nat\_gateways?id=\{id\}&name=\{name\}&description=\{description\}&router\_id=\{router\_id\}&internal\_network\_id=\{internal\_network\_id\}&admin\_state\_up=\{admin\_state\_up\}&tenant\_id=\{tenant\_id\}&spec=\{spec\}&status=\{status\}&created\_at=\{created\_at\}&admin\_state\_up=\{admin\_state\_up\}

## 请求消息<a name="section12659140"></a>

无

## 响应消息<a name="section46823401"></a>

响应参数如[表1](#table22746818)所示。

**表 1**  响应参数

<a name="table22746818"></a>
<table><thead align="left"><tr id="row36492363"><th class="cellrowborder" valign="top" width="20.73%" id="mcps1.2.4.1.1"><p id="p3091445"><a name="p3091445"></a><a name="p3091445"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="28.050000000000004%" id="mcps1.2.4.1.2"><p id="p49080483"><a name="p49080483"></a><a name="p49080483"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p28722989"><a name="p28722989"></a><a name="p28722989"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row44860761"><td class="cellrowborder" valign="top" width="20.73%" headers="mcps1.2.4.1.1 "><p id="p9842985"><a name="p9842985"></a><a name="p9842985"></a>nat_gateways</p>
</td>
<td class="cellrowborder" valign="top" width="28.050000000000004%" headers="mcps1.2.4.1.2 "><p id="p59084293"><a name="p59084293"></a><a name="p59084293"></a>List(nat_gateway)</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p31253252"><a name="p31253252"></a><a name="p31253252"></a>nat_gateway对象列表。</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section18757432"></a>

-   请求样例

    ```
    GET /v2.0/nat_gateways
    ```


-   响应样例

    ```
    {
        "nat_gateways": [
            {
                "router_id": "b1d81744-5165-48b8-916e-e56626feb88f",
                "status": "ACTIVE",
                "description": "",
                "admin_state_up": true,
                "tenant_id": "27e25061336f4af590faeabeb7fcd9a3",
                "created_at": "2017-11-15 14:50:39.505112",
                "spec": "2",
                "internal_network_id": "5930796a-6026-4d8b-8790-6c6bfc9f87e8",
                "id": "a253be25-ae7c-4013-978b-3c0785eccd63",
                "name": "wj3"
            },
            {
                "router_id": "305dc52f-13dd-429b-a2d4-444a1039ba0b",
                "status": "ACTIVE",
                "description": "",
                "admin_state_up": true,
                "tenant_id": "27e25061336f4af590faeabeb7fcd9a3",
                "created_at": "2017-11-17 07:41:07.538062",
                "spec": "2",
                "internal_network_id": "fc09463b-4ef8-4c7a-93c8-92d9ca6daf9d",
                "id": "e824f1b4-4290-4ebc-8322-cfff370dbd1e",
                "name": "lyl001"
            }
        ]
    }
    ```


## 返回值<a name="section42956987"></a>

请参见[通用请求返回值](通用请求返回值.md)。

