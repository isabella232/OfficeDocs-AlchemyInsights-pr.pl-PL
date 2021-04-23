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
ms.openlocfilehash: 8a3b8175c077b77d1c9b5d859012faddcb1fa3a0
ms.sourcegitcommit: 099704f7f4bdf122d09bb4f7cc71d36fc77a7fcf
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2021
ms.locfileid: "51958712"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="b681a-102">Problemy dotyczące porad dotyczących zasad DLP</span><span class="sxs-lookup"><span data-stu-id="b681a-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="b681a-103">**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="b681a-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="b681a-104">Aby skonfigurować porady dotyczące zasad DLP w Centrum zabezpieczeń i & w trybie pełnego wymuszania, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="b681a-104">To configure policy tips on your DLP policy in the Security & Compliance center in full enforcement mode, do the following:</span></span>

- <span data-ttu-id="b681a-105">Upewnij się, że dla reguły DLP **włączono** porady dotyczące zasad.</span><span class="sxs-lookup"><span data-stu-id="b681a-105">Ensure policy tips have been **enabled** on the DLP rule.</span></span> <span data-ttu-id="b681a-106">Aby uzyskać instrukcje, [zobacz Wysyłanie powiadomień e-mail i wyświetlanie porad dotyczących zasad DLP.](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="b681a-106">For steps, see [Send email notifications and show policy tips for DLP policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="b681a-107">Upewnij się, że zawartość jest do tego wymagana, aby wyzwolić regułę podaną w definicjach [encji typu informacji poufnych.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="b681a-107">Ensure your content matches what is required to trigger the rule outlined in [Sensitive information type entity definitions](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="b681a-108">Porady dotyczące zasad są wyświetlane zarówno w aplikacji OWA, jak i w programie Outlook.</span><span class="sxs-lookup"><span data-stu-id="b681a-108">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="b681a-109">Jednak w przypadku korzystania z programu Outlook 2013 lub nowszego porady dotyczące zasad są wyświetlane tylko w określonych warunkach.</span><span class="sxs-lookup"><span data-stu-id="b681a-109">However, when using Outlook 2013 or later, policy tips are displayed only under certain conditions.</span></span> <span data-ttu-id="b681a-110">Aby uzyskać listę określonych warunków, zobacz Obsługiwane warunki dla programu [Outlook 2013](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)lub nowszego, aby uzyskać porady dotyczące zasad.</span><span class="sxs-lookup"><span data-stu-id="b681a-110">For the specific conditions list, see [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

<span data-ttu-id="b681a-111">Aby uzyskać informacje na temat porad dotyczących zasad [DLP,](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) zobacz Informacje na temat porad dotyczących zasad DLP i Macierz pomocy technicznej [dla porad dotyczących zasad DLP.](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps)</span><span class="sxs-lookup"><span data-stu-id="b681a-111">For information on DLP Policy tips, see [DLP Policy Tips Reference](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) and [Support Matrix for DLP Policy tips](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps).</span></span>