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
# <a name="fix-dkim-setup-issues"></a>Rozwiązywanie problemów z konfiguracją DKIM

Jeśli występują problemy z włączaniem DKIM dla domeny niestandardowej, należy wykonać następujące czynności:

- Większość problemów z konfiguracją DKIM jest związana z niepoprawnymi rekordami DNS. Sprawdź, czy rekord CNAME DKIM **(nie** rekord TXT) jest poprawnie sformatowany. Aby uzyskać więcej informacji, zobacz ten [temat](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Po utworzeniu lub zaktualizowaniu rekordów DNS DKIM w usłudze hostingu DNS dla domeny (zazwyczaj rejestratora domen) poczekaj na propagowanie rekordów DNS.

- Jeśli nie można utworzyć rekordów DNS DKIM w centrum \<administracyjnym, możesz zastąpić\> Domenę Niestandardową domeną niestandardową (na przykład contoso.com) i uruchomić to polecenie w [programie Exchange Online PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
