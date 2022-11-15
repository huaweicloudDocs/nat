# DNAT规则模板导入导出<a name="nat_dnat_0005"></a>

## 操作场景<a name="zh-cn_topic_0127293986_section1272311025717"></a>

公网NAT网关创建后，通过添加DNAT规则，则可以通过映射方式将您VPC内的云主机对互联网提供服务。

一个云主机绑定一条DNAT规则，如果您有多个云主机需要为互联网提供服务，则需要创建多条DNAT规则。

## 操作前提<a name="zh-cn_topic_0127293986_section36544171152448"></a>

已成功创建公网NAT网关。

## 操作步骤<a name="section1921525118506"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
3.  在系统首页，单击“网络 \> NAT网关”。

    进入公网NAT网关页面。

4.  在公网NAT网关页面，单击需要添加DNAT规则的公网NAT网关名称。
5.  在公网NAT网关详情页面中，单击“DNAT规则”页签。
6.  在DNAT规则页签中，单击“导入DNAT规则列表”，下载模板。
7.  根据模板中的表头，填写DNAT规则参数，详情请参见[表1](#zh-cn_topic_0127293986_table30787259144637)。

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
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p287045720270"><a name="p287045720270"></a><a name="p287045720270"></a>分为<strong id="b08312054172816"><a name="b08312054172816"></a><a name="b08312054172816"></a>虚拟私有云</strong>和<strong id="b1968859142811"><a name="b1968859142811"></a><a name="b1968859142811"></a>云专线/云连接</strong>两种方式。</p>
    <a name="ul138052045192814"></a><a name="ul138052045192814"></a><ul id="ul138052045192814"><li>虚拟私有云：表示虚拟私有云中的云主机将通过DNAT的方式共享弹性公网IP，为公网提供服务。</li><li>云专线/云连接：表示通过云专线/云连接方式接入虚拟私有云的本地数据中心中的服务器，将通过DNAT的方式为公网提供服务。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0127293986_row13591056167"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127293986_p42842275144637"><a name="zh-cn_topic_0127293986_p42842275144637"></a><a name="zh-cn_topic_0127293986_p42842275144637"></a>支持协议</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127293986_p1747101415356"><a name="zh-cn_topic_0127293986_p1747101415356"></a><a name="zh-cn_topic_0127293986_p1747101415356"></a>协议类型分为TCP、UDP、全部三种类型。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0127293986_row43238809144637"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127293986_p1448715913116"><a name="zh-cn_topic_0127293986_p1448715913116"></a><a name="zh-cn_topic_0127293986_p1448715913116"></a></p>
    <p id="zh-cn_topic_0127293986_p1901342115116"><a name="zh-cn_topic_0127293986_p1901342115116"></a><a name="zh-cn_topic_0127293986_p1901342115116"></a>弹性公网IP</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127293986_p480029104814"><a name="zh-cn_topic_0127293986_p480029104814"></a><a name="zh-cn_topic_0127293986_p480029104814"></a>弹性公网IP地址及公网端口。</p>
    <p id="zh-cn_topic_0127293986_p20658758144637"><a name="zh-cn_topic_0127293986_p20658758144637"></a><a name="zh-cn_topic_0127293986_p20658758144637"></a>只能使用未绑定的弹性公网IP或者被绑定在当前VPC中DNAT规则上的弹性公网IP。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0127293986_row189841183384"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127293986_p89861618173810"><a name="zh-cn_topic_0127293986_p89861618173810"></a><a name="zh-cn_topic_0127293986_p89861618173810"></a>公网端口</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127293986_p18986618153813"><a name="zh-cn_topic_0127293986_p18986618153813"></a><a name="zh-cn_topic_0127293986_p18986618153813"></a>弹性公网IP的端口。当端口类型为“全部”时，不需要配置此参数。</p>
    <p id="zh-cn_topic_0127293986_p17852431794"><a name="zh-cn_topic_0127293986_p17852431794"></a><a name="zh-cn_topic_0127293986_p17852431794"></a>公网端口的范围可以为具体的数值，也可以为连续的数值范围，例如端口可以为80，也可以为80-100。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0127293986_row35593477144637"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127293986_p64499384144637"><a name="zh-cn_topic_0127293986_p64499384144637"></a><a name="zh-cn_topic_0127293986_p64499384144637"></a>私网IP</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><a name="ul6112191010186"></a><a name="ul6112191010186"></a><ul id="ul6112191010186"><li>当使用场景为虚拟私有云时，指云主机的IP地址。表示此IP地址的云主机将通过DNAT方式为公网提供服务。</li><li>当使用场景为云专线时，指用户本地数据中心中服务器的IP地址或者用户的私有IP地址。表示通过云专线/云连接接入到虚拟私有云的本地数据中心端的此私有IP服务器，可以通过DNAT方式为公网提供服务。</li><li>协议类型为TCP、UDP时，需要配置私网IP的端口。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0127293986_row1423724123219"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127293986_p1323715410320"><a name="zh-cn_topic_0127293986_p1323715410320"></a><a name="zh-cn_topic_0127293986_p1323715410320"></a>私网端口</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><a name="ul15695431162419"></a><a name="ul15695431162419"></a><ul id="ul15695431162419"><li>当使用场景为虚拟私有云时，指云主机的端口号。</li><li>当使用场景为云专线时，指用户本地数据中心中服务器的端口号或私有端口号。</li><li>端口类型为“全部”时，不需要配置此参数。</li></ul>
    <p id="zh-cn_topic_0127293986_p625264114344"><a name="zh-cn_topic_0127293986_p625264114344"></a><a name="zh-cn_topic_0127293986_p625264114344"></a>私网端口需要与对应弹性公网IP的公网端口数量保持一致。</p>
    </td>
    </tr>
    <tr id="row13465726183310"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="p7465172643315"><a name="p7465172643315"></a><a name="p7465172643315"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p946592619337"><a name="p946592619337"></a><a name="p946592619337"></a>DNAT规则信息描述。最大支持255个字符。</p>
    </td>
    </tr>
    </tbody>
    </table>

8.  模板填写完后，单击“导入DNAT规则列表”图标，选择本地模板，单击“导入”。

    **图 1**  导入DNAT规则模板<a name="fig17585101045413"></a>  
    ![](figures/导入DNAT规则模板.png "导入DNAT规则模板")

9.  可在DNAT规则列表中查看详情，若“状态”为“运行中”，表示创建成功。
10. 在DNAT规则页签中，单击“导出DNAT规则列表”，可导出已配置好的DNAT规则模板。

