# 查询指定的SNAT规则详情<a name="ZH-CN_TOPIC_0201533641"></a>

## 功能介绍<a name="section59567946"></a>

查询指定的SNAT规则详情。

## URI<a name="section66349468"></a>

GET /v2.0/snat\_rules/\{snat\_rule\_id\}

**表 1**  参数说明

<a name="table1910716134591"></a>
<table><thead align="left"><tr id="row3169413135915"><th class="cellrowborder" valign="top" width="21.272127212721273%" id="mcps1.2.5.1.1"><p id="p16169131375910"><a name="p16169131375910"></a><a name="p16169131375910"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.842084208420843%" id="mcps1.2.5.1.2"><p id="p151699135593"><a name="p151699135593"></a><a name="p151699135593"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.781578157815781%" id="mcps1.2.5.1.3"><p id="p1716915133591"><a name="p1716915133591"></a><a name="p1716915133591"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.104210421042104%" id="mcps1.2.5.1.4"><p id="p016991320594"><a name="p016991320594"></a><a name="p016991320594"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row131691913145916"><td class="cellrowborder" valign="top" width="21.272127212721273%" headers="mcps1.2.5.1.1 "><p id="p116919133595"><a name="p116919133595"></a><a name="p116919133595"></a>snat_rule_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.842084208420843%" headers="mcps1.2.5.1.2 "><p id="p6169171310597"><a name="p6169171310597"></a><a name="p6169171310597"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.781578157815781%" headers="mcps1.2.5.1.3 "><p id="p101695138597"><a name="p101695138597"></a><a name="p101695138597"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.104210421042104%" headers="mcps1.2.5.1.4 "><p id="p31691313145913"><a name="p31691313145913"></a><a name="p31691313145913"></a>所属SNAT规则的id。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section5597798"></a>

无

## 响应消息<a name="section50380184"></a>

