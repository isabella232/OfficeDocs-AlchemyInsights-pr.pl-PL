---
title: Rozwiązywanie problemów dotyczących konfiguracji DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744960"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="5ed06-102">Rozwiązywanie problemów dotyczących konfiguracji DKIM</span><span class="sxs-lookup"><span data-stu-id="5ed06-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="5ed06-103">Jeśli występują problemy z włączeniem DKIM dla domeny niestandardowej, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="5ed06-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="5ed06-104">Większość DKIMych problemów dotyczących konfiguracji dotyczy niepoprawnych rekordów DNS.</span><span class="sxs-lookup"><span data-stu-id="5ed06-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="5ed06-105">Sprawdź, czy rekord CNAME DKIM (**nie** rekord TXT) jest sformatowany poprawnie.</span><span class="sxs-lookup"><span data-stu-id="5ed06-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="5ed06-106">Aby uzyskać więcej informacji, zobacz ten [temat](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="5ed06-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="5ed06-107">Po utworzeniu lub zaktualizowaniu rekordów DNS DKIM w usłudze hostingu DNS dla domeny (zazwyczaj Rejestratorowi domen) Poczekaj, aż rekordy DNS zostaną rozpropagowane.</span><span class="sxs-lookup"><span data-stu-id="5ed06-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="5ed06-108">Jeśli nie możesz utworzyć rekordów DNS DKIM w centrum administracyjnym, możesz zastąpić \<CustomDomain\> domenę niestandardową (na przykład contoso.com) i uruchomić to polecenie w usłudze [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="5ed06-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
