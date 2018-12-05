# 创建NAT网关<a name="ZH-CN_TOPIC_0130808161"></a>

## 功能介绍<a name="section19627306"></a>

创建NAT网关实例。

## URI<a name="section79426345357"></a>

POST /v2.0/nat\_gateways

## 请求消息<a name="section14118316"></a>

请求参数如[表1](#table19786600)所示。

**表 1**  请求参数

<a name="table19786600"></a>
<table><thead align="left"><tr id="row33617107"><th class="cellrowborder" valign="top" width="22.992299229922992%" id="mcps1.2.5.1.1"><p id="p38631174"><a name="p38631174"></a><a name="p38631174"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="18.84188418841884%" id="mcps1.2.5.1.2"><p id="p42117369"><a name="p42117369"></a><a name="p42117369"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="9.770977097709771%" id="mcps1.2.5.1.3"><p id="p56063700"><a name="p56063700"></a><a name="p56063700"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="48.394839483948395%" id="mcps1.2.5.1.4"><p id="p44865856"><a name="p44865856"></a><a name="p44865856"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row10255716"><td class="cellrowborder" valign="top" width="22.992299229922992%" headers="mcps1.2.5.1.1 "><p id="p25406697"><a name="p25406697"></a><a name="p25406697"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.84188418841884%" headers="mcps1.2.5.1.2 "><p id="p44676599"><a name="p44676599"></a><a name="p44676599"></a>Uuid-Str</p>
</td>
<td class="cellrowborder" valign="top" width="9.770977097709771%" headers="mcps1.2.5.1.3 "><p id="p62034741"><a name="p62034741"></a><a name="p62034741"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="48.394839483948395%" headers="mcps1.2.5.1.4 "><p id="p58758091"><a name="p58758091"></a><a name="p58758091"></a>项目的ID。</p>
</td>
</tr>
<tr id="row59060775"><td class="cellrowborder" valign="top" width="22.992299229922992%" headers="mcps1.2.5.1.1 "><p id="p19193461"><a name="p19193461"></a><a name="p19193461"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.84188418841884%" headers="mcps1.2.5.1.2 "><p id="p11166512"><a name="p11166512"></a><a name="p11166512"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="9.770977097709771%" headers="mcps1.2.5.1.3 "><p id="p32072255"><a name="p32072255"></a><a name="p32072255"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="48.394839483948395%" headers="mcps1.2.5.1.4 "><p id="p47715851"><a name="p47715851"></a><a name="p47715851"></a>NAT网关的名字。</p>
<p id="p123130309445"><a name="p123130309445"></a><a name="p123130309445"></a>NAT网关的名字仅支持数字、字母、_（下划线）、-（中划线）、中文。</p>
</td>
</tr>
<tr id="row26789475"><td class="cellrowborder" valign="top" width="22.992299229922992%" headers="mcps1.2.5.1.1 "><p id="p22463828"><a name="p22463828"></a><a name="p22463828"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="18.84188418841884%" headers="mcps1.2.5.1.2 "><p id="p7630774"><a name="p7630774"></a><a name="p7630774"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="9.770977097709771%" headers="mcps1.2.5.1.3 "><p id="p14112944"><a name="p14112944"></a><a name="p14112944"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="48.394839483948395%" headers="mcps1.2.5.1.4 "><p id="p2297835"><a name="p2297835"></a><a name="p2297835"></a>NAT网关的描述。</p>
</td>
</tr>
<tr id="row20680520"><td class="cellrowborder" valign="top" width="22.992299229922992%" headers="mcps1.2.5.1.1 "><p id="p64509447"><a name="p64509447"></a><a name="p64509447"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="18.84188418841884%" headers="mcps1.2.5.1.2 "><p id="p57882714"><a name="p57882714"></a><a name="p57882714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="9.770977097709771%" headers="mcps1.2.5.1.3 "><p id="p57988266"><a name="p57988266"></a><a name="p57988266"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="48.394839483948395%" headers="mcps1.2.5.1.4 "><p id="p244714563112"><a name="p244714563112"></a><a name="p244714563112"></a>NAT网关的规格。</p>
<p id="p66537950"><a name="p66537950"></a><a name="p66537950"></a>取值为：</p>
<a name="ul6656673816199"></a><a name="ul6656673816199"></a><ul id="ul6656673816199"><li>“1”：小型</li><li>“2”：中型</li><li>“3”：大型</li><li>“4”：超大型</li></ul>
</td>
</tr>
<tr id="row61970641"><td class="cellrowborder" valign="top" width="22.992299229922992%" headers="mcps1.2.5.1.1 "><p id="p53566039"><a name="p53566039"></a><a name="p53566039"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.84188418841884%" headers="mcps1.2.5.1.2 "><p id="p118721389226"><a name="p118721389226"></a><a name="p118721389226"></a>Uuid-Str</p>
</td>
<td class="cellrowborder" valign="top" width="9.770977097709771%" headers="mcps1.2.5.1.3 "><p id="p64773780"><a name="p64773780"></a><a name="p64773780"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="48.394839483948395%" headers="mcps1.2.5.1.4 "><p id="p12184860"><a name="p12184860"></a><a name="p12184860"></a>路由器的UUID。</p>
</td>
</tr>
<tr id="row42554878"><td class="cellrowborder" valign="top" width="22.992299229922992%" headers="mcps1.2.5.1.1 "><p id="p24393109"><a name="p24393109"></a><a name="p24393109"></a>internal_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.84188418841884%" headers="mcps1.2.5.1.2 "><p id="p29684841"><a name="p29684841"></a><a name="p29684841"></a>Uuid-Str</p>
</td>
<td class="cellrowborder" valign="top" width="9.770977097709771%" headers="mcps1.2.5.1.3 "><p id="p55661921"><a name="p55661921"></a><a name="p55661921"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="48.394839483948395%" headers="mcps1.2.5.1.4 "><p id="p12321766"><a name="p12321766"></a><a name="p12321766"></a>NAT网关下行口（DVR的下一跳）所属的network id。</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section59955987"></a>

响应参数如[表2](#table58538975)所示。

**表 2**  响应参数

<a name="table58538975"></a>
<table><thead align="left"><tr id="row46091205"><th class="cellrowborder" valign="top" width="15%" id="mcps1.2.4.1.1"><p id="p42400121"><a name="p42400121"></a><a name="p42400121"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="28.999999999999996%" id="mcps1.2.4.1.2"><p id="p11857806"><a name="p11857806"></a><a name="p11857806"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="56.00000000000001%" id="mcps1.2.4.1.3"><p id="p19896826"><a name="p19896826"></a><a name="p19896826"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1030176"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.1 "><p id="p16335431"><a name="p16335431"></a><a name="p16335431"></a>nat_gateway</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.4.1.2 "><p id="p48101526"><a name="p48101526"></a><a name="p48101526"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="56.00000000000001%" headers="mcps1.2.4.1.3 "><p id="p48238799"><a name="p48238799"></a><a name="p48238799"></a>nat_gateway对象。</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section2732972"></a>

-   请求示例

    ```
    POST /v2.0/nat_gateways    
    {
        "nat_gateway": {
            "name": "nat_001",
            "description": "my nat gateway 01",
            "router_id": "d84f345c-80a1-4fa2-a39c-d0d397c3f09a",
            "internal_network_id": "89d66639-aacb-4929-969d-07080b0f9fd9",
            "spec": "1"
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
            "name": "nat_001"
        }
    }
    ```


## 返回值<a name="section20044197"></a>

请参见[通用请求返回值](通用请求返回值.md)。

