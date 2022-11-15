# 添加DNAT规则<a name="zh-cn_topic_0127489530"></a>

## 操作场景<a name="zh-cn_topic_0127293986_section1272311025717"></a>

公网NAT网关创建后，通过添加DNAT规则，则可以通过映射方式将您VPC内的云主机对互联网提供服务。

一个云主机的一个端口对应一条DNAT规则，一个端口只能映射到一个EIP，不能映射到多个EIP。如果您有多个云主机需要为互联网提供服务，则需要创建多条DNAT规则。

## 操作前提<a name="zh-cn_topic_0127293986_section36544171152448"></a>

已成功创建公网NAT网关。

## 操作步骤<a name="zh-cn_topic_0127293986_section61166376152513"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
3.  在系统首页，单击“网络 \> NAT网关”。

    进入公网NAT网关页面。

4.  在公网NAT网关页面，单击需要添加DNAT规则的公网NAT网关名称。
5.  在公网NAT网关详情页面中，单击“DNAT规则”页签。
6.  在DNAT规则页签中，单击“添加DNAT规则”。

    **图 1**  添加DNAT规则<a name="zh-cn_topic_0127293986_fig18104105383315"></a>  
    ![](figures/添加DNAT规则.png "添加DNAT规则")

7.  根据界面提示，配置添加DNAT规则参数，详情请参见[表1](#zh-cn_topic_0127293986_table30787259144637)。

    **表 1**  DNAT规则参数说明

    <a name="zh-cn_topic_0127293986_table30787259144637"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0127293986_row1287982144637"><th class="cellrowborder" valign="top" width="23.189999999999998%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0127293986_p66523784144637"><a name="zh-cn_topic_0127293986_p66523784144637"></a><a name="zh-cn_topic_0127293986_p66523784144637"></a><strong id="zh-cn_topic_0127293986_b64475021144748"><a name="zh-cn_topic_0127293986_b64475021144748"></a><a name="zh-cn_topic_0127293986_b64475021144748"></a>参数</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="76.81%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0127293986_p19717393144637"><a name="zh-cn_topic_0127293986_p19717393144637"></a><a name="zh-cn_topic_0127293986_p19717393144637"></a><strong id="zh-cn_topic_0127293986_b37983896144751"><a name="zh-cn_topic_0127293986_b37983896144751"></a><a name="zh-cn_topic_0127293986_b37983896144751"></a>说明</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0127293986_row20452749101411"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127293986_p930811171516"><a name="zh-cn_topic_0127293986_p930811171516"></a><a name="zh-cn_topic_0127293986_p930811171516"></a>使用场景</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127293986_p82551491578"><a name="zh-cn_topic_0127293986_p82551491578"></a><a name="zh-cn_topic_0127293986_p82551491578"></a>虚拟私有云表示虚拟私有云中的云主机将通过DNAT的方式共享<span id="text1340134883816"><a name="text1340134883816"></a><a name="text1340134883816"></a></span><span id="text1401448193812"><a name="text1401448193812"></a><a name="text1401448193812"></a>弹性公网IP</span>，为公网提供服务。</p>
    <p id="p191738561313"><a name="p191738561313"></a><a name="p191738561313"></a>云专线/云连接表示通过云专线/云连接方式接入虚拟私有云的本地数据中心中的服务器，将通过DNAT的方式为公网提供服务。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0127293986_row1895714384610"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127293986_p11008481568"><a name="zh-cn_topic_0127293986_p11008481568"></a><a name="zh-cn_topic_0127293986_p11008481568"></a>端口类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127293986_p181028481868"><a name="zh-cn_topic_0127293986_p181028481868"></a><a name="zh-cn_topic_0127293986_p181028481868"></a>分为所有端口和具体端口两种类型。</p>
    <a name="ul410617281189"></a><a name="ul410617281189"></a><ul id="ul410617281189"><li>所有端口：属于IP映射方式。此方式相当于为云主机配置了一个<span id="text7583135213818"><a name="text7583135213818"></a><a name="text7583135213818"></a></span><span id="text758385253810"><a name="text758385253810"></a><a name="text758385253810"></a>弹性公网IP</span>，任何访问该<span id="text1638835673813"><a name="text1638835673813"></a><a name="text1638835673813"></a></span><span id="text113889565381"><a name="text113889565381"></a><a name="text113889565381"></a>弹性公网IP</span>的请求都将转发到目标云服务器实例上。</li><li>具体端口：属于端口映射方式。公网NAT网关会将以指定协议和端口访问该<span id="text51056373919"><a name="text51056373919"></a><a name="text51056373919"></a></span><span id="text51064319392"><a name="text51064319392"></a><a name="text51064319392"></a>弹性公网IP</span>的请求转发到目标云主机实例的指定端口上。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0127293986_row13591056167"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127293986_p42842275144637"><a name="zh-cn_topic_0127293986_p42842275144637"></a><a name="zh-cn_topic_0127293986_p42842275144637"></a>支持协议</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127293986_p1747101415356"><a name="zh-cn_topic_0127293986_p1747101415356"></a><a name="zh-cn_topic_0127293986_p1747101415356"></a>协议类型分为TCP和UDP两种类型。端口类型为具体端口时，可配置此参数，端口类型为所有端口时，此参数默认设置为All。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0127293986_row43238809144637"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127293986_p1901342115116"><a name="zh-cn_topic_0127293986_p1901342115116"></a><a name="zh-cn_topic_0127293986_p1901342115116"></a><span id="text437564583717"><a name="text437564583717"></a><a name="text437564583717"></a></span><span id="text1537514450373"><a name="text1537514450373"></a><a name="text1537514450373"></a>弹性公网IP</span></p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127293986_p480029104814"><a name="zh-cn_topic_0127293986_p480029104814"></a><a name="zh-cn_topic_0127293986_p480029104814"></a><span id="text156312165398"><a name="text156312165398"></a><a name="text156312165398"></a></span><span id="text26311516113916"><a name="text26311516113916"></a><a name="text26311516113916"></a>弹性公网IP</span>地址。</p>
    <p id="zh-cn_topic_0127293981_p578114194614"><a name="zh-cn_topic_0127293981_p578114194614"></a><a name="zh-cn_topic_0127293981_p578114194614"></a>这里只能选择没有被绑定的<span id="text14291520113919"><a name="text14291520113919"></a><a name="text14291520113919"></a></span><span id="text9291320143913"><a name="text9291320143913"></a><a name="text9291320143913"></a>弹性公网IP</span>，或者被绑定在当前公网NAT网关中非“所有端口”类型DNAT规则上的<span id="text109331127163919"><a name="text109331127163919"></a><a name="text109331127163919"></a></span><span id="text189331027183914"><a name="text189331027183914"></a><a name="text189331027183914"></a>弹性公网IP</span>，或者被绑定到当前公网NAT网关中SNAT规则上的<span id="text323762373915"><a name="text323762373915"></a><a name="text323762373915"></a></span><span id="text14237102313917"><a name="text14237102313917"></a><a name="text14237102313917"></a>弹性公网IP</span>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0127293986_row189841183384"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127293986_p89861618173810"><a name="zh-cn_topic_0127293986_p89861618173810"></a><a name="zh-cn_topic_0127293986_p89861618173810"></a>公网端口</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p18986618153813"><a name="p18986618153813"></a><a name="p18986618153813"></a><span id="text219573415398"><a name="text219573415398"></a><a name="text219573415398"></a></span><span id="text181951334183917"><a name="text181951334183917"></a><a name="text181951334183917"></a>弹性公网IP</span>的端口。当端口类型为具体端口时，需要配置此参数，有效数值为1-65535。</p>
    <p id="p17852431794"><a name="p17852431794"></a><a name="p17852431794"></a>公网端口的范围可以为具体的数值，也可以为连续的数值范围，例如端口可以为80，也可以为80-100。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0127293986_row35593477144637"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127293986_p64499384144637"><a name="zh-cn_topic_0127293986_p64499384144637"></a><a name="zh-cn_topic_0127293986_p64499384144637"></a>私网IP</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><a name="ul6112191010186"></a><a name="ul6112191010186"></a><ul id="ul6112191010186"><li>当使用场景为虚拟私有云时，指云主机的IP地址。表示此IP地址的云主机将通过DNAT方式为公网提供服务。</li><li>当使用场景为云专线时，指用户本地数据中心中服务器的IP地址或者用户的私有IP地址。表示通过云专线/云连接接入到虚拟私有云的本地数据中心端的此私有IP服务器，可以通过DNAT方式为公网提供服务。<div class="note" id="note2635520513"><a name="note2635520513"></a><a name="note2635520513"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p15631552195114"><a name="p15631552195114"></a><a name="p15631552195114"></a>当使用场景为云专线/云连接时，私网IP还支持虚拟IP。</p>
    </div></div>
    </li><li>端口类型为具体端口时，需要配置私网IP的端口。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0127293986_row1423724123219"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127293986_p1323715410320"><a name="zh-cn_topic_0127293986_p1323715410320"></a><a name="zh-cn_topic_0127293986_p1323715410320"></a>私网端口</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p4994201474513"><a name="p4994201474513"></a><a name="p4994201474513"></a>在使用DNAT为云主机面向公网提供服务场景下，指云主机的端口号。当端口类型为具体端口时，需要配置此参数，有效数值为1-65535。</p>
    <p id="p16418184317411"><a name="p16418184317411"></a><a name="p16418184317411"></a>私网端口的范围可以为具体的数值，也可以为连续的数值范围，例如端口可以为80，也可以为80-100。</p>
    </td>
    </tr>
    <tr id="row1629375132119"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="p12211135512110"><a name="p12211135512110"></a><a name="p12211135512110"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p921111551214"><a name="p921111551214"></a><a name="p921111551214"></a>DNAT规则信息描述。最大支持255个字符。</p>
    </td>
    </tr>
    </tbody>
    </table>

8.  配置完成后，单击“确定”，可在DNAT规则列表中查看详情，若“状态”为“运行中”，表示创建成功。

>![](public_sys-resources/icon-notice.gif) **须知：** 
>配置DNAT规则后，需在对应的云主机中放通对应的安全组规则，否则DNAT规则不能生效。具体操作步骤，请参见[添加安全组规则](https://support.huaweicloud.com/usermanual-vpc/zh-cn_topic_0030969470.html)。

