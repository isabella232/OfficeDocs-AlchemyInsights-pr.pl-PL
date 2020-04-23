---
title: 929 Reguły skrzynki odbiorczej, aby odwrócićprzemysłowetransportu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 6b6e64c0332a579e8f6132b08f2f89b15eb4de27
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43724602"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="0a772-102">Reguły przepływu poczty (znane również jako reguły transportu)</span><span class="sxs-lookup"><span data-stu-id="0a772-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="0a772-103">Ogólne omówienie reguł przepływu poczty: [reguły przepływu poczty (reguły transportu) w usłudze Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="0a772-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="0a772-104">Konfigurowanie reguł przepływu poczty: [Procedury reguł przepływu poczty w usłudze Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="0a772-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="0a772-105">Tworzenie, modyfikowanie i usuwanie reguł przepływu poczty: [zarządzanie regułami przepływu poczty](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="0a772-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="0a772-106">Reguły przepływu poczty można również zarządzać w programie Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0a772-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="0a772-107">Aby uzyskać więcej informacji, zobacz [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (widok), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (zmodyfikuj istniejące), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (wyłącz istniejące) i [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (włącz istniejące).</span><span class="sxs-lookup"><span data-stu-id="0a772-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="0a772-108">Dodatkowe polecenia cmdlet reguł przepływu poczty: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (lista dostępnych akcji), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (lista dostępnych warunków i wyjątków), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (reguły eksportu) i [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (reguły importu).</span><span class="sxs-lookup"><span data-stu-id="0a772-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
