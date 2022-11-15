# 创建告警规则<a name="zh-cn_topic_0113772081"></a>

## 操作场景<a name="zh-cn_topic_0201532920_section38299792222911"></a>

通过设置NAT网关告警规则，用户可自定义监控目标与通知策略，及时了解NAT网关运行状况，从而起到预警作用。

## 操作步骤<a name="zh-cn_topic_0201532920_section7969360222918"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
3.  选择“管理与监管 \> 云监控服务”。
4.  在左侧导航树栏，选择“告警 \> 告警规则”。
5.  在“告警规则”界面，单击“创建告警规则”进行添加，或者选择已有的告警规则进行修改，设置NAT网关的告警规则。
6.  在“创建告警规则”界面，根据界面提示配置参数。
    1.  根据界面提示，配置告警规则的基本信息。

        **表 1**  配置规则信息

        <a name="zh-cn_topic_0201532920_table17694105411317"></a>
        <table><thead align="left"><tr id="zh-cn_topic_0201532920_row18694135418312"><th class="cellrowborder" valign="top" width="19.21%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0201532920_p4694195463111"><a name="zh-cn_topic_0201532920_p4694195463111"></a><a name="zh-cn_topic_0201532920_p4694195463111"></a>参数</p>
        </th>
        <th class="cellrowborder" valign="top" width="80.78999999999999%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0201532920_p12694175417314"><a name="zh-cn_topic_0201532920_p12694175417314"></a><a name="zh-cn_topic_0201532920_p12694175417314"></a>参数说明</p>
        </th>
        </tr>
        </thead>
        <tbody><tr id="zh-cn_topic_0201532920_row17694105423111"><td class="cellrowborder" valign="top" width="19.21%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0201532920_p7694854113110"><a name="zh-cn_topic_0201532920_p7694854113110"></a><a name="zh-cn_topic_0201532920_p7694854113110"></a>名称</p>
        </td>
        <td class="cellrowborder" valign="top" width="80.78999999999999%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0201532920_p469414543310"><a name="zh-cn_topic_0201532920_p469414543310"></a><a name="zh-cn_topic_0201532920_p469414543310"></a>系统会随机产生一个名称，用户也可以进行修改。</p>
        <p id="zh-cn_topic_0201532920_p596775521914"><a name="zh-cn_topic_0201532920_p596775521914"></a><a name="zh-cn_topic_0201532920_p596775521914"></a>取值样例：alarm-b6al</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0201532920_row13694165413316"><td class="cellrowborder" valign="top" width="19.21%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0201532920_p6694115493116"><a name="zh-cn_topic_0201532920_p6694115493116"></a><a name="zh-cn_topic_0201532920_p6694115493116"></a>描述</p>
        </td>
        <td class="cellrowborder" valign="top" width="80.78999999999999%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0201532920_p0694954103120"><a name="zh-cn_topic_0201532920_p0694954103120"></a><a name="zh-cn_topic_0201532920_p0694954103120"></a>告警规则描述（此参数非必填项）。</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0201532920_row73291535102612"><td class="cellrowborder" valign="top" width="19.21%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0201532920_p157352063456"><a name="zh-cn_topic_0201532920_p157352063456"></a><a name="zh-cn_topic_0201532920_p157352063456"></a>企业项目</p>
        </td>
        <td class="cellrowborder" valign="top" width="80.78999999999999%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0201532920_p1730219522"><a name="zh-cn_topic_0201532920_p1730219522"></a><a name="zh-cn_topic_0201532920_p1730219522"></a>告警规则所属的企业项目。只有拥有该企业项目权限的用户才可以查看和管理该告警规则。创建企业项目请参考：<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0108763964.html" target="_blank" rel="noopener noreferrer">创建企业项目</a>。</p>
        </td>
        </tr>
        </tbody>
        </table>

    2.  选择监控对象，配置告警内容参数。

        **图 1**  配置告警内容<a name="zh-cn_topic_0201532920_fig1674320252422"></a>  
        ![](figures/配置告警内容.png "配置告警内容")

        **表 2**  配置告警内容

        <a name="zh-cn_topic_0201532920_table1951189104216"></a>
        <table><thead align="left"><tr id="zh-cn_topic_0201532920_row79491995423"><th class="cellrowborder" valign="top" width="14.99%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201532920_p1694917913426"><a name="zh-cn_topic_0201532920_p1694917913426"></a><a name="zh-cn_topic_0201532920_p1694917913426"></a>参数</p>
        </th>
        <th class="cellrowborder" valign="top" width="63.71%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201532920_p79496924210"><a name="zh-cn_topic_0201532920_p79496924210"></a><a name="zh-cn_topic_0201532920_p79496924210"></a>参数说明</p>
        </th>
        <th class="cellrowborder" valign="top" width="21.3%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201532920_p139491990425"><a name="zh-cn_topic_0201532920_p139491990425"></a><a name="zh-cn_topic_0201532920_p139491990425"></a>取值样例</p>
        </th>
        </tr>
        </thead>
        <tbody><tr id="zh-cn_topic_0201532920_row17949393429"><td class="cellrowborder" valign="top" width="14.99%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201532920_p19949592427"><a name="zh-cn_topic_0201532920_p19949592427"></a><a name="zh-cn_topic_0201532920_p19949592427"></a>资源类型</p>
        </td>
        <td class="cellrowborder" valign="top" width="63.71%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201532920_p89497934220"><a name="zh-cn_topic_0201532920_p89497934220"></a><a name="zh-cn_topic_0201532920_p89497934220"></a>配置告警规则监控的服务名称。</p>
        </td>
        <td class="cellrowborder" valign="top" width="21.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201532920_p19494917424"><a name="zh-cn_topic_0201532920_p19494917424"></a><a name="zh-cn_topic_0201532920_p19494917424"></a>NAT网关</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0201532920_row895014917429"><td class="cellrowborder" valign="top" width="14.99%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201532920_p12949993427"><a name="zh-cn_topic_0201532920_p12949993427"></a><a name="zh-cn_topic_0201532920_p12949993427"></a>维度</p>
        </td>
        <td class="cellrowborder" valign="top" width="63.71%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201532920_p1694918915428"><a name="zh-cn_topic_0201532920_p1694918915428"></a><a name="zh-cn_topic_0201532920_p1694918915428"></a>用于指定告警规则对应指标的维度名称</p>
        </td>
        <td class="cellrowborder" valign="top" width="21.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201532920_p5949129174211"><a name="zh-cn_topic_0201532920_p5949129174211"></a><a name="zh-cn_topic_0201532920_p5949129174211"></a>公网NAT网关</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0201532920_row9950199425"><td class="cellrowborder" valign="top" width="14.99%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201532920_p1695069174215"><a name="zh-cn_topic_0201532920_p1695069174215"></a><a name="zh-cn_topic_0201532920_p1695069174215"></a>监控范围</p>
        </td>
        <td class="cellrowborder" valign="top" width="63.71%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201532920_p595012916426"><a name="zh-cn_topic_0201532920_p595012916426"></a><a name="zh-cn_topic_0201532920_p595012916426"></a>告警规则适用的资源范围，可选择资源分组或指定资源。</p>
        <div class="note" id="zh-cn_topic_0201532920_note1895019910426"><a name="zh-cn_topic_0201532920_note1895019910426"></a><a name="zh-cn_topic_0201532920_note1895019910426"></a><span class="notetitle"> 说明： </span><div class="notebody"><a name="zh-cn_topic_0201532920_ul895019914215"></a><a name="zh-cn_topic_0201532920_ul895019914215"></a><ul id="zh-cn_topic_0201532920_ul895019914215"><li>当选择资源分组时，该分组下任何资源满足告警策略时，都会触发告警通知。</li><li>选择指定资源时，勾选具体的监控对象，单击<a name="zh-cn_topic_0201532920_image1935911824313"></a><a name="zh-cn_topic_0201532920_image1935911824313"></a><span><img id="zh-cn_topic_0201532920_image1935911824313" src="figures/icon-rightArrow.png"></span>将监控对象同步到右侧对话框。</li></ul>
        </div></div>
        </td>
        <td class="cellrowborder" valign="top" width="21.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201532920_p1195016918422"><a name="zh-cn_topic_0201532920_p1195016918422"></a><a name="zh-cn_topic_0201532920_p1195016918422"></a>指定资源</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0201532920_row5951139154215"><td class="cellrowborder" valign="top" width="14.99%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201532920_p49501692426"><a name="zh-cn_topic_0201532920_p49501692426"></a><a name="zh-cn_topic_0201532920_p49501692426"></a>选择类型</p>
        </td>
        <td class="cellrowborder" valign="top" width="63.71%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201532920_p1295099124214"><a name="zh-cn_topic_0201532920_p1295099124214"></a><a name="zh-cn_topic_0201532920_p1295099124214"></a>根据需要可选择从模板导入或自定义创建。</p>
        </td>
        <td class="cellrowborder" valign="top" width="21.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201532920_p995019910423"><a name="zh-cn_topic_0201532920_p995019910423"></a><a name="zh-cn_topic_0201532920_p995019910423"></a>自定义创建</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0201532920_row1095129204217"><td class="cellrowborder" valign="top" width="14.99%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201532920_p189513916422"><a name="zh-cn_topic_0201532920_p189513916422"></a><a name="zh-cn_topic_0201532920_p189513916422"></a>模板</p>
        </td>
        <td class="cellrowborder" valign="top" width="63.71%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201532920_p795116910422"><a name="zh-cn_topic_0201532920_p795116910422"></a><a name="zh-cn_topic_0201532920_p795116910422"></a>选择需要导入的模板。</p>
        <p id="zh-cn_topic_0201532920_p83209532920"><a name="zh-cn_topic_0201532920_p83209532920"></a><a name="zh-cn_topic_0201532920_p83209532920"></a>您可以选择系统预置的默认告警模板，或者选择自定义模板。</p>
        </td>
        <td class="cellrowborder" valign="top" width="21.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201532920_p169511293424"><a name="zh-cn_topic_0201532920_p169511293424"></a><a name="zh-cn_topic_0201532920_p169511293424"></a>-</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0201532920_row89519954220"><td class="cellrowborder" valign="top" width="14.99%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201532920_p1951159164214"><a name="zh-cn_topic_0201532920_p1951159164214"></a><a name="zh-cn_topic_0201532920_p1951159164214"></a>告警策略</p>
        </td>
        <td class="cellrowborder" valign="top" width="63.71%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201532920_p9951189154217"><a name="zh-cn_topic_0201532920_p9951189154217"></a><a name="zh-cn_topic_0201532920_p9951189154217"></a>触发告警规则的告警策略。</p>
        <p id="zh-cn_topic_0201532920_p10661061173"><a name="zh-cn_topic_0201532920_p10661061173"></a><a name="zh-cn_topic_0201532920_p10661061173"></a>当资源类型选择站点监控、日志监控、自定义监控、具体的云服务时，是否触发告警取决于连续周期的数据是否达到阈值。例如SNAT连接数监控周期为1分钟，连续三个周期原始值≥8000个，则触发告警。</p>
        </td>
        <td class="cellrowborder" valign="top" width="21.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201532920_p29511797423"><a name="zh-cn_topic_0201532920_p29511797423"></a><a name="zh-cn_topic_0201532920_p29511797423"></a>-</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0201532920_row5951129114220"><td class="cellrowborder" valign="top" width="14.99%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201532920_p179518918423"><a name="zh-cn_topic_0201532920_p179518918423"></a><a name="zh-cn_topic_0201532920_p179518918423"></a>告警级别</p>
        </td>
        <td class="cellrowborder" valign="top" width="63.71%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201532920_p169511919421"><a name="zh-cn_topic_0201532920_p169511919421"></a><a name="zh-cn_topic_0201532920_p169511919421"></a>根据告警的严重程度不同等级，可选择紧急、重要、次要、提示。</p>
        </td>
        <td class="cellrowborder" valign="top" width="21.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201532920_p12951098425"><a name="zh-cn_topic_0201532920_p12951098425"></a><a name="zh-cn_topic_0201532920_p12951098425"></a>重要</p>
        </td>
        </tr>
        </tbody>
        </table>

    3.  根据界面提示，配置告警通知参数。

        **图 2**  配置告警通知<a name="zh-cn_topic_0201532920_fig458094616420"></a>  
        ![](figures/配置告警通知.png "配置告警通知")

        **表 3**  配置告警通知

        <a name="zh-cn_topic_0201532920_table54161352427"></a>
        <table><thead align="left"><tr id="zh-cn_topic_0201532920_row13415173554216"><th class="cellrowborder" valign="top" width="18.87%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0201532920_p174151835174212"><a name="zh-cn_topic_0201532920_p174151835174212"></a><a name="zh-cn_topic_0201532920_p174151835174212"></a>参数</p>
        </th>
        <th class="cellrowborder" valign="top" width="81.13%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0201532920_p13415123594216"><a name="zh-cn_topic_0201532920_p13415123594216"></a><a name="zh-cn_topic_0201532920_p13415123594216"></a>参数说明</p>
        </th>
        </tr>
        </thead>
        <tbody><tr id="zh-cn_topic_0201532920_row3415103514420"><td class="cellrowborder" valign="top" width="18.87%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0201532920_p1741553594216"><a name="zh-cn_topic_0201532920_p1741553594216"></a><a name="zh-cn_topic_0201532920_p1741553594216"></a>发送通知</p>
        </td>
        <td class="cellrowborder" valign="top" width="81.13%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0201532920_p1641523534216"><a name="zh-cn_topic_0201532920_p1641523534216"></a><a name="zh-cn_topic_0201532920_p1641523534216"></a>配置是否发送邮件、短信、HTTP和HTTPS通知用户。</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0201532920_row42651257134517"><td class="cellrowborder" valign="top" width="18.87%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0201532920_p1441533517421"><a name="zh-cn_topic_0201532920_p1441533517421"></a><a name="zh-cn_topic_0201532920_p1441533517421"></a>通知对象</p>
        </td>
        <td class="cellrowborder" valign="top" width="81.13%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0201532920_p1741725011112"><a name="zh-cn_topic_0201532920_p1741725011112"></a><a name="zh-cn_topic_0201532920_p1741725011112"></a>需要发送告警通知的对象，可选择云账号联系人或主题名称。</p>
        <a name="zh-cn_topic_0201532920_ul15465311191116"></a><a name="zh-cn_topic_0201532920_ul15465311191116"></a><ul id="zh-cn_topic_0201532920_ul15465311191116"><li>云账号联系人为注册账号时的手机和邮箱。</li><li>主题是消息发布或客户端订阅通知的特定事件类型，若此处没有需要的主题则需先创建主题并添加订阅，创建主题并添加订阅请参见<a href="https://support.huaweicloud.com/usermanual-ces/ces_01_0069.html" target="_blank" rel="noopener noreferrer">《云监控用户指南》</a>。</li></ul>
        </td>
        </tr>
        <tr id="zh-cn_topic_0201532920_row18415153564213"><td class="cellrowborder" valign="top" width="18.87%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0201532920_p1241513574211"><a name="zh-cn_topic_0201532920_p1241513574211"></a><a name="zh-cn_topic_0201532920_p1241513574211"></a>生效时间</p>
        </td>
        <td class="cellrowborder" valign="top" width="81.13%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0201532920_p11415123518423"><a name="zh-cn_topic_0201532920_p11415123518423"></a><a name="zh-cn_topic_0201532920_p11415123518423"></a>该告警规则仅在生效时间内发送通知消息。</p>
        <p id="zh-cn_topic_0201532920_p44151435144210"><a name="zh-cn_topic_0201532920_p44151435144210"></a><a name="zh-cn_topic_0201532920_p44151435144210"></a>如生效时间为08:00-20:00，则该告警规则仅在08:00-20:00发送通知消息。</p>
        </td>
        </tr>
        <tr id="zh-cn_topic_0201532920_row1416153504210"><td class="cellrowborder" valign="top" width="18.87%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0201532920_p0415235174219"><a name="zh-cn_topic_0201532920_p0415235174219"></a><a name="zh-cn_topic_0201532920_p0415235174219"></a>触发条件</p>
        </td>
        <td class="cellrowborder" valign="top" width="81.13%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0201532920_p141617354423"><a name="zh-cn_topic_0201532920_p141617354423"></a><a name="zh-cn_topic_0201532920_p141617354423"></a>可以选择“出现告警”、“恢复正常”两种状态，作为触发告警通知的条件。</p>
        </td>
        </tr>
        </tbody>
        </table>

7.  规则参数设置完成后，单击“立即创建”。

    NAT网关告警规则设置完成后，当符合规则的告警产生时，系统会自动进行通知。


>![](public_sys-resources/icon-note.gif) **说明：** 
>更多关于设置告警规则的信息，请参见[《云监控用户指南》](https://support.huaweicloud.com/usermanual-ces/ces_01_0073.html)。

