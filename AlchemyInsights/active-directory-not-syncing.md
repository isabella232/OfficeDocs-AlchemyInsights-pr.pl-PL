---
title: Nie można zsynchronizować usługi Active Directory
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
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930985"
---
# <a name="active-directory-not-syncing"></a>Nie można zsynchronizować usługi Active Directory

Jeśli otrzymujesz błędy synchronizacji, takie jak "ostatnia synchronizacja", lub zwróć uwagę na stan synchronizacji katalogów w portalu administracyjnym usługi Office "Ostatnia synchronizacja ponad 3 dni temu", może to oznaczać, że program AADConnect ma nieprawidłowe ustawienia lub niewystarczające uprawnienia do przeprowadzenia synchronizacji.  

Ponowne zainstalowanie programu AADConnect przy użyciu ustawień ekspresowych może szybko rozwiązać ten problem:

1. [Pobierz najnowszą wersję programu AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Postępuj zgodnie z instrukcjami dotyczącymi instalacji ekspresowej.](/azure/active-directory/hybrid/how-to-connect-install-express)

Program Azure AD Connect można zainstalować w systemie Windows Server 2012 lub nowszym. Serwer musi być dołączony do domeny i może być kontrolerem domeny lub serwerem członkowskim. Aby uzyskać pełną listę wymagań Połączenie i wymagań wstępnych usługi Azure AD, zapoznaj się z wymaganiami wstępnymi usługi [Azure AD Połączenie.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Aby uzyskać więcej informacji o kontach usługi AADConnect, zobacz Usługa [Azure AD Połączenie: Konta i uprawnienia.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)
