# 创建中转子网和中转IP<a name="nat_privatenatexsub_0001_"></a>

## 操作场景<a name="zh-cn_topic_0127293981_section18103401105119"></a>

私网NAT网关创建成功后，您需要创建中转子网与中转IP。

通过创建中转子网与中转IP，使虚拟私有云内多个云主机可以共享中转IP访问用户本地数据中心（IDC）或其他虚拟私有云，或面向私网提供服务。

## 前提条件<a name="zh-cn_topic_0127293981_section27241609"></a>

-   中转VPC创建成功。
-   云专线接入的用户，云专线的虚拟网关中，“VPC网段”参数建议设置为"0.0.0.0/0"。具体配置请参考[创建虚拟网关](https://support.huaweicloud.com/qs-dc/dc_03_0004.html)。

## 操作步骤<a name="section1712319445577"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
3.  在系统首页，单击“网络  \> NAT网关”。

    进入NAT网关页面。

4.  在NAT网关页面，单击“NAT网关\> 私网NAT网关”。
5.  在“中转子网”页签中，单击“创建中转子网”。
6.  根据界面提示，配置中转子网参数，详情请参见[表1](#table12551133922418)。

    **图 1**  创建中转子网<a name="fig888518254285"></a>  
    ![](figures/创建中转子网.png "创建中转子网")

    **表 1**  中转子网参数说明

    <a name="table12551133922418"></a>
    <table><thead align="left"><tr id="row1654919390247"><th class="cellrowborder" valign="top" width="23.189999999999998%" id="mcps1.2.3.1.1"><p id="p1154953982415"><a name="p1154953982415"></a><a name="p1154953982415"></a><strong id="b65491039102420"><a name="b65491039102420"></a><a name="b65491039102420"></a>参数</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="76.81%" id="mcps1.2.3.1.2"><p id="p254903912244"><a name="p254903912244"></a><a name="p254903912244"></a><strong id="b17549153917241"><a name="b17549153917241"></a><a name="b17549153917241"></a>说明</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row165490391243"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="p8549143972416"><a name="p8549143972416"></a><a name="p8549143972416"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p8549163992412"><a name="p8549163992412"></a><a name="p8549163992412"></a>中转子网名称。最大支持64个字符，仅支持中文、数字、字母、_（下划线）、-（中划线）。该参数为必填项。</p>
    </td>
    </tr>
    <tr id="row18550939162415"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="p1954915393242"><a name="p1954915393242"></a><a name="p1954915393242"></a>虚拟私有云</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p455003922410"><a name="p455003922410"></a><a name="p455003922410"></a>中转子网所属的VPC。该参数为选填项。</p>
    </td>
    </tr>
    <tr id="row1555043972420"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="p10550139162417"><a name="p10550139162417"></a><a name="p10550139162417"></a>子网</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p6550113913243"><a name="p6550113913243"></a><a name="p6550113913243"></a>中转子网所在子网。该参数为选填项。</p>
    </td>
    </tr>
    <tr id="row185511439132411"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="p855143942417"><a name="p855143942417"></a><a name="p855143942417"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p355114392249"><a name="p355114392249"></a><a name="p355114392249"></a>中转子网信息描述。最大支持255个字符。该参数为选填项。</p>
    </td>
    </tr>
    </tbody>
    </table>

7.  单击“确定”，完成中转子网创建。
8.  单击目标中转子网名称。

    进入中转子网详情页。

9.  单击“创建中转IP”，根据界面提示，配置中转IP参数。

    **图 2**  创建中转IP<a name="fig138971775302"></a>  
    ![](figures/创建中转IP.png "创建中转IP")

    **表 2**  中转IP参数说明

    <a name="table432418475297"></a>
    <table><thead align="left"><tr id="row133204479299"><th class="cellrowborder" valign="top" width="23.189999999999998%" id="mcps1.2.3.1.1"><p id="p1231915473298"><a name="p1231915473298"></a><a name="p1231915473298"></a><strong id="b131934742916"><a name="b131934742916"></a><a name="b131934742916"></a>参数</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="76.81%" id="mcps1.2.3.1.2"><p id="p11320194716290"><a name="p11320194716290"></a><a name="p11320194716290"></a><strong id="b2320124722916"><a name="b2320124722916"></a><a name="b2320124722916"></a>说明</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row532444732915"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="p14320174713292"><a name="p14320174713292"></a><a name="p14320174713292"></a>分配方式</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p132254772917"><a name="p132254772917"></a><a name="p132254772917"></a>中转IP的分配方式。</p>
    <a name="ul15324147122918"></a><a name="ul15324147122918"></a><ul id="ul15324147122918"><li>自动分配</li><li>手动分配</li></ul>
    </td>
    </tr>
    <tr id="row1132484772914"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="p19324164720290"><a name="p19324164720290"></a><a name="p19324164720290"></a>IP地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p1632413471290"><a name="p1632413471290"></a><a name="p1632413471290"></a>分配方式为手动分配时，需要填写。此IP地址需包含在中转子网网段内。</p>
    </td>
    </tr>
    </tbody>
    </table>

10. 单击“确定”，完成中转IP创建。

## 相关链接<a name="section341951101415"></a>

[管理中转子网](DNAT规则管理-私网NAT网关-38.md)

