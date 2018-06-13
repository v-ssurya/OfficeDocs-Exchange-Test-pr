﻿---
title: 'DLP policy templates: Exchange 2013 Help'
TOCTitle: DLP policy templates
ms:assetid: c7b1a8e4-30d9-4409-85c5-f85ae023737d
ms:mtpsurl: https://technet.microsoft.com/en-us/library/JJ657730(v=EXCHG.150)
ms:contentKeyID: 49300690
ms.date: 12/10/2017
mtps_version: v=EXCHG.150
---

# DLP policy templates

 

_**Applies to:** Exchange Online, Exchange Server 2013_


You can use data loss prevention (DLP) policy templates to get started with your DLP solution in Microsoft Exchange 2013. A DLP policy template is a model for a policy. You can select a template to begin the process of building your own customized DLP policy. Within your DLP policy, you can customize the rules to ensure that it meets your business needs for data loss prevention. Several policy templates are supplied by Microsoft, but these are not the only way to implement a data loss prevention solution in Exchange.

Looking for management tasks related to DLP policy templates? See [DLP procedures](dlp-procedures-exchange-2013-help.md).

**Contents**

Extend the templates and information types to meet your needs

Create your own new DLP policy template

Include DLP functionality with existing transport rules

Use DLP policies created by Microsoft

For more information

## Extend the templates and information types to meet your needs

You can incorporate sensitive-content definitions and policy templates from Microsoft Partners or from files that you develop yourself as an addition to the DLP policy templates, information types, and rules already provided in Exchange 2013. Presented here are several ways in which you can add your own unique DLP content and extend DLP functionality. The templates already provided by Microsoft are a convenient method to get started with a DLP solution. In order to extend the DLP features with your own unique DLP policy template files, you must understand the XML schema requirements for policy templates that are created independent of Exchange. To learn more about the Exchange Management Shell cmdlets associated with DLP policy templates, see cmdlets related to `Get-DlpPolicyTemplate` in [Policy and compliance cmdlets](https://technet.microsoft.com/en-us/library/dd298082\(v=exchg.150\)). Furthermore, you can define your own sensitive content types after you understand the format and procedure to incorporate them. To learn more about the Exchange Management Shell cmdlets associated with DLP policy templates, see cmdlets related to `Get-ClassificationRuleCollection` in [Policy and compliance cmdlets](https://technet.microsoft.com/en-us/library/dd298082\(v=exchg.150\)).


> [!WARNING]
> You should turn on your DLP policies in test mode before enforcing them in your production environment. During such tests, we recommended that you configure sample user mailboxes and send test messages that invoke your test policies in order to confirm the results.



## Create your own new DLP policy template or your own sensitive information types in a classification rule package

You can create a DLP policy template file apart from Exchange that meets the specific XML schema definition provided by Microsoft and then import the file into your system so that you can create DLP policies from it. By creating your own template files, you can define your own model for DLP policies that Microsoft has not already provided. This is different than creating a DLP policy by using the Exchange Administration Center, which typically happens after policy templates are available. If you create a policy template independent of Exchange, you will need to import it before you can use it to scan messages. You can also create your own sensitive information definitions apart from those defined by Microsoft in Exchange. There is a separate XML schema definition for DLP policy template files and classification rule packages. To get started with this, see the following information:

  -  
    [Define your own DLP templates and information types](define-your-own-dlp-templates-and-information-types-exchange-2013-help.md)

  -  
    [Import a custom DLP policy template from a file](import-a-custom-dlp-policy-template-from-a-file-exchange-2013-help.md)

## Include DLP functionality with existing transport rules

You can incorporate DLP detection capabilities with traditional transport rules without creating a new DLP policy. If you have created a complex set of rules in a previous version of Exchange, and you want to duplicate them or add sensitive information detection in Exchange 2013, then you can use the transport rules editor in the Exchange Administration Center or the Exchange management shell to incorporate these two features. To get started with this, see the following information:

  -  
    [Mail flow rules (transport rules) in Exchange 2013](mail-flow-rules-transport-rules-in-exchange-2013-exchange-2013-help.md) (Exchange Server 2013)

  -  
    [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/en-us/library/jj919238\(v=exchg.150\)) (Exchange Online)

  -  
    [Manage mail flow rules](manage-mail-flow-rules-exchange-2013-help.md)
    
    [Policy and compliance cmdlets](https://technet.microsoft.com/en-us/library/dd298082\(v=exchg.150\))

## Use DLP policies created by Microsoft

Numerous DLP policies are supplied by Microsoft. This is the easiest way to get started with a DLP solution that is flexible and simple to implement. You can always use the provided policies as a starting point and customize them further to meet your requirements. To get started with this, see the following information:

  - [DLP policy templates supplied in Exchange](dlp-policy-templates-supplied-in-exchange-exchange-2013-help.md)

  - [Create a DLP policy from a template](how-to-new-dlp-data-loss-prevention-policy-template.md)

## For more information

[Data loss prevention](technical-overview-of-dlp-data-loss-prevention-in-exchange.md)
