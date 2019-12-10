# 查询指定的DNAT规则详情<a name="ZH-CN_TOPIC_0201533643"></a>

## 功能介绍<a name="section242916116504"></a>

查询指定的DNAT规则详情。

## URI<a name="section55252672165026"></a>

GET /v2.0/dnat\_rules/\{dnat\_rule\_id\}

**表 1**  参数说明

<a name="table41603310017"></a>
<table><thead align="left"><tr id="row323012314017"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p1023043508"><a name="p1023043508"></a><a name="p1023043508"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="22%" id="mcps1.2.5.1.2"><p id="p1823017318015"><a name="p1823017318015"></a><a name="p1823017318015"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="p52301036011"><a name="p52301036011"></a><a name="p52301036011"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="32%" id="mcps1.2.5.1.4"><p id="p7230330014"><a name="p7230330014"></a><a name="p7230330014"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row9230031106"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1823033907"><a name="p1823033907"></a><a name="p1823033907"></a>dnat_rule_id</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.2.5.1.2 "><p id="p42301335017"><a name="p42301335017"></a><a name="p42301335017"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p623013311018"><a name="p623013311018"></a><a name="p623013311018"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.5.1.4 "><p id="p5230735019"><a name="p5230735019"></a><a name="p5230735019"></a>所属DNAT规则的id。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section30445355165052"></a>

无

## 响应消息<a name="section1412948816517"></a>

