# 创建用户并授权使用NAT网关<a name="zh-cn_topic_201905304"></a>

如果您需要对您所拥有的NAT网关（NAT Gateway，简称NAT网关）进行精细的权限管理，您可以使用统一身份认证服务（Identity and Access Management，简称IAM），通过IAM，您可以：

-   根据企业的业务组织，在您的华为云账号中，给企业中不同职能部门的员工创建IAM用户，让员工拥有唯一安全凭证，并使用NAT网关。
-   根据企业用户的职能，设置不同的访问权限，以达到用户之间的权限隔离。
-   将NAT网关委托给更专业、高效的其他华为云账号或者云服务，这些账号或者云服务可以根据权限进行代运维。

如果华为云账号已经能满足您的要求，不需要创建独立的IAM用户，您可以跳过本章节，不影响您使用NAT网关服务的其它功能。

本章节为您介绍对用户授权的方法，操作流程如[图1](#zh-cn_topic_0171158980_fig111743404535)所示。

## 前提条件<a name="section61001726122520"></a>

-   “NAT Viewer”属于策略，请先在IAM控制台中开通基于策略的访问控制公测，开通方法请参见：[申请基于策略的访问控制公测](https://support.huaweicloud.com/usermanual-iam/iam_01_019.html)。
-   给用户组授权之前，请您了解用户组可以添加的NAT网关权限，并结合实际需求进行选择，NAT网关支持的系统权限，请参见：[NAT网关权限](https://support.huaweicloud.com/productdesc-natgateway/nat_permission_0000.html)。若您需要对除NAT网关之外的其它服务授权，IAM支持服务的所有策略请参见[权限策略](https://support.huaweicloud.com/permissions/policy_list.html?product=natgateway)。

## 示例流程<a name="zh-cn_topic_0171158980_section203711514125317"></a>

**图 1**  给用户授权NAT网关权限流程<a name="zh-cn_topic_0171158980_fig111743404535"></a>  
![](figures/给用户授权NAT网关权限流程.jpg "给用户授权NAT网关权限流程")

1.  <a name="zh-cn_topic_0171158980_li527593485415"></a>创建用户组并授权

    在IAM控制台创建用户组，并授予NAT网关服务权限“NAT Viewer”。

2.  创建用户

    在IAM控制台创建用户，并将其加入[1.创建用户组并授权](#zh-cn_topic_0171158980_li527593485415)中创建的用户组。

3.  用户登录并验证权限

    新创建的用户登录控制台

    切换至授权区域，验证权限：

    -   在“服务列表”中选择NAT网关，进入NAT网关主界面，单击右上角“购买NAT网关”，如果无法购买NAT网关（假设当前权限仅包含NAT Viewer），表示“NAT Viewer”已生效。
    -   在“服务列表”中选择除NAT网关外（假设当前策略仅包含NAT Viewer）的任一服务，若提示权限不足，表示“NAT Viewer”已生效。


