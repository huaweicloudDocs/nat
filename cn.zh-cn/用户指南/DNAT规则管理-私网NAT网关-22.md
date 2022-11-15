# 购买私网NAT网关<a name="nat_privatenat_0002"></a>

## 操作场景<a name="zh-cn_topic_0201532882_section141051954102215"></a>

如果您的VPC中的资源要通过私网NAT网关访问用户本地数据中心（IDC）或其他虚拟私有云，或面向私网提供服务，则需要购买私网NAT网关。

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   私网NAT网关目前在“华东-上海二”、“西南-贵阳一”、“中国-香港”、“拉美-圣保罗一”、“非洲-约翰内斯堡”、“拉美-墨西哥城一”限时免费。
>-   私网NAT网关目前在“华南-广州-友好用户环境”、“华南-广州”、“华东-上海一”、“华北-北京四”、“华北-乌兰察布一”、“亚太-曼谷”、“亚太-新加坡”已开始计费。

>![](public_sys-resources/icon-caution.gif) **注意：** 
>购买私网NAT网关必须指定私网NAT网关所在VPC、子网、私网NAT网关规格。

## 操作步骤<a name="zh-cn_topic_0201532882_section82633199366"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
3.  在系统首页，单击“网络  \> NAT网关”。

    进入NAT网关页面。

