---
title: Rozwiązywanie problemów z konfiguracją DKIM
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
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945941"
---
# <a name="fix-dkim-setup-issues"></a>Rozwiązywanie problemów z konfiguracją DKIM

Jeśli wystąpią problemy podczas włączania funkcji DKIM dla domeny niestandardowej, należy wykonać następujące czynności:

- Większość problemów z konfiguracją DKIM jest związanych z niepoprawnymi rekordami DNS. Sprawdź, czy rekord CNAME DKIM **(a** nie rekord TXT) został poprawnie sformatowany. Aby uzyskać więcej informacji, zobacz ten [temat.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

- Po utworzeniu lub zaktualizowaniu rekordów DNS DKIM w usłudze hostingu DNS domeny (zwykle rejestratora domen) poczekaj na propagację rekordów DNS.

- Jeśli nie możesz utworzyć rekordów DNS DKIM w centrum administracyjnym, możesz zastąpić domenę niestandardową (na przykład contoso.com) i uruchomić to polecenie w programie \<CustomDomain\> [Exchange Online PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
