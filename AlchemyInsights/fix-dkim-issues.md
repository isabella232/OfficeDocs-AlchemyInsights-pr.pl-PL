---
title: Rozwiąż problemy związane z instalacją DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765285"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="6bfb1-102">Rozwiąż problemy związane z instalacją DKIM</span><span class="sxs-lookup"><span data-stu-id="6bfb1-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="6bfb1-103">Jeśli występują problemy z włączeniem DKIM dla domeny niestandardowej, wykonaj następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="6bfb1-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="6bfb1-104">Większość problemów z instalacją DKIM odnoszą się do niepoprawne rekordy DNS.</span><span class="sxs-lookup"><span data-stu-id="6bfb1-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="6bfb1-105">Sprawdź, czy rekord DKIM CNAME (**nie** rekord TXT) jest poprawnie sformatowany.</span><span class="sxs-lookup"><span data-stu-id="6bfb1-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="6bfb1-106">Aby uzyskać więcej informacji zobacz w tym [temacie](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="6bfb1-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="6bfb1-107">Po utworzeniu lub aktualizacji rekordów DKIM DNS na DNS obsługującego usługę dla domeny (zazwyczaj rejestratorem domeny), poczekaj, aż do propagowania rekordy DNS.</span><span class="sxs-lookup"><span data-stu-id="6bfb1-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="6bfb1-108">Jeśli rekordy DKIM DNS nie może utworzyć w Centrum administracyjnego, można zastąpić \<CustomDomain\> z niestandardowej domeny (np. contoso.com) i uruchomić to polecenie w [Programie PowerShell Online programu Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="6bfb1-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
