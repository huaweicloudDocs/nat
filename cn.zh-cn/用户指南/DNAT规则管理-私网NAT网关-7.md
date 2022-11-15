# 添加SNAT规则<a name="zh-cn_topic_0127489529"></a>

## 操作场景<a name="zh-cn_topic_0127293981_section18103401105119"></a>

公网NAT网关创建成功后，您需要创建SNAT规则。通过创建SNAT规则，虚拟私有云子网中全部或部分云主机可以通过共享弹性公网IP访问公网，或云专线/云连接用户侧端该网段下的服务器可以通过共享弹性公网IP访问公网。

一个子网对应一条SNAT规则，如果VPC中有多个子网需要访问公网，则可以通过创建多个SNAT规则实现共享一个或多个弹性公网IP资源。

## 前提条件<a name="zh-cn_topic_0127293981_section27241609"></a>

-   公网NAT网关创建成功。
-   云专线接入的用户，云专线的虚拟网关中，“VPC网段”参数建议设置为"0.0.0.0/0"。具体配置请参考[创建虚拟网关](https://support.huaweicloud.com/qs-dc/dc_03_0004.html)。

## 操作步骤<a name="zh-cn_topic_0127293981_section43847892"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region-0.png)图标，选择区域和项目。
3.  在系统首页，单击“网络 \> NAT网关”。

    进入公网NAT网关页面。

4.  在公网NAT网关页面，单击需要添加SNAT规则的公网NAT网关名称。
5.  在SNAT规则页签中，单击“添加SNAT规则”。

    **图 1**  添加SNAT规则<a name="fig1199611814445"></a>  
    ![](figures/添加SNAT规则.png "添加SNAT规则")

6.  根据界面提示，配置添加SNAT规则参数，详情请参见[表1](#zh-cn_topic_0127293981_table4272024117597)。

    **表 1**  SNAT规则参数说明

    <a name="zh-cn_topic_0127293981_table4272024117597"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0127293981_row3248015417597"><th class="cellrowborder" valign="top" width="26.0674482558981%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0127293981_p1364683317597"><a name="zh-cn_topic_0127293981_p1364683317597"></a><a name="zh-cn_topic_0127293981_p1364683317597"></a><strong id="zh-cn_topic_0127293981_b24166891144739"><a name="zh-cn_topic_0127293981_b24166891144739"></a><a name="zh-cn_topic_0127293981_b24166891144739"></a>参数</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="73.93255174410189%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0127293981_p1643000117597"><a name="zh-cn_topic_0127293981_p1643000117597"></a><a name="zh-cn_topic_0127293981_p1643000117597"></a><strong id="zh-cn_topic_0127293981_b1365228517597"><a name="zh-cn_topic_0127293981_b1365228517597"></a><a name="zh-cn_topic_0127293981_b1365228517597"></a>说明</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0127293981_row144002379410"><td class="cellrowborder" valign="top" width="26.0674482558981%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127293981_p2400173718417"><a name="zh-cn_topic_0127293981_p2400173718417"></a><a name="zh-cn_topic_0127293981_p2400173718417"></a>使用场景</p>
    </td>
    <td class="cellrowborder" valign="top" width="73.93255174410189%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127293981_p4400123718411"><a name="zh-cn_topic_0127293981_p4400123718411"></a><a name="zh-cn_topic_0127293981_p4400123718411"></a>SNAT规则使用的场景。</p>
    <p id="p51852719278"><a name="p51852719278"></a><a name="p51852719278"></a>当虚拟私有云中的云主机需要访问公网时，选择虚拟私有云。</p>
    <p id="p21892752716"><a name="p21892752716"></a><a name="p21892752716"></a>当云专线/VPN本地数据中心端的服务器需要访问公网时，选择云专线/云连接。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0127293981_row3209331417597"><td class="cellrowborder" valign="top" width="26.0674482558981%" headers="mcps1.2.3.1.1 "><p id="p206671421164"><a name="p206671421164"></a><a name="p206671421164"></a>子网</p>
    </td>
    <td class="cellrowborder" valign="top" width="73.93255174410189%" headers="mcps1.2.3.1.2 "><a name="ul1779741412317"></a><a name="ul1779741412317"></a><ul id="ul1779741412317"><li>使用已有：选择现有子网，使云服务器通过SNAT方式访问公网。</li><li>自定义：自定义一个网段或者填写某个主机地址，使云服务器通过SNAT方式访问公网。<div class="note" id="note1725213854717"><a name="note1725213854717"></a><a name="note1725213854717"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p16265625171016"><a name="p16265625171016"></a><a name="p16265625171016"></a>支持配置0.0.0.0/0的地址段，在多段地址配置时更方便。</p>
    <p id="p13252484473"><a name="p13252484473"></a><a name="p13252484473"></a>可以配置32位主机地址，NAT网关只针对此地址起作用。</p>
    </div></div>
    </li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0127293981_row5801532217597"><td class="cellrowborder" valign="top" width="26.0674482558981%" headers="mcps1.2.3.1.1 "><p id="p02871145345"><a name="p02871145345"></a><a name="p02871145345"></a><span id="text437564583717"><a name="text437564583717"></a><a name="text437564583717"></a></span><span id="text1537514450373"><a name="text1537514450373"></a><a name="text1537514450373"></a>弹性公网IP</span></p>
    </td>
    <td class="cellrowborder" valign="top" width="73.93255174410189%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127293981_p94462428451"><a name="zh-cn_topic_0127293981_p94462428451"></a><a name="zh-cn_topic_0127293981_p94462428451"></a>用来提供互联网访问的公网IP。</p>
    <p id="zh-cn_topic_0127293981_p578114194614"><a name="zh-cn_topic_0127293981_p578114194614"></a><a name="zh-cn_topic_0127293981_p578114194614"></a>这里只能选择没有被绑定的<span id="text5848135683711"><a name="text5848135683711"></a><a name="text5848135683711"></a></span><span id="text178481256203710"><a name="text178481256203710"></a><a name="text178481256203710"></a>弹性公网IP</span>，或者被绑定在当前公网NAT网关中非“所有端口”类型DNAT规则上的<span id="text57201823812"><a name="text57201823812"></a><a name="text57201823812"></a></span><span id="text2720988384"><a name="text2720988384"></a><a name="text2720988384"></a>弹性公网IP</span>，或者被绑定到当前公网NAT网关中SNAT规则上的<span id="text3122181903812"><a name="text3122181903812"></a><a name="text3122181903812"></a></span><span id="text10122141983819"><a name="text10122141983819"></a><a name="text10122141983819"></a>弹性公网IP</span>。</p>
    <p id="p1270810226152"><a name="p1270810226152"></a><a name="p1270810226152"></a>可选择多条EIP添加在SNAT规则中。一条SNAT规则最多添加20个EIP。SNAT规则使用多个EIP时，业务运行时会随机选取其中的一个。</p>
    </td>
    </tr>
    <tr id="row182413199575"><td class="cellrowborder" valign="top" width="26.0674482558981%" headers="mcps1.2.3.1.1 "><p id="p8824161914573"><a name="p8824161914573"></a><a name="p8824161914573"></a>监控</p>
    </td>
    <td class="cellrowborder" valign="top" width="73.93255174410189%" headers="mcps1.2.3.1.2 "><p id="p5825319145715"><a name="p5825319145715"></a><a name="p5825319145715"></a><span>为SNAT连接数</span>设置告警。</p>
    <p id="p1542202115919"><a name="p1542202115919"></a><a name="p1542202115919"></a><span>可通过设置告警及时了解SNAT连接数运行状况，从而起到预警作用。</span></p>
    </td>
    </tr>
    <tr id="row153111641748"><td class="cellrowborder" valign="top" width="26.0674482558981%" headers="mcps1.2.3.1.1 "><p id="p5274235692544"><a name="p5274235692544"></a><a name="p5274235692544"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="73.93255174410189%" headers="mcps1.2.3.1.2 "><p id="p4427248192544"><a name="p4427248192544"></a><a name="p4427248192544"></a>SNAT规则信息描述。最大支持255个字符。</p>
    </td>
    </tr>
    </tbody>
    </table>

7.  配置完成后，单击确定，完成“SNAT规则”创建。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >-   根据您的业务需求，可以为一个公网NAT网关添加多条SNAT规则。
    >-   一个VPC支持关联多个公网NAT网关。
    >-   VPC内的每个子网只能添加一条SNAT规则。


