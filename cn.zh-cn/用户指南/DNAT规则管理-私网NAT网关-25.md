# 添加DNAT规则<a name="nat_privatednat_0001"></a>

## 操作场景<a name="zh-cn_topic_0127293986_section1272311025717"></a>

私网NAT网关创建后，通过添加DNAT规则，则可以通过映射方式将您VPC内的云主机实例对外部私网（IDC或其他VPC）提供服务。

云主机的每个端口分别对应一条DNAT规则，一个云主机的多个端口或者多个云主机需要为外部私网提供服务，则需要创建多条DNAT规则。

## 前提条件<a name="zh-cn_topic_0127293986_section36544171152448"></a>

-   已成功创建私网NAT网关。
-   中转子网与中转IP创建成功。

## 操作步骤<a name="zh-cn_topic_0127293986_section61166376152513"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
3.  在系统首页，单击“网络  \> NAT网关”。

    进入NAT网关页面。

4.  在NAT网关页面，单击“NAT网关\> 私网NAT网关”。

1.  在私网NAT网关页面，单击需要添加DNAT规则的私网NAT网关名称。
2.  在私网NAT网关详情页面中，单击“DNAT规则”页签。
3.  在DNAT规则页签中，单击“添加DNAT规则”。

    >![](public_sys-resources/icon-notice.gif) **须知：** 
    >配置DNAT规则后，需在目标云主机实例中放通对应的安全组规则，否则DNAT规则不能生效。具体操作步骤，请参见[添加安全组规则](https://support.huaweicloud.com/usermanual-vpc/zh-cn_topic_0030969470.html)。

4.  根据界面提示，配置添加DNAT规则参数，详情请参见[表1](#table149569172358)。

    **图 1**  添加DNAT规则<a name="fig125211034143520"></a>  
    ![](figures/添加DNAT规则-2.png "添加DNAT规则-2")

    **表 1**  DNAT规则参数说明

    <a name="table149569172358"></a>
    <table><thead align="left"><tr id="row15953617183514"><th class="cellrowborder" valign="top" width="23.189999999999998%" id="mcps1.2.3.1.1"><p id="p1995317179354"><a name="p1995317179354"></a><a name="p1995317179354"></a><strong id="b1395316175352"><a name="b1395316175352"></a><a name="b1395316175352"></a>参数</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="76.81%" id="mcps1.2.3.1.2"><p id="p9953131793510"><a name="p9953131793510"></a><a name="p9953131793510"></a><strong id="b1095310178356"><a name="b1095310178356"></a><a name="b1095310178356"></a>说明</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1695421713516"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="p99537173359"><a name="p99537173359"></a><a name="p99537173359"></a>端口类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p12953191720359"><a name="p12953191720359"></a><a name="p12953191720359"></a>分为具体端口和所有端口两种类型。</p>
    <a name="ul195481716352"></a><a name="ul195481716352"></a><ul id="ul195481716352"><li>具体端口：属于端口映射方式。私网NAT网关会将以指定协议和端口访问该中转IP的请求转发到目标云主机实例的指定端口上。</li><li>所有端口：属于IP映射方式。此方式相当于为云主机配置了一个私网IP（中转IP），任何访问该中转IP的请求都将转发到目标云服务器实例上。</li></ul>
    </td>
    </tr>
    <tr id="row17954121773510"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="p39543178356"><a name="p39543178356"></a><a name="p39543178356"></a>支持协议</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p12954171716351"><a name="p12954171716351"></a><a name="p12954171716351"></a>协议类型分为TCP和UDP两种类型。端口类型为所有端口时，此参数默认设置为All。</p>
    <p id="p695421723511"><a name="p695421723511"></a><a name="p695421723511"></a>端口类型为具体端口时，可配置此参数。</p>
    </td>
    </tr>
    <tr id="row89541217143512"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="p7954161713512"><a name="p7954161713512"></a><a name="p7954161713512"></a>中转子网</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p79541179356"><a name="p79541179356"></a><a name="p79541179356"></a>选择中转VPC中创建的中转子网，非当前VPC的中转子网。</p>
    </td>
    </tr>
    <tr id="row2955171783510"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="p12954111753518"><a name="p12954111753518"></a><a name="p12954111753518"></a>中转IP</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p6954101712352"><a name="p6954101712352"></a><a name="p6954101712352"></a>通过该中转IP访问用户IDC或其他VPC。</p>
    <p id="p7955181753518"><a name="p7955181753518"></a><a name="p7955181753518"></a><span>这里只能选择没有被绑定的中转IP，或者被绑定在当前私网NAT网关中非“所有端口”类型DNAT规则上的中转IP。</span></p>
    </td>
    </tr>
    <tr id="row1395531720352"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="p1295541793514"><a name="p1295541793514"></a><a name="p1295541793514"></a>中转IP端口</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p9955317133518"><a name="p9955317133518"></a><a name="p9955317133518"></a>中转IP对外提供服务的端口号。端口范围是1～65535。</p>
    <p id="p19551917153512"><a name="p19551917153512"></a><a name="p19551917153512"></a>端口类型为具体端口时，需要配置此参数。</p>
    </td>
    </tr>
    <tr id="row1495521712355"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="p109551917123515"><a name="p109551917123515"></a><a name="p109551917123515"></a>实例类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p79556174353"><a name="p79556174353"></a><a name="p79556174353"></a>选择对外部私网提供服务的<span>实例类型。</span></p>
    <a name="ul595515177355"></a><a name="ul595515177355"></a><ul id="ul595515177355"><li>服务器</li><li>虚拟IP地址</li><li>负载均衡器</li><li>自定义</li></ul>
    </td>
    </tr>
    <tr id="row1295614173357"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="p7956171793517"><a name="p7956171793517"></a><a name="p7956171793517"></a>网卡</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p19569176359"><a name="p19569176359"></a><a name="p19569176359"></a>服务器网卡。实例类型为服务器时，需要配置此参数。</p>
    </td>
    </tr>
    <tr id="row13669928395"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="p3670162193915"><a name="p3670162193915"></a><a name="p3670162193915"></a>IP地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p1267018214394"><a name="p1267018214394"></a><a name="p1267018214394"></a>对外部私网提供服务的云主机IP地址。实例类型为自定义时，需要配置此参数。</p>
    </td>
    </tr>
    <tr id="row19956171783518"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="p14956417103518"><a name="p14956417103518"></a><a name="p14956417103518"></a>业务端口</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p18956191743519"><a name="p18956191743519"></a><a name="p18956191743519"></a>实例对外提供服务的协议端口号。端口范围是1～65535。</p>
    <p id="p1495671713514"><a name="p1495671713514"></a><a name="p1495671713514"></a>端口类型为具体端口时，需要配置此参数。</p>
    </td>
    </tr>
    <tr id="row14956141773510"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="p139567172356"><a name="p139567172356"></a><a name="p139567172356"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p189561517123511"><a name="p189561517123511"></a><a name="p189561517123511"></a>DNAT规则信息描述。最大支持255个字符。</p>
    </td>
    </tr>
    </tbody>
    </table>

5.  配置完成后，单击“确定”，可在DNAT规则列表中查看详情，若“状态”为“运行中”，表示创建成功。

## 相关链接<a name="section341951101415"></a>

[管理DNAT规则](DNAT规则管理-私网NAT网关-34.md)