响应参数如[表2](#table65459315)所示。

**表 2**  响应参数

<a name="table65459315"></a>
<table><thead align="left"><tr id="row47811128"><th class="cellrowborder" valign="top" width="20.73%" id="mcps1.2.4.1.1"><p id="p47496137"><a name="p47496137"></a><a name="p47496137"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="28.050000000000004%" id="mcps1.2.4.1.2"><p id="p21981920"><a name="p21981920"></a><a name="p21981920"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p6428601"><a name="p6428601"></a><a name="p6428601"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row50954701"><td class="cellrowborder" valign="top" width="20.73%" headers="mcps1.2.4.1.1 "><p id="p33690117"><a name="p33690117"></a><a name="p33690117"></a>snat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="28.050000000000004%" headers="mcps1.2.4.1.2 "><p id="p44544970"><a name="p44544970"></a><a name="p44544970"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p447513"><a name="p447513"></a><a name="p447513"></a>snat_rule对象。详见<a href="#table113261845122312">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  snat\_rule字段说明

<a name="table113261845122312"></a>
<table><thead align="left"><tr id="row3326164512310"><th class="cellrowborder" valign="top" width="20.662066206620665%" id="mcps1.2.4.1.1"><p id="p144282010346"><a name="p144282010346"></a><a name="p144282010346"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="28.25282528252825%" id="mcps1.2.4.1.2"><p id="p1742881017412"><a name="p1742881017412"></a><a name="p1742881017412"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.085108510851086%" id="mcps1.2.4.1.3"><p id="p1442813106416"><a name="p1442813106416"></a><a name="p1442813106416"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row73267459231"><td class="cellrowborder" valign="top" width="20.662066206620665%" headers="mcps1.2.4.1.1 "><p id="p4180209175512"><a name="p4180209175512"></a><a name="p4180209175512"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="28.25282528252825%" headers="mcps1.2.4.1.2 "><p id="p318018955517"><a name="p318018955517"></a><a name="p318018955517"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.085108510851086%" headers="mcps1.2.4.1.3 "><p id="p418017905520"><a name="p418017905520"></a><a name="p418017905520"></a>SNAT规则的id。</p>
</td>
</tr>
<tr id="row11326845102317"><td class="cellrowborder" valign="top" width="20.662066206620665%" headers="mcps1.2.4.1.1 "><p id="p2180189185519"><a name="p2180189185519"></a><a name="p2180189185519"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.25282528252825%" headers="mcps1.2.4.1.2 "><p id="p11801797556"><a name="p11801797556"></a><a name="p11801797556"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.085108510851086%" headers="mcps1.2.4.1.3 "><p id="p6180499553"><a name="p6180499553"></a><a name="p6180499553"></a>项目的ID。</p>
</td>
</tr>
<tr id="row13261445132318"><td class="cellrowborder" valign="top" width="20.662066206620665%" headers="mcps1.2.4.1.1 "><p id="p1718019914553"><a name="p1718019914553"></a><a name="p1718019914553"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.25282528252825%" headers="mcps1.2.4.1.2 "><p id="p318009145510"><a name="p318009145510"></a><a name="p318009145510"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.085108510851086%" headers="mcps1.2.4.1.3 "><p id="p21801692559"><a name="p21801692559"></a><a name="p21801692559"></a>所属NAT网关的id。</p>
</td>
</tr>
<tr id="row2032617455238"><td class="cellrowborder" valign="top" width="20.662066206620665%" headers="mcps1.2.4.1.1 "><p id="p1518016915520"><a name="p1518016915520"></a><a name="p1518016915520"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.25282528252825%" headers="mcps1.2.4.1.2 "><p id="p181803945519"><a name="p181803945519"></a><a name="p181803945519"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.085108510851086%" headers="mcps1.2.4.1.3 "><p id="p13180179195519"><a name="p13180179195519"></a><a name="p13180179195519"></a>规则使用的网络id。</p>
</td>
</tr>
<tr id="row1632610451230"><td class="cellrowborder" valign="top" width="20.662066206620665%" headers="mcps1.2.4.1.1 "><p id="p201802919559"><a name="p201802919559"></a><a name="p201802919559"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="28.25282528252825%" headers="mcps1.2.4.1.2 "><p id="p7180592555"><a name="p7180592555"></a><a name="p7180592555"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.085108510851086%" headers="mcps1.2.4.1.3 "><p id="p16180139205514"><a name="p16180139205514"></a><a name="p16180139205514"></a>cidr，vpc 子网网段的子集或专线侧网段。</p>
</td>
</tr>
<tr id="row11326645162317"><td class="cellrowborder" valign="top" width="20.662066206620665%" headers="mcps1.2.4.1.1 "><p id="p0180129105513"><a name="p0180129105513"></a><a name="p0180129105513"></a>source_type</p>
</td>
<td class="cellrowborder" valign="top" width="28.25282528252825%" headers="mcps1.2.4.1.2 "><p id="p1118089165512"><a name="p1118089165512"></a><a name="p1118089165512"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="51.085108510851086%" headers="mcps1.2.4.1.3 "><p id="p1118010920557"><a name="p1118010920557"></a><a name="p1118010920557"></a>0：VPC侧，可以指定network_id 或者cidr</p>
<p id="p61801291556"><a name="p61801291556"></a><a name="p61801291556"></a>1：专线侧，只能指定cidr</p>
<p id="p131806910557"><a name="p131806910557"></a><a name="p131806910557"></a>不输入默认为0（VPC）</p>
</td>
</tr>
<tr id="row4326104512234"><td class="cellrowborder" valign="top" width="20.662066206620665%" headers="mcps1.2.4.1.1 "><p id="p891724055516"><a name="p891724055516"></a><a name="p891724055516"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.25282528252825%" headers="mcps1.2.4.1.2 "><p id="p39177408550"><a name="p39177408550"></a><a name="p39177408550"></a>String(4096)</p>
</td>
<td class="cellrowborder" valign="top" width="51.085108510851086%" headers="mcps1.2.4.1.3 "><a name="ul391714011555"></a><a name="ul391714011555"></a><ul id="ul391714011555"><li>功能说明：弹性公网IP的id，多个弹性公网IP使用逗号分隔。</li><li>取值范围：最大长度4096字节。</li><li>约束：弹性公网IP的id个数不能超过20个</li></ul>
</td>
</tr>
<tr id="row2785103161819"><td class="cellrowborder" valign="top" width="20.662066206620665%" headers="mcps1.2.4.1.1 "><p id="p1791083317183"><a name="p1791083317183"></a><a name="p1791083317183"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="28.25282528252825%" headers="mcps1.2.4.1.2 "><p id="p491023317185"><a name="p491023317185"></a><a name="p491023317185"></a>String(1024)</p>
</td>
<td class="cellrowborder" valign="top" width="51.085108510851086%" headers="mcps1.2.4.1.3 "><a name="ul39101233161818"></a><a name="ul39101233161818"></a><ul id="ul39101233161818"><li>功能说明：弹性公网IP，多个弹性公网IP使用逗号分隔。</li><li>取值范围：最大长度1024字节。</li></ul>
</td>
</tr>
<tr id="row932614518236"><td class="cellrowborder" valign="top" width="20.662066206620665%" headers="mcps1.2.4.1.1 "><p id="p9917640115517"><a name="p9917640115517"></a><a name="p9917640115517"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="28.25282528252825%" headers="mcps1.2.4.1.2 "><p id="p1917204015553"><a name="p1917204015553"></a><a name="p1917204015553"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.085108510851086%" headers="mcps1.2.4.1.3 "><a name="ul191724018551"></a><a name="ul191724018551"></a><ul id="ul191724018551"><li>功能说明：SNAT规则的状态</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="row3326134518239"><td class="cellrowborder" valign="top" width="20.662066206620665%" headers="mcps1.2.4.1.1 "><p id="p1491714408557"><a name="p1491714408557"></a><a name="p1491714408557"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="28.25282528252825%" headers="mcps1.2.4.1.2 "><p id="p1764614265487"><a name="p1764614265487"></a><a name="p1764614265487"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="51.085108510851086%" headers="mcps1.2.4.1.3 "><a name="ul71858556358"></a><a name="ul71858556358"></a><ul id="ul71858556358"><li>解冻/冻结状态。</li><li>取值范围：<a name="ul11838172814409"></a><a name="ul11838172814409"></a><ul id="ul11838172814409"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="row1932664512234"><td class="cellrowborder" valign="top" width="20.662066206620665%" headers="mcps1.2.4.1.1 "><p id="p09171040115511"><a name="p09171040115511"></a><a name="p09171040115511"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="28.25282528252825%" headers="mcps1.2.4.1.2 "><p id="p1291734045514"><a name="p1291734045514"></a><a name="p1291734045514"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.085108510851086%" headers="mcps1.2.4.1.3 "><a name="ul1691774045514"></a><a name="ul1691774045514"></a><ul id="ul1691774045514"><li>SNAT规则的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</li></ul>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section50768476"></a>

-   请求样例

    ```
    GET https://{Endpoint}/v2.0/snat_rules/5b95c675-69c2-4656-ba06-58ff72e1d338
    ```


-   响应样例

    ```
    {
        "snat_rule": {
            "floating_ip_id": "bdc10a4c-d81a-41ec-adf7-de857f7c812a",
            "status": "ACTIVE",
            "nat_gateway_id": "a78fb3eb-1654-4710-8742-3fc49d5f04f8",
            "admin_state_up": true,
            "network_id": "eaad9cd6-2372-4be1-9535-9bd37210ae7b",
            "cidr": "null",
            "source_type":0,
            "tenant_id": "27e25061336f4af590faeabeb7fcd9a3",
            "created_at": "2017-11-18 07:54:21.665430",
            "id": "5b95c675-69c2-4656-ba06-58ff72e1d338",
            "floating_ip_address": "5.21.11.226"
        }
    }
    ```


## 状态码<a name="section1941962013172"></a>

请参考[状态码](状态码.md)。

