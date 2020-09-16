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
# <a name="fix-dkim-setup-issues"></a>Rozwiązywanie problemów dotyczących konfiguracji DKIM

Jeśli występują problemy z włączeniem DKIM dla domeny niestandardowej, wykonaj następujące czynności:

- Większość DKIMych problemów dotyczących konfiguracji dotyczy niepoprawnych rekordów DNS. Sprawdź, czy rekord CNAME DKIM (**nie** rekord TXT) jest sformatowany poprawnie. Aby uzyskać więcej informacji, zobacz ten [temat](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Po utworzeniu lub zaktualizowaniu rekordów DNS DKIM w usłudze hostingu DNS dla domeny (zazwyczaj Rejestratorowi domen) Poczekaj, aż rekordy DNS zostaną rozpropagowane.

- Jeśli nie możesz utworzyć rekordów DNS DKIM w centrum administracyjnym, możesz zastąpić \<CustomDomain\> domenę niestandardową (na przykład contoso.com) i uruchomić to polecenie w usłudze [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
