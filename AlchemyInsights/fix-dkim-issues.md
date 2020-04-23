---
title: Rozwiązywanie problemów z konfiguracją DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717572"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="c6e02-102">Rozwiązywanie problemów z konfiguracją DKIM</span><span class="sxs-lookup"><span data-stu-id="c6e02-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="c6e02-103">Jeśli występują problemy z włączaniem DKIM dla domeny niestandardowej, należy wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="c6e02-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="c6e02-104">Większość problemów z konfiguracją DKIM jest związana z niepoprawnymi rekordami DNS.</span><span class="sxs-lookup"><span data-stu-id="c6e02-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="c6e02-105">Sprawdź, czy rekord CNAME DKIM **(nie** rekord TXT) jest poprawnie sformatowany.</span><span class="sxs-lookup"><span data-stu-id="c6e02-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="c6e02-106">Aby uzyskać więcej informacji, zobacz ten [temat](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="c6e02-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="c6e02-107">Po utworzeniu lub zaktualizowaniu rekordów DNS DKIM w usłudze hostingu DNS dla domeny (zazwyczaj rejestratora domen) poczekaj na propagowanie rekordów DNS.</span><span class="sxs-lookup"><span data-stu-id="c6e02-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="c6e02-108">Jeśli nie można utworzyć rekordów DNS DKIM w centrum \<administracyjnym, możesz zastąpić\> Domenę Niestandardową domeną niestandardową (na przykład contoso.com) i uruchomić to polecenie w [programie Exchange Online PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="c6e02-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
