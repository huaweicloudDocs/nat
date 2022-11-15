# 标签管理<a name="nat_tag_0000"></a>

## 应用场景<a name="section51463883214456"></a>

NAT网关标签是NAT网关的标识。为NAT网关添加标签，可以方便用户识别和管理拥有的NAT网关。您可以在创建NAT网关时增加标签或者在已经创建的NAT网关详情页添加标签，最多可以给NAT网关添加10个标签。

>![](public_sys-resources/icon-note.gif) **说明：** 
>目前仅公网NAT网关支持标签管理功能。

标签共由两部分组成：“键”和“值”，其中，“键”和“值”的命名规则如[表1](#ted9687ca14074ef785241145365a6175)所示。

**表 1**  标签命名规则

<a name="ted9687ca14074ef785241145365a6175"></a>
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

## 操作步骤<a name="section4374728222113"></a>

**在公网NAT网关列表页，按标签的键或值搜索目标公网NAT网关。**

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
3.  选择“网络  \> NAT网关”。
4.  单击公网NAT网关列表右上角的“标签搜索”，展开查询页。
5.  输入待查询公网NAT网关的标签值。键和值均不能为空。
6.  单击“+”，添加需查询的标签值。

    系统支持添加10个标签值，并取各个标签值的交集，对目标公网NAT网关进行搜索。

7.  单击“搜索”。

    系统根据标签的键和值搜索公网NAT网关。


**在公网NAT网关的标签页，执行标签的增、删、改、查操作。**

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
3.  选择“网络  \> NAT网关”。
4.  单击公网NAT网关列表中需要查看的公网NAT网关名称，进入公网NAT网关详情页面。

1.  选择“标签”页签，对公网NAT网关的标签执行增、删、改、查。
    -   查看

        在“标签”页，可以查看当前公网NAT网关的标签详情，包括标签个数，以及每个标签的键和值。

    -   添加

        单击左上角的“添加标签”，在弹出的“添加标签”窗口，输入新添加标签的键和值，并单击“确定”。

        >![](public_sys-resources/icon-note.gif) **说明：** 
        >您可以根据界面提示，使用标签管理服务的预定义标签功能，简化添加标签的操作。预定义标签操作请参见[《标签管理服务用户指南》](https://support.huaweicloud.com/usermanual-tms/zh-cn_topic_0101849262.html)。

    -   修改

        单击标签所在行“操作”列下的“编辑”，在弹出的“编辑标签”窗口，输入修改后标签的值，并单击“确定”。

    -   删除

        单击标签所在行“操作”列下的“删除”，如果确认删除，在弹出的“删除标签”窗口，单击“是”。



