# 创建SNAT规则<a name="ZH-CN_TOPIC_0130808157"></a>

## 功能介绍<a name="section45647471"></a>

创建SNAT规则。

>![](public_sys-resources/icon-note.gif) **说明：**   
>创建规则时，要求网关状态status = "ACTIVE"，要求网关管理员状态admin\_state\_up = True。  

## URI<a name="section8174056"></a>

POST /v2.0/snat\_rules

## 请求消息<a name="section58118839"></a>

请求参数如[表1](#table9655225)所示。

**表 1**  请求参数

<a name="table9655225"></a>
<table><thead align="left"><tr id="row16018111"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.2.5.1.1"><p id="p22398640"><a name="p22398640"></a><a name="p22398640"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="12.24%" id="mcps1.2.5.1.2"><p id="p2350590"><a name="p2350590"></a><a name="p2350590"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="14.29%" id="mcps1.2.5.1.3"><p id="p56180112"><a name="p56180112"></a><a name="p56180112"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="52.04%" id="mcps1.2.5.1.4"><p id="p54295247"><a name="p54295247"></a><a name="p54295247"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row35838882"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.1 "><p id="p17268338"><a name="p17268338"></a><a name="p17268338"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.2 "><p id="p56558118"><a name="p56558118"></a><a name="p56558118"></a>Uuid-Str</p>
</td>
<td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.3 "><p id="p17804839"><a name="p17804839"></a><a name="p17804839"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="52.04%" headers="mcps1.2.5.1.4 "><p id="p1330112415579"><a name="p1330112415579"></a><a name="p1330112415579"></a>所属NAT网关的id。</p>
</td>
</tr>
<tr id="row27716925"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.1 "><p id="p30478492"><a name="p30478492"></a><a name="p30478492"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.2 "><p id="p52838820"><a name="p52838820"></a><a name="p52838820"></a>Uuid-Str</p>
</td>
<td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.3 "><p id="p52086012"><a name="p52086012"></a><a name="p52086012"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="52.04%" headers="mcps1.2.5.1.4 "><p id="p494913202574"><a name="p494913202574"></a><a name="p494913202574"></a>规则使用的网络id。与cidr参数二选一。</p>
</td>
</tr>
<tr id="row1301427182716"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.1 "><p id="p5300638112711"><a name="p5300638112711"></a><a name="p5300638112711"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.2 "><p id="p1830063862717"><a name="p1830063862717"></a><a name="p1830063862717"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.3 "><p id="p143001638102715"><a name="p143001638102715"></a><a name="p143001638102715"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="52.04%" headers="mcps1.2.5.1.4 "><p id="p830023810275"><a name="p830023810275"></a><a name="p830023810275"></a>cidr，可以是网段或者主机格式，与network_id参数二选一。</p>
<p id="p49176911316"><a name="p49176911316"></a><a name="p49176911316"></a>Source_type=0时，cidr必须是vpc 子网网段的子集(不能相等）;</p>
<p id="p109178993117"><a name="p109178993117"></a><a name="p109178993117"></a>Source_type=1时，cidr必须指定专线侧网段， 且不能与vpc侧的网段冲突。</p>
</td>
</tr>
<tr id="row12031224162716"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.1 "><p id="p0814549132719"><a name="p0814549132719"></a><a name="p0814549132719"></a>source_type</p>
</td>
<td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.2 "><p id="p198146498274"><a name="p198146498274"></a><a name="p198146498274"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.3 "><p id="p28146498279"><a name="p28146498279"></a><a name="p28146498279"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="52.04%" headers="mcps1.2.5.1.4 "><p id="p15814184919276"><a name="p15814184919276"></a><a name="p15814184919276"></a>0：VPC侧，可以指定network_id 或者cidr</p>
<p id="p3814144915278"><a name="p3814144915278"></a><a name="p3814144915278"></a>1：专线侧,只能指定cidr</p>
<p id="p188141049122717"><a name="p188141049122717"></a><a name="p188141049122717"></a>不输入默认为0（VPC）</p>
</td>
</tr>
<tr id="row54194737"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.1 "><p id="p27697577"><a name="p27697577"></a><a name="p27697577"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.2 "><p id="p28911278"><a name="p28911278"></a><a name="p28911278"></a>Uuid-Str</p>
</td>
<td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.3 "><p id="p60112167"><a name="p60112167"></a><a name="p60112167"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="52.04%" headers="mcps1.2.5.1.4 "><p id="p37247357"><a name="p37247357"></a><a name="p37247357"></a>浮动IP的id。</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section53307511"></a>

响应参数如[表2](#table64245911)所示。

**表 2**  响应参数

<a name="table64245911"></a>
<table><thead align="left"><tr id="row15388566"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p38514356"><a name="p38514356"></a><a name="p38514356"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="26%" id="mcps1.2.4.1.2"><p id="p32655106"><a name="p32655106"></a><a name="p32655106"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.4.1.3"><p id="p38657103"><a name="p38657103"></a><a name="p38657103"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row44217630"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p24858302"><a name="p24858302"></a><a name="p24858302"></a>snat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.4.1.2 "><p id="p256599"><a name="p256599"></a><a name="p256599"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.4.1.3 "><p id="p5825169"><a name="p5825169"></a><a name="p5825169"></a>snat_rule对象。</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section10005551"></a>

-   请求样例

1.  VPC 侧指定network\_id

    ```
    POST /v2.0/snat_rules   
    {
        "snat_rule": {
            "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
            "network_id": "eaad9cd6-2372-4be1-9535-9bd37210ae7b",
            "source_type":0,
            "floating_ip_id": "bdc10a4c-d81a-41ec-adf7-de857f7c812a"
        }
    }
    ```


1.  VPC侧指定CIDR

    ```
    POST /v2.0/snat_rules 
    {      
       "snat_rule": {
             "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
             "cidr": "192.168.1.10/32",
             "source_type":0,
             "floating_ip_id": "bdc10a4c-d81a-41ec-adf7-de857f7c812a"
          }
      }
    ```


1.  专线侧 指定CIDR

    ```
    POST /v2.0/snat_rules
     {
          "snat_rule": { 
             "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
             "cidr": "172.30.0.0/24",
             "source_type":1,
             "floating_ip_id": "bdc10a4c-d81a-41ec-adf7-de857f7c812a"
          }
      }
    ```


-   响应样例

    ```
    {
        "snat_rule": {
            "floating_ip_id": "bdc10a4c-d81a-41ec-adf7-de857f7c812a",
            "status": "PENDING_CREATE",
            "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
            "admin_state_up": true,
            "network_id": "eaad9cd6-2372-4be1-9535-9bd37210ae7b",
            "cidr": "",
            "source_type":0,
            "tenant_id": "27e25061336f4af590faeabeb7fcd9a3",
            "created_at": "2017-11-18 07:54:21.665430",
            "id": "5b95c675-69c2-4656-ba06-58ff72e1d338",
            "floating_ip_address": "5.21.11.226"
        }
    }
    ```


## 返回值<a name="section5143287"></a>

请参见[通用请求返回值](通用请求返回值.md)。

