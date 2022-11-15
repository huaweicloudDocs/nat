# 创建中转子网<a name="nat_exsub_0001"></a>

## 操作场景<a name="section185510413453"></a>

通过创建中转子网与中转IP，使虚拟私有云内多个云主机可以共享中转IP访问用户本地数据中心（IDC）或其他虚拟私有云，或面向私网提供服务。

## 操作步骤<a name="section498820319366"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
3.  在系统首页，单击“网络  \> NAT网关”。

    进入NAT网关页面。

4.  在NAT网关页面，单击“NAT网关\> 私网NAT网关”。
5.  在“中转子网”页签中，单击“创建中转子网”。
6.  根据界面提示，配置中转子网参数，详情请参见[表1](#zh-cn_topic_0127293986_table30787259144637)。

    **表 1**  中转子网参数说明

    <a name="zh-cn_topic_0127293986_table30787259144637"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0127293986_row1287982144637"><th class="cellrowborder" valign="top" width="23.189999999999998%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0127293986_p66523784144637"><a name="zh-cn_topic_0127293986_p66523784144637"></a><a name="zh-cn_topic_0127293986_p66523784144637"></a><strong id="zh-cn_topic_0127293986_b64475021144748"><a name="zh-cn_topic_0127293986_b64475021144748"></a><a name="zh-cn_topic_0127293986_b64475021144748"></a>参数</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="76.81%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0127293986_p19717393144637"><a name="zh-cn_topic_0127293986_p19717393144637"></a><a name="zh-cn_topic_0127293986_p19717393144637"></a><strong id="zh-cn_topic_0127293986_b37983896144751"><a name="zh-cn_topic_0127293986_b37983896144751"></a><a name="zh-cn_topic_0127293986_b37983896144751"></a>说明</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0127293986_row20452749101411"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0259133770_p2832836319588"><a name="zh-cn_topic_0259133770_p2832836319588"></a><a name="zh-cn_topic_0259133770_p2832836319588"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0259133770_p1289605119588"><a name="zh-cn_topic_0259133770_p1289605119588"></a><a name="zh-cn_topic_0259133770_p1289605119588"></a>中转子网名称。最大支持64个字符，仅支持中文、数字、字母、_（下划线）、-（中划线）。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0127293986_row1895714384610"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0259133770_p1464780019588"><a name="zh-cn_topic_0259133770_p1464780019588"></a><a name="zh-cn_topic_0259133770_p1464780019588"></a>虚拟私有云</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p6718522122311"><a name="p6718522122311"></a><a name="p6718522122311"></a>中转子网所属的VPC。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0127293986_row13591056167"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0259133770_p17196519588"><a name="zh-cn_topic_0259133770_p17196519588"></a><a name="zh-cn_topic_0259133770_p17196519588"></a>子网</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p16752553239"><a name="p16752553239"></a><a name="p16752553239"></a>中转子网IP所在子网。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0127293986_row189841183384"><td class="cellrowborder" valign="top" width="23.189999999999998%" headers="mcps1.2.3.1.1 "><p id="p7371045184212"><a name="p7371045184212"></a><a name="p7371045184212"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="76.81%" headers="mcps1.2.3.1.2 "><p id="p171281819162316"><a name="p171281819162316"></a><a name="p171281819162316"></a>中转子网信息描述。最大支持255个字符。</p>
    </td>
    </tr>
    </tbody>
    </table>


