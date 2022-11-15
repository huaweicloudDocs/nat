# 创建中转IP<a name="nat_exip_0001"></a>

## 操作场景<a name="section5439354114616"></a>

通过创建中转子网与中转IP，使虚拟私有云内多个云主机可以共享中转IP访问用户本地数据中心（IDC）或其他虚拟私有云，或面向私网提供服务。

## 操作步骤<a name="section2533151214536"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
3.  在系统首页，单击“网络  \> NAT网关”。

    进入NAT网关页面。

4.  在NAT网关页面，单击“NAT网关\> 私网NAT网关”。
5.  在“中转子网”页签中，单击目标中转子网名称。

    进入中转子网详情页。

6.  单击“创建中转IP”，根据界面提示，配置中转子网参数。

    **表 1**  中转IP参数说明

    <a name="table19797726185310"></a>
    <table><thead align="left"><tr id="row147981026125315"><th class="cellrowborder" valign="top" width="23.189999999999998%" id="mcps1.2.3.1.1"><p id="p1379832615534"><a name="p1379832615534"></a><a name="p1379832615534"></a><strong id="b479813262539"><a name="b479813262539"></a><a name="b479813262539"></a>参数</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="76.81%" id="mcps1.2.3.1.2"><p id="p1079882695310"><a name="p1079882695310"></a><a name="p1079882695310"></a><strong id="b8798026195311"><a name="b8798026195311"></a><a name="b8798026195311"></a>说明</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1179832613535"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="p14798192665310"><a name="p14798192665310"></a><a name="p14798192665310"></a>分配方式</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p810815171783"><a name="p810815171783"></a><a name="p810815171783"></a>中转IP的分配方式。</p>
    <a name="ul1520272010813"></a><a name="ul1520272010813"></a><ul id="ul1520272010813"><li>自动分配</li><li>手动分配</li></ul>
    </td>
    </tr>
    <tr id="row2798142616536"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="p14798626115310"><a name="p14798626115310"></a><a name="p14798626115310"></a>IP地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p1079892665319"><a name="p1079892665319"></a><a name="p1079892665319"></a>分配方式为手动分配时，需要填写。此IP地址需包含在中转子网网段内。</p>
    </td>
    </tr>
    </tbody>
    </table>


