---
title: Brakujące wiadomości e-mail w kwarantannie
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: bd5a04fd5abad962b4e85e009a9232e1a93219c238c629506df5cfb034453df2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892057"
---
# <a name="missing-emails-in-quarantine"></a>Brakujące wiadomości e-mail w kwarantannie

Administratorzy [mogą wyświetlać, zwalniać lub usuwać te wiadomości](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

W portalu Microsoft 365 Defender podpowiem <https://security.microsoft.com> przejdź do **recenzji** \> **Kwarantanna**. Aby przejść bezpośrednio do strony **kwarantanny,** użyj <https://security.microsoft.com/quarantine> .  

Aby uzyskać więcej informacji na temat wartości wyszukiwania/filtrowania, których można użyć, zobacz Zarządzanie wiadomościami i plikami poddanymi kwarantannie jako administrator w u [administratorach usługi EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Polecenia cmdlet, których używasz do wyświetlania wiadomości i plików w kwarantannie oraz zarządzania nimi w kwarantannie, to:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)To polecenie cmdlet jest tylko dla wiadomości, a nie plików z załączników programu Sejf dla plików SharePoint, OneDrive lub Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
