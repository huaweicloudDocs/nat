# 查询DNAT规则列表<a name="nat_apiv2_0019"></a>

## 功能介绍<a name="zh-cn_topic_0168797280_section28610428164132"></a>

查询DNAT规则列表。

## URI<a name="zh-cn_topic_0168797280_section19503903164158"></a>

GET /v2/\{project\_id\}/dnat\_rules

>![](public_sys-resources/icon-note.gif) **说明：**   
>可以在URI后面用‘?’和‘&’添加不同的查询条件组合。支持参数说明中所有非必选参数过滤，请参考请求样例。  

**表 1**  参数说明

<a name="zh-cn_topic_0168797280_table93762054132613"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797280_row9501145413265"><th class="cellrowborder" valign="top" width="21.34%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0168797280_p550115415265"><a name="zh-cn_topic_0168797280_p550115415265"></a><a name="zh-cn_topic_0168797280_p550115415265"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.08%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0168797280_p846884314190"><a name="zh-cn_topic_0168797280_p846884314190"></a><a name="zh-cn_topic_0168797280_p846884314190"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.65%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0168797280_p3501754122611"><a name="zh-cn_topic_0168797280_p3501754122611"></a><a name="zh-cn_topic_0168797280_p3501754122611"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="52.93%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0168797280_p250105419269"><a name="zh-cn_topic_0168797280_p250105419269"></a><a name="zh-cn_topic_0168797280_p250105419269"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797280_row10334203817502"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797280_p167061545155011"><a name="zh-cn_topic_0168797280_p167061545155011"></a><a name="zh-cn_topic_0168797280_p167061545155011"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797280_p174692435197"><a name="zh-cn_topic_0168797280_p174692435197"></a><a name="zh-cn_topic_0168797280_p174692435197"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797280_p10706345205019"><a name="zh-cn_topic_0168797280_p10706345205019"></a><a name="zh-cn_topic_0168797280_p10706345205019"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797280_p970618457503"><a name="zh-cn_topic_0168797280_p970618457503"></a><a name="zh-cn_topic_0168797280_p970618457503"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row43352038165013"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797280_p270615451501"><a name="zh-cn_topic_0168797280_p270615451501"></a><a name="zh-cn_topic_0168797280_p270615451501"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797280_p12469174321913"><a name="zh-cn_topic_0168797280_p12469174321913"></a><a name="zh-cn_topic_0168797280_p12469174321913"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797280_p107131538135310"><a name="zh-cn_topic_0168797280_p107131538135310"></a><a name="zh-cn_topic_0168797280_p107131538135310"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797280_p10706104545013"><a name="zh-cn_topic_0168797280_p10706104545013"></a><a name="zh-cn_topic_0168797280_p10706104545013"></a>功能说明：每页返回的个数</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row14501165412613"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797280_p75013243343"><a name="zh-cn_topic_0168797280_p75013243343"></a><a name="zh-cn_topic_0168797280_p75013243343"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797280_p16975185561917"><a name="zh-cn_topic_0168797280_p16975185561917"></a><a name="zh-cn_topic_0168797280_p16975185561917"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797280_p1850122411341"><a name="zh-cn_topic_0168797280_p1850122411341"></a><a name="zh-cn_topic_0168797280_p1850122411341"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797280_p195072453418"><a name="zh-cn_topic_0168797280_p195072453418"></a><a name="zh-cn_topic_0168797280_p195072453418"></a>DNAT规则的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row105011454132610"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797280_p1501024133416"><a name="zh-cn_topic_0168797280_p1501024133416"></a><a name="zh-cn_topic_0168797280_p1501024133416"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797280_p9721456181914"><a name="zh-cn_topic_0168797280_p9721456181914"></a><a name="zh-cn_topic_0168797280_p9721456181914"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797280_p8501524153419"><a name="zh-cn_topic_0168797280_p8501524153419"></a><a name="zh-cn_topic_0168797280_p8501524153419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797280_p150524123413"><a name="zh-cn_topic_0168797280_p150524123413"></a><a name="zh-cn_topic_0168797280_p150524123413"></a>项目ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row650115472619"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797280_p650924193418"><a name="zh-cn_topic_0168797280_p650924193418"></a><a name="zh-cn_topic_0168797280_p650924193418"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797280_p229795718196"><a name="zh-cn_topic_0168797280_p229795718196"></a><a name="zh-cn_topic_0168797280_p229795718196"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797280_p750182443418"><a name="zh-cn_topic_0168797280_p750182443418"></a><a name="zh-cn_topic_0168797280_p750182443418"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797280_p1451624163419"><a name="zh-cn_topic_0168797280_p1451624163419"></a><a name="zh-cn_topic_0168797280_p1451624163419"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row1501125413265"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797280_p35192443411"><a name="zh-cn_topic_0168797280_p35192443411"></a><a name="zh-cn_topic_0168797280_p35192443411"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797280_p6349145814192"><a name="zh-cn_topic_0168797280_p6349145814192"></a><a name="zh-cn_topic_0168797280_p6349145814192"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797280_p17514241349"><a name="zh-cn_topic_0168797280_p17514241349"></a><a name="zh-cn_topic_0168797280_p17514241349"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797280_p135110246348"><a name="zh-cn_topic_0168797280_p135110246348"></a><a name="zh-cn_topic_0168797280_p135110246348"></a>虚拟机或者裸机的Port ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row16501354192619"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797280_p1651182413349"><a name="zh-cn_topic_0168797280_p1651182413349"></a><a name="zh-cn_topic_0168797280_p1651182413349"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797280_p293335810196"><a name="zh-cn_topic_0168797280_p293335810196"></a><a name="zh-cn_topic_0168797280_p293335810196"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797280_p195192414349"><a name="zh-cn_topic_0168797280_p195192414349"></a><a name="zh-cn_topic_0168797280_p195192414349"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797280_p15511224133415"><a name="zh-cn_topic_0168797280_p15511224133415"></a><a name="zh-cn_topic_0168797280_p15511224133415"></a>用户私有IP地址，例如专线连接的私有云地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row1150185452610"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797280_p5511424123420"><a name="zh-cn_topic_0168797280_p5511424123420"></a><a name="zh-cn_topic_0168797280_p5511424123420"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797280_p16452125917197"><a name="zh-cn_topic_0168797280_p16452125917197"></a><a name="zh-cn_topic_0168797280_p16452125917197"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797280_p3209415532"><a name="zh-cn_topic_0168797280_p3209415532"></a><a name="zh-cn_topic_0168797280_p3209415532"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797280_p7513246347"><a name="zh-cn_topic_0168797280_p7513246347"></a><a name="zh-cn_topic_0168797280_p7513246347"></a>虚拟机或者裸机对外提供服务的协议端口号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row1950195417261"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797280_p165122412348"><a name="zh-cn_topic_0168797280_p165122412348"></a><a name="zh-cn_topic_0168797280_p165122412348"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797280_p103664012204"><a name="zh-cn_topic_0168797280_p103664012204"></a><a name="zh-cn_topic_0168797280_p103664012204"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797280_p851132413341"><a name="zh-cn_topic_0168797280_p851132413341"></a><a name="zh-cn_topic_0168797280_p851132413341"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797280_p05119242344"><a name="zh-cn_topic_0168797280_p05119242344"></a><a name="zh-cn_topic_0168797280_p05119242344"></a>弹性公网IP的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row18501454162610"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797280_p16511224133414"><a name="zh-cn_topic_0168797280_p16511224133414"></a><a name="zh-cn_topic_0168797280_p16511224133414"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797280_p1231112112010"><a name="zh-cn_topic_0168797280_p1231112112010"></a><a name="zh-cn_topic_0168797280_p1231112112010"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797280_p5511224153414"><a name="zh-cn_topic_0168797280_p5511224153414"></a><a name="zh-cn_topic_0168797280_p5511224153414"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797280_p1352324123412"><a name="zh-cn_topic_0168797280_p1352324123412"></a><a name="zh-cn_topic_0168797280_p1352324123412"></a>弹性公网的IP地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row15501115452610"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797280_p155262418349"><a name="zh-cn_topic_0168797280_p155262418349"></a><a name="zh-cn_topic_0168797280_p155262418349"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797280_p11867124207"><a name="zh-cn_topic_0168797280_p11867124207"></a><a name="zh-cn_topic_0168797280_p11867124207"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797280_p18540194345317"><a name="zh-cn_topic_0168797280_p18540194345317"></a><a name="zh-cn_topic_0168797280_p18540194345317"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797280_p05210248347"><a name="zh-cn_topic_0168797280_p05210248347"></a><a name="zh-cn_topic_0168797280_p05210248347"></a>Floatingip对外提供服务的端口号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row15011954142618"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797280_p552192443414"><a name="zh-cn_topic_0168797280_p552192443414"></a><a name="zh-cn_topic_0168797280_p552192443414"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797280_p94551834208"><a name="zh-cn_topic_0168797280_p94551834208"></a><a name="zh-cn_topic_0168797280_p94551834208"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797280_p1521524123418"><a name="zh-cn_topic_0168797280_p1521524123418"></a><a name="zh-cn_topic_0168797280_p1521524123418"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797280_p1152182413347"><a name="zh-cn_topic_0168797280_p1152182413347"></a><a name="zh-cn_topic_0168797280_p1152182413347"></a>协议类型，目前支持TCP、UDP、ANY。</p>
<p id="zh-cn_topic_0168797280_p185242483420"><a name="zh-cn_topic_0168797280_p185242483420"></a><a name="zh-cn_topic_0168797280_p185242483420"></a>对应协议号6、17、0。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row13501165414269"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797280_p4529244343"><a name="zh-cn_topic_0168797280_p4529244343"></a><a name="zh-cn_topic_0168797280_p4529244343"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797280_p12369174162019"><a name="zh-cn_topic_0168797280_p12369174162019"></a><a name="zh-cn_topic_0168797280_p12369174162019"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797280_p9525242343"><a name="zh-cn_topic_0168797280_p9525242343"></a><a name="zh-cn_topic_0168797280_p9525242343"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0168797280_p165282423412"><a name="zh-cn_topic_0168797280_p165282423412"></a><a name="zh-cn_topic_0168797280_p165282423412"></a>DNAT规则的描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row18532115313334"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797280_p1252172410347"><a name="zh-cn_topic_0168797280_p1252172410347"></a><a name="zh-cn_topic_0168797280_p1252172410347"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797280_p999412432017"><a name="zh-cn_topic_0168797280_p999412432017"></a><a name="zh-cn_topic_0168797280_p999412432017"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797280_p1852142423414"><a name="zh-cn_topic_0168797280_p1852142423414"></a><a name="zh-cn_topic_0168797280_p1852142423414"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0168797280_ul952182413342"></a><a name="zh-cn_topic_0168797280_ul952182413342"></a><ul id="zh-cn_topic_0168797280_ul952182413342"><li>功能说明：DNAT规则的状态。</li><li>取值范围：<u id="zh-cn_topic_0168797280_u1752182473413"><a name="zh-cn_topic_0168797280_u1752182473413"></a><a name="zh-cn_topic_0168797280_u1752182473413"></a><u id="zh-cn_topic_0168797280_u105212413416"><a name="zh-cn_topic_0168797280_u105212413416"></a><a name="zh-cn_topic_0168797280_u105212413416"></a><a href="资源状态说明.md">资源状态说明</a></u></u>。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row359059183310"><td class="cellrowborder" valign="top" width="21.34%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0168797280_p752122412345"><a name="zh-cn_topic_0168797280_p752122412345"></a><a name="zh-cn_topic_0168797280_p752122412345"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0168797280_p46491350206"><a name="zh-cn_topic_0168797280_p46491350206"></a><a name="zh-cn_topic_0168797280_p46491350206"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0168797280_p5994165417270"><a name="zh-cn_topic_0168797280_p5994165417270"></a><a name="zh-cn_topic_0168797280_p5994165417270"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="52.93%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0168797280_ul71858556358"></a><a name="zh-cn_topic_0168797280_ul71858556358"></a><ul id="zh-cn_topic_0168797280_ul71858556358"><li>解冻/冻结状态。</li><li>取值范围：<a name="zh-cn_topic_0168797280_ul11838172814409"></a><a name="zh-cn_topic_0168797280_ul11838172814409"></a><ul id="zh-cn_topic_0168797280_ul11838172814409"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0168797280_section2749321016454"></a>

