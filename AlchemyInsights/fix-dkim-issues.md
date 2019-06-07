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
# <a name="fix-dkim-setup-issues"></a>Rozwiąż problemy związane z instalacją DKIM

Jeśli występują problemy z włączeniem DKIM dla domeny niestandardowej, wykonaj następujące kroki:

- Większość problemów z instalacją DKIM odnoszą się do niepoprawne rekordy DNS. Sprawdź, czy rekord DKIM CNAME (**nie** rekord TXT) jest poprawnie sformatowany. Aby uzyskać więcej informacji zobacz w tym [temacie](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Po utworzeniu lub aktualizacji rekordów DKIM DNS na DNS obsługującego usługę dla domeny (zazwyczaj rejestratorem domeny), poczekaj, aż do propagowania rekordy DNS.

- Jeśli rekordy DKIM DNS nie może utworzyć w Centrum administracyjnego, można zastąpić \<CustomDomain\> z niestandardowej domeny (np. contoso.com) i uruchomić to polecenie w [Programie PowerShell Online programu Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
