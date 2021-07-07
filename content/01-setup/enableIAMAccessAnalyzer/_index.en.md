+++
title = "Enable Amazon IAM Access Analyzer"
menuTitle = "Enable IAM Access Analyzer"
date = 2020-07-30T14:27:03-05:00
weight = 10
chapter = true
pre = "<b></b>"
+++

Now we are going to enable **IAM Access Analyzer** to monitor access to resources.

1. Go to the [Access Analyzer](https://console.aws.amazon.com/access-analyzer/home) console.
2. Click on the **Create analyzer** button.

{{% notice note %}}
At this point, if you have AWS Organizations implemented, you will have two choices for Zones of trust: ***Current Account*** and ***Current Organization***. If this is the case, it is recommended to enable IAM Access Analyzer on the whole Organization, instead of a single account.
{{% /notice %}}

![IAM Access Analyzer Zones of Trust Choices](/images/IAMAccessAnalyzerOrg.png)

{{% notice note %}}
If you are working with your own single account, enterprise accounts outside AWS Organizations or with Event Engine, you will be presented with only the ***Current Account*** choice.
{{% /notice %}}

3. Review the information, edit the analyzer's name if you like, choose the appropiate Zone of trust according to your scenario. Click on the **Create analyzer** button.  

{{% notice note %}}
If you are using Event Engine, disregard the error message at the top.
{{% /notice %}}

**IAM Access Analyzer** will be active and begin monitoring the resource access findings in this AWS account or AWS Organization.

![IAM Access Analyzer console view](/images/IAMAccessAnalyzerView.png)