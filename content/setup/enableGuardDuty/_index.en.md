+++
title = "Enable Amazon GuardDuty"
menuTitle = "Enable GuardDuty"
date = 2020-07-30T14:27:03-05:00
weight = 10
chapter = true
pre = "<b></b>"
+++

Amazon GuardDuty is a threat detection service that continuosly monitors for malicious activity and unauthorized behavior to protect your AWS, workloads, and data stored in Amazon S3. 

As a kick-off, you are going to enable GuardDuty in your AWS account. Let's begin!

1. Go to the [Amazon GuardDuty](https://console.aws.amazon.com/guardduty/home) console.
2. Click on the **Get Started** button.
3. Click on the **Enable GuardDuty** button.  If not present then GuardDuty is already enabled.

{{% notice warning%}}
When you enable GuardDuty for the first time, your account is automatically enrolled in the 30-day free trial for GuardDuty. To learn more, see [Amazon GuardDuty pricing](https://aws.amazon.com/guardduty/pricing/)  
If you are using Event Engine this does not apply.
{{% /notice %}}

GuardDuty is now enabled and will begin monitoring your AWS Account, but before moving on, let's do some additional configurations.

4. You will update the frequency for updated findings, for doing that: Click on **Settings** and under **Findings export options** choose the option *Update CWE and S3 every 15 minutes* and click **Save** 

![GuardDutyFindingsExport](/images/findingsexport.png)

5. Finally, let's verify if **GuardDuty for Amazon S3** is enabled. Go to **Settings** -> **S3 Protection** and verify that the message "S3 Protection is enabled on this account" is shown.

![S3Protection](/images/s3protection.png)

{{% notice note%}}
S3 Protection is enabled by default in all new GuardDuty activations, but if you had GuardDuty enabled before, proceed to activate the S3 Protection. It has an independent 30-days free trial.
{{% /notice %}}