# 购买公网NAT网关<a name="zh-cn_topic_0150270259"></a>

## 操作场景<a name="zh-cn_topic_0201532882_section141051954102215"></a>

如果您要通过公网NAT网关访问公网或为公网提供服务，则需要购买公网NAT网关。

## 前提条件<a name="zh-cn_topic_0201532882_section1825861973713"></a>

-   购买公网NAT网关必须指定公网NAT网关所在VPC、子网。
-   由于需要放通到公网NAT网关的流量，即在VPC中需要有指向公网NAT网关的路由，因此在购买公网NAT网关时，会自动在VPC的默认路由表中添加一条0.0.0.0/0的默认路由指向所购买的公网NAT网关。如果在购买公网NAT网关前，VPC默认路由表下已经存在0.0.0.0/0的默认路由，则会导致自动添加该默认路由指向公网NAT网关失败，此时需要在公网NAT网关购买成功后，手动为此网关添加一条不同的路由或在新路由表中创建0.0.0.0/0的默认路由指向该网关。

## 操作步骤<a name="zh-cn_topic_0201532882_section82633199366"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
3.  在系统首页，单击“网络 \> NAT网关”。

    进入公网NAT网关页面。

4.  在公网NAT网关页面，单击“购买公网NAT网关”，进入公网NAT网关购买页面。
5.  根据界面提示，配置公网NAT网关的基本信息，配置参数请参见[表1](#zh-cn_topic_0259133770_table27487005195751)。

    **表 1**  参数说明

    <a name="zh-cn_topic_0259133770_table27487005195751"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0259133770_row9940336195751"><th class="cellrowborder" valign="top" width="31.740000000000002%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0259133770_p5995559819588"><a name="zh-cn_topic_0259133770_p5995559819588"></a><a name="zh-cn_topic_0259133770_p5995559819588"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="68.26%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0259133770_p2456526519588"><a name="zh-cn_topic_0259133770_p2456526519588"></a><a name="zh-cn_topic_0259133770_p2456526519588"></a>参数说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0259133770_row23152322195751"><td class="cellrowborder" valign="top" width="31.740000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0259133770_p6699528015250"><a name="zh-cn_topic_0259133770_p6699528015250"></a><a name="zh-cn_topic_0259133770_p6699528015250"></a>计费模式</p>
    </td>
    <td class="cellrowborder" valign="top" width="68.26%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0259133770_p6600326015310"><a name="zh-cn_topic_0259133770_p6600326015310"></a><a name="zh-cn_topic_0259133770_p6600326015310"></a>公网NAT网关支持按需计费、包年/包月。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0259133770_row93821753517"><td class="cellrowborder" valign="top" width="31.740000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0259133770_p22912486162048"><a name="zh-cn_topic_0259133770_p22912486162048"></a><a name="zh-cn_topic_0259133770_p22912486162048"></a>区域</p>
    </td>
    <td class="cellrowborder" valign="top" width="68.26%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0259133770_p43972101162048"><a name="zh-cn_topic_0259133770_p43972101162048"></a><a name="zh-cn_topic_0259133770_p43972101162048"></a>公网NAT网关所在的区域。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0259133770_row32613315195751"><td class="cellrowborder" valign="top" width="31.740000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0259133770_p2832836319588"><a name="zh-cn_topic_0259133770_p2832836319588"></a><a name="zh-cn_topic_0259133770_p2832836319588"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="68.26%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0259133770_p1289605119588"><a name="zh-cn_topic_0259133770_p1289605119588"></a><a name="zh-cn_topic_0259133770_p1289605119588"></a>公网NAT网关名称。最大支持64个字符，仅支持数字、字母、_（下划线）、-（中划线）。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0259133770_row27553870195751"><td class="cellrowborder" valign="top" width="31.740000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0259133770_p1464780019588"><a name="zh-cn_topic_0259133770_p1464780019588"></a><a name="zh-cn_topic_0259133770_p1464780019588"></a>虚拟私有云</p>
    </td>
    <td class="cellrowborder" valign="top" width="68.26%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0259133770_p4562116519588"><a name="zh-cn_topic_0259133770_p4562116519588"></a><a name="zh-cn_topic_0259133770_p4562116519588"></a>公网NAT网关所属的VPC。</p>
    <p id="zh-cn_topic_0259133770_p13668174021018"><a name="zh-cn_topic_0259133770_p13668174021018"></a><a name="zh-cn_topic_0259133770_p13668174021018"></a>VPC仅在<span id="zh-cn_topic_0259133770_ph61101713113716"><a name="zh-cn_topic_0259133770_ph61101713113716"></a><a name="zh-cn_topic_0259133770_ph61101713113716"></a>购买</span>公网NAT网关时可以选择，后续不支持修改。</p>
    <div class="note" id="zh-cn_topic_0259133770_note1378963764012"><a name="zh-cn_topic_0259133770_note1378963764012"></a><a name="zh-cn_topic_0259133770_note1378963764012"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0259133770_p279033714015"><a name="zh-cn_topic_0259133770_p279033714015"></a><a name="zh-cn_topic_0259133770_p279033714015"></a>由于需要放通到公网NAT网关的流量，即在VPC中需要有指向公网NAT网关的路由，因此在<span id="zh-cn_topic_0259133770_ph195554115432"><a name="zh-cn_topic_0259133770_ph195554115432"></a><a name="zh-cn_topic_0259133770_ph195554115432"></a>购买</span>公网NAT网关时，会自动在VPC的默认路由表中添加一条0.0.0.0/0的默认路由指向所<span id="zh-cn_topic_0259133770_ph1455531120438"><a name="zh-cn_topic_0259133770_ph1455531120438"></a><a name="zh-cn_topic_0259133770_ph1455531120438"></a>购买</span>的公网NAT网关。如果在<span id="zh-cn_topic_0259133770_ph455541164313"><a name="zh-cn_topic_0259133770_ph455541164313"></a><a name="zh-cn_topic_0259133770_ph455541164313"></a>购买</span>公网NAT网关前，VPC默认路由表下已经存在0.0.0.0/0的默认路由，则会导致自动添加该默认路由指向公网NAT网关失败，此时需要在公网NAT网关<span id="zh-cn_topic_0259133770_ph1755614111436"><a name="zh-cn_topic_0259133770_ph1755614111436"></a><a name="zh-cn_topic_0259133770_ph1755614111436"></a>购买</span>成功后，手动为此网关添加一条不同的路由或在新路由表中创建0.0.0.0/0的默认路由指向该网关。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0259133770_row47407746195751"><td class="cellrowborder" valign="top" width="31.740000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0259133770_p17196519588"><a name="zh-cn_topic_0259133770_p17196519588"></a><a name="zh-cn_topic_0259133770_p17196519588"></a>子网</p>
    </td>
    <td class="cellrowborder" valign="top" width="68.26%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0259133770_p980412105420"><a name="zh-cn_topic_0259133770_p980412105420"></a><a name="zh-cn_topic_0259133770_p980412105420"></a>公网NAT网关所属VPC中的子网。</p>
    <p id="zh-cn_topic_0259133770_p1392917619588"><a name="zh-cn_topic_0259133770_p1392917619588"></a><a name="zh-cn_topic_0259133770_p1392917619588"></a>子网至少有一个可用的IP地址。</p>
    <p id="zh-cn_topic_0259133770_p14481165611919"><a name="zh-cn_topic_0259133770_p14481165611919"></a><a name="zh-cn_topic_0259133770_p14481165611919"></a>子网仅在<span id="zh-cn_topic_0259133770_ph195511118133714"><a name="zh-cn_topic_0259133770_ph195511118133714"></a><a name="zh-cn_topic_0259133770_ph195511118133714"></a>购买</span>公网NAT网关时可以选择，后续不支持修改。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0259133770_row3011590195751"><td class="cellrowborder" valign="top" width="31.740000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0259133770_p1770884719588"><a name="zh-cn_topic_0259133770_p1770884719588"></a><a name="zh-cn_topic_0259133770_p1770884719588"></a>规格</p>
    </td>
    <td class="cellrowborder" valign="top" width="68.26%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0259133770_p156313256519"><a name="zh-cn_topic_0259133770_p156313256519"></a><a name="zh-cn_topic_0259133770_p156313256519"></a>公网NAT网关的规格。</p>
    <p id="zh-cn_topic_0259133770_p03201316191210"><a name="zh-cn_topic_0259133770_p03201316191210"></a><a name="zh-cn_topic_0259133770_p03201316191210"></a>公网NAT网关共有小型、中型、大型和超大型四种规格类型，可通过“了解更多”查看各规格详情。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0259133770_row98721653013"><td class="cellrowborder" valign="top" width="31.740000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0259133770_p58721651500"><a name="zh-cn_topic_0259133770_p58721651500"></a><a name="zh-cn_topic_0259133770_p58721651500"></a>企业项目</p>
    </td>
    <td class="cellrowborder" valign="top" width="68.26%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0259133770_p187218519019"><a name="zh-cn_topic_0259133770_p187218519019"></a><a name="zh-cn_topic_0259133770_p187218519019"></a>配置公网NAT网关归属的企业项目。当公网NAT网关配置企业项目时，该公网NAT网关将归属于该企业项目。当没有指定企业项目时，将默认使用项目名称为default的企业项目。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0259133770_row2219225792544"><td class="cellrowborder" valign="top" width="31.740000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0259133770_p5274235692544"><a name="zh-cn_topic_0259133770_p5274235692544"></a><a name="zh-cn_topic_0259133770_p5274235692544"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="68.26%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0259133770_p4427248192544"><a name="zh-cn_topic_0259133770_p4427248192544"></a><a name="zh-cn_topic_0259133770_p4427248192544"></a>公网NAT网关信息描述。最大支持255个字符。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0259133770_row29995813516"><td class="cellrowborder" valign="top" width="31.740000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0259133770_p119916585518"><a name="zh-cn_topic_0259133770_p119916585518"></a><a name="zh-cn_topic_0259133770_p119916585518"></a>标签</p>
    </td>
    <td class="cellrowborder" valign="top" width="68.26%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_p20140951169"><a name="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_p20140951169"></a><a name="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_p20140951169"></a>公网NAT网关的标识，包括键和值。可以创建10个标签。</p>
    <p id="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_p39052702211138"><a name="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_p39052702211138"></a><a name="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_p39052702211138"></a>标签的命名规则请参考<a href="#zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_table248245914136">表2</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0259133770_row105571852134014"><td class="cellrowborder" valign="top" width="31.740000000000002%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0259133770_p1955835204015"><a name="zh-cn_topic_0259133770_p1955835204015"></a><a name="zh-cn_topic_0259133770_p1955835204015"></a>购买时长</p>
    </td>
    <td class="cellrowborder" valign="top" width="68.26%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0259133770_p185581652154019"><a name="zh-cn_topic_0259133770_p185581652154019"></a><a name="zh-cn_topic_0259133770_p185581652154019"></a>公网NAT网关购买时长。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 2**  标签命名规则

    <a name="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_table248245914136"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_row2997812223119"><th class="cellrowborder" valign="top" width="12.049999999999999%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_p4367076523119"><a name="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_p4367076523119"></a><a name="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_p4367076523119"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="87.94999999999999%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_p4767111023119"><a name="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_p4767111023119"></a><a name="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_p4767111023119"></a>规则</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_row5695691323119"><td class="cellrowborder" valign="top" width="12.049999999999999%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_p5010724023119"><a name="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_p5010724023119"></a><a name="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_p5010724023119"></a>键</p>
    </td>
    <td class="cellrowborder" valign="top" width="87.94999999999999%" headers="mcps1.2.3.1.2 "><a name="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"></a><a name="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"></a><ul id="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"><li>不能为空。</li><li>对于同一NAT网关键值唯一。</li><li>长度不超过36个字符。</li><li>不能包含“=”、“*”、“&lt;”、“&gt;”、“\\”、“,”、“|”和“/”，且首尾字符不能为空格。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_row1973304523119"><td class="cellrowborder" valign="top" width="12.049999999999999%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_p5487280123119"><a name="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_p5487280123119"></a><a name="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_p5487280123119"></a>值</p>
    </td>
    <td class="cellrowborder" valign="top" width="87.94999999999999%" headers="mcps1.2.3.1.2 "><a name="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"></a><a name="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"></a><ul id="zh-cn_topic_0259133770_zh-cn_topic_0030971658_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"><li>长度不超过43个字符。</li><li>不能包含“=”、“*”、“&lt;”、“&gt;”、“\\”、“,”、“|”和“/”，且首尾字符不能为空格。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

    配置完成上述信息，会显示公网NAT网关配置费用，可通过“了解计费详情”查看计费信息。

6.  单击“立即购买”，在“规格确认”页面，您可以再次核对公网NAT网关信息。
7.  确认无误后，单击“提交”，开始创建公网NAT网关。

    公网NAT网关的创建过程一般需要1-5分钟。

8.  在“公网NAT网关”列表，查看公网NAT网关状态。

公网NAT网关创建成功后，查看该公网NAT网关所在的VPC的默认路由表下是否存在0.0.0.0/0的默认路由指向该公网NAT网关，如果不存在，请在默认路由表中添加一条指向该公网NAT网关的路由，或创建一个自定义路由表并在自定义路由表中添加0.0.0.0/0的默认路由指向该公网NAT网关。如下步骤以在自定义路由表中添加路由为例。

## 添加默认路由指向公网NAT网关<a name="section157491040181519"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
3.  在系统首页，单击“网络 \> 虚拟私有云”。
4.  单击左侧的“路由表”。
5.  在路由表页面，单击右上角的“创建路由表”。

    所属VPC：选择公网NAT网关所在的VPC。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >如果自定义路由表配额不足，请通过[提交工单](https://support.huaweicloud.com/usermanual-ticket/zh-cn_topic_0127038618.html)申请扩大路由表的配额。

6.  自定义路由表创建成功后，单击自定义路由表名称。进入自定义路由表基本信息页。
7.  单击“添加路由”，按照如下配置参数。

    目的地址：0.0.0.0/0

    下一跳类型：NAT网关

    下一跳：选择已创建的NAT网关

    **图 1**  添加路由<a name="zh-cn_topic_0259133770_fig86181523171120"></a>  
    ![](figures/添加路由.png "添加路由")

8.  单击“确定”。