响应参数如[表2](#table66411570165117)所示。

**表 2**  响应参数

<a name="table66411570165117"></a>
<table><thead align="left"><tr id="row43436947165117"><th class="cellrowborder" valign="top" width="20.75%" id="mcps1.2.4.1.1"><p id="p28731843165117"><a name="p28731843165117"></a><a name="p28731843165117"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="21.88%" id="mcps1.2.4.1.2"><p id="p45577964165117"><a name="p45577964165117"></a><a name="p45577964165117"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.37%" id="mcps1.2.4.1.3"><p id="p67033414165117"><a name="p67033414165117"></a><a name="p67033414165117"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row60997448165117"><td class="cellrowborder" valign="top" width="20.75%" headers="mcps1.2.4.1.1 "><p id="p41846242165117"><a name="p41846242165117"></a><a name="p41846242165117"></a>dnat_rule</p>
</td>
<td class="cellrowborder" valign="top" width="21.88%" headers="mcps1.2.4.1.2 "><p id="p34102461165117"><a name="p34102461165117"></a><a name="p34102461165117"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="57.37%" headers="mcps1.2.4.1.3 "><p id="p5298260165117"><a name="p5298260165117"></a><a name="p5298260165117"></a>dnat_rule对象。详见<a href="#table9899152414719">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  dnat\_rule字段说明

<a name="table9899152414719"></a>
<table><thead align="left"><tr id="row198997241973"><th class="cellrowborder" valign="top" width="20.312031203120313%" id="mcps1.2.4.1.1"><p id="p3368163219712"><a name="p3368163219712"></a><a name="p3368163219712"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="22.58225822582258%" id="mcps1.2.4.1.2"><p id="p23681832770"><a name="p23681832770"></a><a name="p23681832770"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.1057105710571%" id="mcps1.2.4.1.3"><p id="p23681432671"><a name="p23681432671"></a><a name="p23681432671"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row88993241676"><td class="cellrowborder" valign="top" width="20.312031203120313%" headers="mcps1.2.4.1.1 "><p id="p1136816321074"><a name="p1136816321074"></a><a name="p1136816321074"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="22.58225822582258%" headers="mcps1.2.4.1.2 "><p id="p1236803212715"><a name="p1236803212715"></a><a name="p1236803212715"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.1057105710571%" headers="mcps1.2.4.1.3 "><p id="p636818322071"><a name="p636818322071"></a><a name="p636818322071"></a>DNAT规则的id。</p>
</td>
</tr>
<tr id="row198999241712"><td class="cellrowborder" valign="top" width="20.312031203120313%" headers="mcps1.2.4.1.1 "><p id="p15368632273"><a name="p15368632273"></a><a name="p15368632273"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.58225822582258%" headers="mcps1.2.4.1.2 "><p id="p6368132672"><a name="p6368132672"></a><a name="p6368132672"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.1057105710571%" headers="mcps1.2.4.1.3 "><p id="p4368193211713"><a name="p4368193211713"></a><a name="p4368193211713"></a>项目的ID。</p>
</td>
</tr>
<tr id="row18993246715"><td class="cellrowborder" valign="top" width="20.312031203120313%" headers="mcps1.2.4.1.1 "><p id="p10368143213712"><a name="p10368143213712"></a><a name="p10368143213712"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.58225822582258%" headers="mcps1.2.4.1.2 "><p id="p03681132579"><a name="p03681132579"></a><a name="p03681132579"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.1057105710571%" headers="mcps1.2.4.1.3 "><p id="p0368163220715"><a name="p0368163220715"></a><a name="p0368163220715"></a>所属NAT网关的id。</p>
</td>
</tr>
<tr id="row1899924074"><td class="cellrowborder" valign="top" width="20.312031203120313%" headers="mcps1.2.4.1.1 "><p id="p0368183220715"><a name="p0368183220715"></a><a name="p0368183220715"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.58225822582258%" headers="mcps1.2.4.1.2 "><p id="p12368932672"><a name="p12368932672"></a><a name="p12368932672"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.1057105710571%" headers="mcps1.2.4.1.3 "><p id="p3368132676"><a name="p3368132676"></a><a name="p3368132676"></a>虚拟机或者裸机的Port ID。</p>
</td>
</tr>
<tr id="row38991524672"><td class="cellrowborder" valign="top" width="20.312031203120313%" headers="mcps1.2.4.1.1 "><p id="p836823213715"><a name="p836823213715"></a><a name="p836823213715"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="22.58225822582258%" headers="mcps1.2.4.1.2 "><p id="p1636843210716"><a name="p1636843210716"></a><a name="p1636843210716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.1057105710571%" headers="mcps1.2.4.1.3 "><p id="p2036803210718"><a name="p2036803210718"></a><a name="p2036803210718"></a>用户私有IP地址，例如专线连接的私有云地址。</p>
</td>
</tr>
<tr id="row48998241373"><td class="cellrowborder" valign="top" width="20.312031203120313%" headers="mcps1.2.4.1.1 "><p id="p936811322076"><a name="p936811322076"></a><a name="p936811322076"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="22.58225822582258%" headers="mcps1.2.4.1.2 "><p id="p6368153211712"><a name="p6368153211712"></a><a name="p6368153211712"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.1057105710571%" headers="mcps1.2.4.1.3 "><p id="p15368123218715"><a name="p15368123218715"></a><a name="p15368123218715"></a>虚拟机或者裸机对外提供服务的协议端口号。</p>
</td>
</tr>
<tr id="row1789914241878"><td class="cellrowborder" valign="top" width="20.312031203120313%" headers="mcps1.2.4.1.1 "><p id="p43681532970"><a name="p43681532970"></a><a name="p43681532970"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.58225822582258%" headers="mcps1.2.4.1.2 "><p id="p123684326717"><a name="p123684326717"></a><a name="p123684326717"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.1057105710571%" headers="mcps1.2.4.1.3 "><p id="p93683323710"><a name="p93683323710"></a><a name="p93683323710"></a>弹性公网IP的id。</p>
</td>
</tr>
<tr id="row7899102413716"><td class="cellrowborder" valign="top" width="20.312031203120313%" headers="mcps1.2.4.1.1 "><p id="p1336843213714"><a name="p1336843213714"></a><a name="p1336843213714"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="22.58225822582258%" headers="mcps1.2.4.1.2 "><p id="p536820321572"><a name="p536820321572"></a><a name="p536820321572"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.1057105710571%" headers="mcps1.2.4.1.3 "><p id="p193681532072"><a name="p193681532072"></a><a name="p193681532072"></a>弹性公网的IP地址。</p>
</td>
</tr>
<tr id="row889916241373"><td class="cellrowborder" valign="top" width="20.312031203120313%" headers="mcps1.2.4.1.1 "><p id="p73686321175"><a name="p73686321175"></a><a name="p73686321175"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="22.58225822582258%" headers="mcps1.2.4.1.2 "><p id="p1836813210719"><a name="p1836813210719"></a><a name="p1836813210719"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.1057105710571%" headers="mcps1.2.4.1.3 "><p id="p73683325711"><a name="p73683325711"></a><a name="p73683325711"></a>Floatingip对外提供服务的端口号。</p>
</td>
</tr>
<tr id="row489932414710"><td class="cellrowborder" valign="top" width="20.312031203120313%" headers="mcps1.2.4.1.1 "><p id="p17368232474"><a name="p17368232474"></a><a name="p17368232474"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="22.58225822582258%" headers="mcps1.2.4.1.2 "><p id="p163683321719"><a name="p163683321719"></a><a name="p163683321719"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.1057105710571%" headers="mcps1.2.4.1.3 "><p id="p336893219716"><a name="p336893219716"></a><a name="p336893219716"></a>协议类型，目前支持TCP/UDP/ANY</p>
<p id="p9368432271"><a name="p9368432271"></a><a name="p9368432271"></a>对应协议号6/17/0</p>
</td>
</tr>
<tr id="row389917241879"><td class="cellrowborder" valign="top" width="20.312031203120313%" headers="mcps1.2.4.1.1 "><p id="p1736833215711"><a name="p1736833215711"></a><a name="p1736833215711"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="22.58225822582258%" headers="mcps1.2.4.1.2 "><p id="p736853214714"><a name="p736853214714"></a><a name="p736853214714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.1057105710571%" headers="mcps1.2.4.1.3 "><a name="ul113681321476"></a><a name="ul113681321476"></a><ul id="ul113681321476"><li>功能说明：DNAT规则的状态。</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="row1589910244715"><td class="cellrowborder" valign="top" width="20.312031203120313%" headers="mcps1.2.4.1.1 "><p id="p1836883218715"><a name="p1836883218715"></a><a name="p1836883218715"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="22.58225822582258%" headers="mcps1.2.4.1.2 "><p id="p1764614265487"><a name="p1764614265487"></a><a name="p1764614265487"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="57.1057105710571%" headers="mcps1.2.4.1.3 "><a name="ul71858556358"></a><a name="ul71858556358"></a><ul id="ul71858556358"><li>解冻/冻结状态。</li><li>取值范围：<a name="ul11838172814409"></a><a name="ul11838172814409"></a><ul id="ul11838172814409"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="row28997241277"><td class="cellrowborder" valign="top" width="20.312031203120313%" headers="mcps1.2.4.1.1 "><p id="p13368332977"><a name="p13368332977"></a><a name="p13368332977"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="22.58225822582258%" headers="mcps1.2.4.1.2 "><p id="p136853217716"><a name="p136853217716"></a><a name="p136853217716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.1057105710571%" headers="mcps1.2.4.1.3 "><a name="ul2036815321717"></a><a name="ul2036815321717"></a><ul id="ul2036815321717"><li>DNAT规则的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</li></ul>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section24779297165121"></a>

-   请求样例

    ```
    GET https://{Endpoint}/v2.0/dnat_rules/5b95c675-69c2-4656-ba06-58ff72e1d338
    ```


-   响应样例

    ```
    {              
    　　"dnat_rule": {
        　　"floating_ip_id": "bf99c679-9f41-4dac-8513-9c9228e713e1",
       　　 "status": "ACTIVE",
        　　"nat_gateway_id": "cda3a125-2406-456c-a11f-598e10578541",
       　　 "admin_state_up": true,
       　　 "port_id": "9a469561-daac-4c94-88f5-39366e5ea193",
        　　"internal_service_port": 993,
        　　"protocol": "TCP",
        　　"tenant_id": "abc",
        　　"created_at": "2017-11-15 15:44:42.595173",
        　　"id": "79195d50-0271-41f1-bded-4c089b2502ff",
        　　"floating_ip_address": "5.21.11.226",
       　　 "external_service_port": 242
        　　"private_ip": ""  
       }
    }
    ```


## 状态码<a name="section16249219165526"></a>

请参考[状态码](状态码.md)。

