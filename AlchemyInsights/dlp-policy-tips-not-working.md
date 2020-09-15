---
title: Porady dotyczące zasad DLP nie działają
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 1e1f9b84cb8bd07468d3da0eeaff3716b9a309a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679595"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="566bd-102">Porady dotyczące zasad DLP</span><span class="sxs-lookup"><span data-stu-id="566bd-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="566bd-103">**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="566bd-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="566bd-104">**Porady dotyczące zasad DLP**</span><span class="sxs-lookup"><span data-stu-id="566bd-104">**DLP policy tips**</span></span>

<span data-ttu-id="566bd-105">W przypadku korzystania z **zasad DLP**użytkownicy mogą być powiadamiani o naruszeniu zasad z **poradami dotyczącymi zasad**.</span><span class="sxs-lookup"><span data-stu-id="566bd-105">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="566bd-106">Administratorzy mogą skonfigurować porady dotyczące zasad, które będą wyświetlane podczas testowania zasad DLP lub gdy zasady są w trybie pełnego wymuszania.</span><span class="sxs-lookup"><span data-stu-id="566bd-106">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="566bd-107">Aby skonfigurować porady dotyczące zasad DLP w centrum zabezpieczeń i zgodności w trybie pełnego wymuszania, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="566bd-107">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="566bd-108">Upewnij się, że w regule DLP **włączono** porady dotyczące zasad, wykonując kroki opisane [tutaj](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="566bd-108">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="566bd-109">Upewnij się, że **zawartość jest zgodna** z tym, co jest **wymagane** do uruchomienia reguły przedkreślonej w [tym artykule.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="566bd-109">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="566bd-110">Porady dotyczące zasad są wyświetlane zarówno w programie OWA, jak i w programie Outlook.</span><span class="sxs-lookup"><span data-stu-id="566bd-110">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="566bd-111">Jednak w przypadku korzystania z **programu Outlook 2013 lub nowszego**porady dotyczące zasad są wyświetlane tylko w określonych warunkach.</span><span class="sxs-lookup"><span data-stu-id="566bd-111">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="566bd-112">Te warunki wymieniono poniżej: [obsługiwane warunki dotyczące programu Outlook 2013 lub nowszego do wyświetlania porad dotyczących zasad](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="566bd-112">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span></span>

<span data-ttu-id="566bd-113">Aby uzyskać dodatkowe informacje na temat wskazówek dotyczących zasad DLP, zobacz: [Pokazywanie porad dotyczących zasad dla zasad DLP](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="566bd-113">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span></span>
  