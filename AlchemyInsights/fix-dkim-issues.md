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
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506784"
---
# <a name="fix-dkim-setup-issues"></a>Rozwiązywanie problemów z konfiguracją DKIM

Jeśli występują problemy z włączaniem DKIM dla domeny niestandardowej, należy wykonać następujące czynności:

- Większość problemów z konfiguracją DKIM jest związana z niepoprawnymi rekordami DNS. Sprawdź, czy rekord CNAME DKIM **(nie** rekord TXT) jest poprawnie sformatowany. Aby uzyskać więcej informacji, zobacz ten [temat](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Po utworzeniu lub zaktualizowaniu rekordów DNS DKIM w usłudze hostingu DNS dla domeny (zazwyczaj rejestratora domen) poczekaj na propagowanie rekordów DNS.

- Jeśli nie można utworzyć rekordów DNS DKIM w centrum administracyjnym, możesz zastąpić \<CustomDomain\> domeną niestandardową (na przykład contoso.com) i uruchomić to polecenie w [programie Exchange Online PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