无

## 响应消息<a name="zh-cn_topic_0168797280_section55770648164519"></a>

响应参数如[表2](#zh-cn_topic_0168797280_table47307406164538)所示。

**表 2**  响应参数

<a name="zh-cn_topic_0168797280_table47307406164538"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797280_row43170063164538"><th class="cellrowborder" valign="top" width="20.73%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797280_p7114239164538"><a name="zh-cn_topic_0168797280_p7114239164538"></a><a name="zh-cn_topic_0168797280_p7114239164538"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="28.050000000000004%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797280_p39382504164538"><a name="zh-cn_topic_0168797280_p39382504164538"></a><a name="zh-cn_topic_0168797280_p39382504164538"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797280_p19483074164538"><a name="zh-cn_topic_0168797280_p19483074164538"></a><a name="zh-cn_topic_0168797280_p19483074164538"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797280_row34625156164538"><td class="cellrowborder" valign="top" width="20.73%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797280_p53174238164538"><a name="zh-cn_topic_0168797280_p53174238164538"></a><a name="zh-cn_topic_0168797280_p53174238164538"></a>dnat_rules</p>
</td>
<td class="cellrowborder" valign="top" width="28.050000000000004%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797280_p12146041164538"><a name="zh-cn_topic_0168797280_p12146041164538"></a><a name="zh-cn_topic_0168797280_p12146041164538"></a>Array(Object)</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797280_p31957648164538"><a name="zh-cn_topic_0168797280_p31957648164538"></a><a name="zh-cn_topic_0168797280_p31957648164538"></a>dnat_rule对象列表。请参考<a href="#zh-cn_topic_0168797280_table19520113319519">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  dnat\_rule字段说明

<a name="zh-cn_topic_0168797280_table19520113319519"></a>
<table><thead align="left"><tr id="zh-cn_topic_0168797280_row185205331254"><th class="cellrowborder" valign="top" width="20.49204920492049%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0168797280_p05291666"><a name="zh-cn_topic_0168797280_p05291666"></a><a name="zh-cn_topic_0168797280_p05291666"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="28.36283628362836%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0168797280_p75093619"><a name="zh-cn_topic_0168797280_p75093619"></a><a name="zh-cn_topic_0168797280_p75093619"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.14511451145114%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0168797280_p451917619"><a name="zh-cn_topic_0168797280_p451917619"></a><a name="zh-cn_topic_0168797280_p451917619"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0168797280_row15520133952"><td class="cellrowborder" valign="top" width="20.49204920492049%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797280_p951910610"><a name="zh-cn_topic_0168797280_p951910610"></a><a name="zh-cn_topic_0168797280_p951910610"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="28.36283628362836%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797280_p1656918614"><a name="zh-cn_topic_0168797280_p1656918614"></a><a name="zh-cn_topic_0168797280_p1656918614"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.14511451145114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797280_p051291561"><a name="zh-cn_topic_0168797280_p051291561"></a><a name="zh-cn_topic_0168797280_p051291561"></a>DNAT规则的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row105201033858"><td class="cellrowborder" valign="top" width="20.49204920492049%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797280_p254910616"><a name="zh-cn_topic_0168797280_p254910616"></a><a name="zh-cn_topic_0168797280_p254910616"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.36283628362836%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797280_p1251899611"><a name="zh-cn_topic_0168797280_p1251899611"></a><a name="zh-cn_topic_0168797280_p1251899611"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.14511451145114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797280_p15895619"><a name="zh-cn_topic_0168797280_p15895619"></a><a name="zh-cn_topic_0168797280_p15895619"></a>项目的ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row145201533552"><td class="cellrowborder" valign="top" width="20.49204920492049%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797280_p7512916615"><a name="zh-cn_topic_0168797280_p7512916615"></a><a name="zh-cn_topic_0168797280_p7512916615"></a>nat_gateway_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.36283628362836%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797280_p155999619"><a name="zh-cn_topic_0168797280_p155999619"></a><a name="zh-cn_topic_0168797280_p155999619"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.14511451145114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797280_p1251091363"><a name="zh-cn_topic_0168797280_p1251091363"></a><a name="zh-cn_topic_0168797280_p1251091363"></a>NAT网关的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row65209331152"><td class="cellrowborder" valign="top" width="20.49204920492049%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797280_p45892062"><a name="zh-cn_topic_0168797280_p45892062"></a><a name="zh-cn_topic_0168797280_p45892062"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.36283628362836%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797280_p3517914615"><a name="zh-cn_topic_0168797280_p3517914615"></a><a name="zh-cn_topic_0168797280_p3517914615"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.14511451145114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797280_p1651197615"><a name="zh-cn_topic_0168797280_p1651197615"></a><a name="zh-cn_topic_0168797280_p1651197615"></a>虚拟机或者裸机的Port ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row25205331457"><td class="cellrowborder" valign="top" width="20.49204920492049%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797280_p1251911618"><a name="zh-cn_topic_0168797280_p1251911618"></a><a name="zh-cn_topic_0168797280_p1251911618"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="28.36283628362836%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797280_p1351091667"><a name="zh-cn_topic_0168797280_p1351091667"></a><a name="zh-cn_topic_0168797280_p1351091667"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.14511451145114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797280_p95891616"><a name="zh-cn_topic_0168797280_p95891616"></a><a name="zh-cn_topic_0168797280_p95891616"></a>用户私有IP地址，例如专线连接的私有云地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row1052018331559"><td class="cellrowborder" valign="top" width="20.49204920492049%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797280_p75194611"><a name="zh-cn_topic_0168797280_p75194611"></a><a name="zh-cn_topic_0168797280_p75194611"></a>internal_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="28.36283628362836%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797280_p01355315317"><a name="zh-cn_topic_0168797280_p01355315317"></a><a name="zh-cn_topic_0168797280_p01355315317"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="51.14511451145114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797280_p14520920611"><a name="zh-cn_topic_0168797280_p14520920611"></a><a name="zh-cn_topic_0168797280_p14520920611"></a>虚拟机或者裸机对外提供服务的协议端口号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row1752020331551"><td class="cellrowborder" valign="top" width="20.49204920492049%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797280_p051991961"><a name="zh-cn_topic_0168797280_p051991961"></a><a name="zh-cn_topic_0168797280_p051991961"></a>floating_ip_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.36283628362836%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797280_p05109969"><a name="zh-cn_topic_0168797280_p05109969"></a><a name="zh-cn_topic_0168797280_p05109969"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.14511451145114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797280_p135997619"><a name="zh-cn_topic_0168797280_p135997619"></a><a name="zh-cn_topic_0168797280_p135997619"></a>弹性公网IP的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row652015339517"><td class="cellrowborder" valign="top" width="20.49204920492049%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797280_p9510911613"><a name="zh-cn_topic_0168797280_p9510911613"></a><a name="zh-cn_topic_0168797280_p9510911613"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="28.36283628362836%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797280_p155189360"><a name="zh-cn_topic_0168797280_p155189360"></a><a name="zh-cn_topic_0168797280_p155189360"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.14511451145114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797280_p25297618"><a name="zh-cn_topic_0168797280_p25297618"></a><a name="zh-cn_topic_0168797280_p25297618"></a>弹性公网的IP地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row1752013312513"><td class="cellrowborder" valign="top" width="20.49204920492049%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797280_p175199763"><a name="zh-cn_topic_0168797280_p175199763"></a><a name="zh-cn_topic_0168797280_p175199763"></a>external_service_port</p>
</td>
<td class="cellrowborder" valign="top" width="28.36283628362836%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797280_p1951396617"><a name="zh-cn_topic_0168797280_p1951396617"></a><a name="zh-cn_topic_0168797280_p1951396617"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="51.14511451145114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797280_p1557910616"><a name="zh-cn_topic_0168797280_p1557910616"></a><a name="zh-cn_topic_0168797280_p1557910616"></a>Floatingip对外提供服务的端口号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row752017339518"><td class="cellrowborder" valign="top" width="20.49204920492049%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797280_p185591614"><a name="zh-cn_topic_0168797280_p185591614"></a><a name="zh-cn_topic_0168797280_p185591614"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="28.36283628362836%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797280_p1251395611"><a name="zh-cn_topic_0168797280_p1251395611"></a><a name="zh-cn_topic_0168797280_p1251395611"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.14511451145114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797280_p4517918619"><a name="zh-cn_topic_0168797280_p4517918619"></a><a name="zh-cn_topic_0168797280_p4517918619"></a>协议类型，目前支持TCP、UDP、ANY。</p>
<p id="zh-cn_topic_0168797280_p1551098611"><a name="zh-cn_topic_0168797280_p1551098611"></a><a name="zh-cn_topic_0168797280_p1551098611"></a>对应协议号6、17、0。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row7520143311514"><td class="cellrowborder" valign="top" width="20.49204920492049%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797280_p125991664"><a name="zh-cn_topic_0168797280_p125991664"></a><a name="zh-cn_topic_0168797280_p125991664"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="28.36283628362836%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797280_p4569262"><a name="zh-cn_topic_0168797280_p4569262"></a><a name="zh-cn_topic_0168797280_p4569262"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="51.14511451145114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797280_p4510915617"><a name="zh-cn_topic_0168797280_p4510915617"></a><a name="zh-cn_topic_0168797280_p4510915617"></a>DNAT规则的描述。</p>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row55358331458"><td class="cellrowborder" valign="top" width="20.49204920492049%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797280_p353919612"><a name="zh-cn_topic_0168797280_p353919612"></a><a name="zh-cn_topic_0168797280_p353919612"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="28.36283628362836%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797280_p85893612"><a name="zh-cn_topic_0168797280_p85893612"></a><a name="zh-cn_topic_0168797280_p85893612"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.14511451145114%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797280_ul6519962"></a><a name="zh-cn_topic_0168797280_ul6519962"></a><ul id="zh-cn_topic_0168797280_ul6519962"><li>功能说明：DNAT规则的状态。</li><li>取值范围：<a href="资源状态说明.md#table1390614366107">资源状态说明</a>。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row1353593311511"><td class="cellrowborder" valign="top" width="20.49204920492049%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797280_p10529463"><a name="zh-cn_topic_0168797280_p10529463"></a><a name="zh-cn_topic_0168797280_p10529463"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="28.36283628362836%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797280_p1051099619"><a name="zh-cn_topic_0168797280_p1051099619"></a><a name="zh-cn_topic_0168797280_p1051099619"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="51.14511451145114%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797280_ul44884251357"></a><a name="zh-cn_topic_0168797280_ul44884251357"></a><ul id="zh-cn_topic_0168797280_ul44884251357"><li>解冻/冻结状态。</li><li>取值范围：<a name="zh-cn_topic_0168797280_ul24889251258"></a><a name="zh-cn_topic_0168797280_ul24889251258"></a><ul id="zh-cn_topic_0168797280_ul24889251258"><li>“true”：解冻</li><li>“false”：冻结</li></ul>
</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row1953517336520"><td class="cellrowborder" valign="top" width="20.49204920492049%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797280_p1050916613"><a name="zh-cn_topic_0168797280_p1050916613"></a><a name="zh-cn_topic_0168797280_p1050916613"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="28.36283628362836%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797280_p4529368"><a name="zh-cn_topic_0168797280_p4529368"></a><a name="zh-cn_topic_0168797280_p4529368"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.14511451145114%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0168797280_ul1151898616"></a><a name="zh-cn_topic_0168797280_ul1151898616"></a><ul id="zh-cn_topic_0168797280_ul1151898616"><li>DNAT规则的创建时间戳，遵循UTC时间，保留小数点后6位，格式是yyyy-mm-dd hh:mm:ss</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row19201277542"><td class="cellrowborder" valign="top" width="20.49204920492049%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797280_p144447813543"><a name="zh-cn_topic_0168797280_p144447813543"></a><a name="zh-cn_topic_0168797280_p144447813543"></a>internal_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="28.36283628362836%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797280_p104441582544"><a name="zh-cn_topic_0168797280_p104441582544"></a><a name="zh-cn_topic_0168797280_p104441582544"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.14511451145114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797280_p1744448155420"><a name="zh-cn_topic_0168797280_p1744448155420"></a><a name="zh-cn_topic_0168797280_p1744448155420"></a>虚拟机或者裸机对外提供服务的协议端口号范围。</p>
<a name="zh-cn_topic_0168797280_ul14444988542"></a><a name="zh-cn_topic_0168797280_ul14444988542"></a><ul id="zh-cn_topic_0168797280_ul14444988542"><li>功能说明：该端口范围与external _service_port_range按顺序实现1:1映射。</li><li>取值范围：1~65535。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0168797280_row1420113710541"><td class="cellrowborder" valign="top" width="20.49204920492049%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0168797280_p44459885417"><a name="zh-cn_topic_0168797280_p44459885417"></a><a name="zh-cn_topic_0168797280_p44459885417"></a>external_service_port_range</p>
</td>
<td class="cellrowborder" valign="top" width="28.36283628362836%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0168797280_p1445108185415"><a name="zh-cn_topic_0168797280_p1445108185415"></a><a name="zh-cn_topic_0168797280_p1445108185415"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.14511451145114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0168797280_p1944510865418"><a name="zh-cn_topic_0168797280_p1944510865418"></a><a name="zh-cn_topic_0168797280_p1944510865418"></a>Floatingip对外提供服务的端口号范围。</p>
<a name="zh-cn_topic_0168797280_ul1344518855416"></a><a name="zh-cn_topic_0168797280_ul1344518855416"></a><ul id="zh-cn_topic_0168797280_ul1344518855416"><li>功能说明：该端口范围与internal _service_port_range按顺序实现1:1映射。</li><li>取值范围：1~65535。</li></ul>
</td>
</tr>
</tbody>
</table>

## 示例<a name="zh-cn_topic_0168797280_section39793997164640"></a>

-   请求样例

    ```
    GET https://{Endpoint}/v2/d199ba7e0ba64899b2e81518104b1526d/dnat_rules?limit=10
    ```


-   响应样例

    ```
    { 
         "dnat_rules": [ 
             { 
                 "floating_ip_id": "bf99c679-9f41-4dac-8513-9c9228e713e1", 
                 "status": "ACTIVE", 
                 "nat_gateway_id": "cda3a125-2406-456c-a11f-598e10578541", 
                 "admin_state_up": true, 
                 "port_id": "9a469561-daac-4c94-88f5-39366e5ea193", 
                 "private_ip": "", 
                 "internal_service_port": 993, 
                 "protocol": "tcp", 
                 "tenant_id": "abc", 
                 "created_at": "2017-11-15 15:44:42.595173", 
                 "id": "79195d50-0271-41f1-bded-4c089b2502ff", 
                 "floating_ip_address": "5.21.11.226", 
                 "external_service_port": 242, 
                 "description": "my dnat rule 01" 
             }, 
             { 
                 "floating_ip_id": "cf99c679-9f41-4dac-8513-9c9228e713e1", 
                 "status": "ACTIVE", 
                 "nat_gateway_id": "dda3a125-2406-456c-a11f-598e10578541", 
                 "admin_state_up": true, 
                 "port_id": "", 
                 "private_ip": "192.168.1.100", 
                 "internal_service_port": 0, 
                 "protocol": "any", 
                 "tenant_id": "abc", 
                 "created_at": "2017-11-16 15:44:42.595173", 
                 "id": "89195d50-0271-41f1-bded-4c089b2502ff", 
                 "floating_ip_address": "5.21.11.227", 
                 "external_service_port": 0, 
                 "description": "my dnat rule 01" 
             } 
         ] 
     }
    ```


## 状态码<a name="zh-cn_topic_0168797280_section45841191164749"></a>

请参考[状态码](状态码.md)。