4.  在NAT网关页面，单击“NAT网关\> 私网NAT网关”。
5.  在私网NAT网关页面，单击“购买私网NAT网关”，进入私网NAT网关购买页面。
6.  根据界面提示，配置私网NAT网关的基本信息，配置参数请参见[表1](#table68520404137)。

    **表 1**  参数说明

    <a name="table68520404137"></a>
    <table><thead align="left"><tr id="row178501340161314"><th class="cellrowborder" valign="top" width="31.740000000000002%" id="mcps1.2.3.1.1"><p id="p198502403136"><a name="p198502403136"></a><a name="p198502403136"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="68.26%" id="mcps1.2.3.1.2"><p id="p68502040141319"><a name="p68502040141319"></a><a name="p68502040141319"></a>参数说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row18850164051316"><td class="cellrowborder" valign="top" width="31.740000000000002%" headers="mcps1.2.3.1.1 "><p id="p8850184011136"><a name="p8850184011136"></a><a name="p8850184011136"></a>计费模式</p>
    </td>
    <td class="cellrowborder" valign="top" width="68.26%" headers="mcps1.2.3.1.2 "><p id="p1085064081319"><a name="p1085064081319"></a><a name="p1085064081319"></a>私网NAT网关支持按需计费、包年/包月。</p>
    </td>
    </tr>
    <tr id="row1985017408137"><td class="cellrowborder" valign="top" width="31.740000000000002%" headers="mcps1.2.3.1.1 "><p id="p5850640101316"><a name="p5850640101316"></a><a name="p5850640101316"></a>区域</p>
    </td>
    <td class="cellrowborder" valign="top" width="68.26%" headers="mcps1.2.3.1.2 "><p id="p1985014014135"><a name="p1985014014135"></a><a name="p1985014014135"></a>私网NAT网关所在的区域。</p>
    </td>
    </tr>
    <tr id="row58511140191316"><td class="cellrowborder" valign="top" width="31.740000000000002%" headers="mcps1.2.3.1.1 "><p id="p485074021317"><a name="p485074021317"></a><a name="p485074021317"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="68.26%" headers="mcps1.2.3.1.2 "><p id="p12851154017136"><a name="p12851154017136"></a><a name="p12851154017136"></a>私网NAT网关名称。最大支持64个字符，仅支持中文、数字、字母、_（下划线）、-（中划线）。</p>
    </td>
    </tr>
    <tr id="row1851740141310"><td class="cellrowborder" valign="top" width="31.740000000000002%" headers="mcps1.2.3.1.1 "><p id="p14851124015132"><a name="p14851124015132"></a><a name="p14851124015132"></a>虚拟私有云</p>
    </td>
    <td class="cellrowborder" valign="top" width="68.26%" headers="mcps1.2.3.1.2 "><p id="p3851104091320"><a name="p3851104091320"></a><a name="p3851104091320"></a>私网NAT网关所属的VPC。</p>
    <p id="p585115405137"><a name="p585115405137"></a><a name="p585115405137"></a>VPC仅在<span id="ph1889041824413"><a name="ph1889041824413"></a><a name="ph1889041824413"></a>购买</span>私网NAT网关时可以选择，后续不支持修改。</p>
    </td>
    </tr>
    <tr id="row1485114401135"><td class="cellrowborder" valign="top" width="31.740000000000002%" headers="mcps1.2.3.1.1 "><p id="p18851164061311"><a name="p18851164061311"></a><a name="p18851164061311"></a>子网</p>
    </td>
    <td class="cellrowborder" valign="top" width="68.26%" headers="mcps1.2.3.1.2 "><p id="p2851194019138"><a name="p2851194019138"></a><a name="p2851194019138"></a>私网NAT网关所属VPC中的子网。</p>
    <p id="p385120401136"><a name="p385120401136"></a><a name="p385120401136"></a>子网至少有一个可用的IP地址。</p>
    <p id="p68516407136"><a name="p68516407136"></a><a name="p68516407136"></a>子网仅在<span id="ph375011258444"><a name="ph375011258444"></a><a name="ph375011258444"></a>购买</span>私网NAT网关时可以选择，后续不支持修改。</p>
    </td>
    </tr>
    <tr id="row11851164013137"><td class="cellrowborder" valign="top" width="31.740000000000002%" headers="mcps1.2.3.1.1 "><p id="p158514409133"><a name="p158514409133"></a><a name="p158514409133"></a>规格</p>
    </td>
    <td class="cellrowborder" valign="top" width="68.26%" headers="mcps1.2.3.1.2 "><p id="p48513403135"><a name="p48513403135"></a><a name="p48513403135"></a>私网NAT网关的规格。</p>
    <p id="p485114017136"><a name="p485114017136"></a><a name="p485114017136"></a>私网NAT网关共有小型、中型、大型和超大型四种规格类型。规格详情参见<a href="https://support.huaweicloud.com/productdesc-natgateway/zh-cn_topic_0086739763.html" target="_blank" rel="noopener noreferrer">产品规格</a>。</p>
    </td>
    </tr>
    <tr id="row785124041316"><td class="cellrowborder" valign="top" width="31.740000000000002%" headers="mcps1.2.3.1.1 "><p id="p1285184011136"><a name="p1285184011136"></a><a name="p1285184011136"></a>企业项目</p>
    </td>
    <td class="cellrowborder" valign="top" width="68.26%" headers="mcps1.2.3.1.2 "><p id="p208511440151319"><a name="p208511440151319"></a><a name="p208511440151319"></a>配置私网NAT网关归属的企业项目。当私网NAT网关配置企业项目时，该私网NAT网关将归属于该企业项目。</p>
    <p id="p104711735163613"><a name="p104711735163613"></a><a name="p104711735163613"></a>当没有指定企业项目时，将默认使用项目名称为default的企业项目。</p>
    </td>
    </tr>
    <tr id="row68521040171318"><td class="cellrowborder" valign="top" width="31.740000000000002%" headers="mcps1.2.3.1.1 "><p id="p58517406134"><a name="p58517406134"></a><a name="p58517406134"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="68.26%" headers="mcps1.2.3.1.2 "><p id="p18521440181312"><a name="p18521440181312"></a><a name="p18521440181312"></a>私网NAT网关信息描述。最大支持255个字符。</p>
    </td>
    </tr>
    </tbody>
    </table>

7.  单击“立即购买”。

## 相关链接<a name="section341951101415"></a>

[管理私网NAT网关](DNAT规则管理-私网NAT网关-26.md)

