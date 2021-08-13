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
ms.openlocfilehash: 4bfbe6b2dd9a2112f0cb7af0d6e7a46693bc70680895fd674ddb0332b7071797
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937111"
---
# <a name="active-directory-not-syncing"></a>Nie można zsynchronizować usługi Active Directory

Jeśli otrzymujesz błędy synchronizacji, takie jak "ostatnia synchronizacja", lub zwróć uwagę na stan synchronizacji katalogów w portalu administracyjnym usługi Office "Ostatnia synchronizacja ponad 3 dni temu", może to oznaczać, że program AADConnect ma nieprawidłowe ustawienia lub niewystarczające uprawnienia do przeprowadzenia synchronizacji.  

Ponowne zainstalowanie programu AADConnect przy użyciu ustawień ekspresowych może szybko rozwiązać ten problem:

1. [Pobierz najnowszą wersję programu AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Postępuj zgodnie z instrukcjami dotyczącymi instalacji ekspresowej.](/azure/active-directory/hybrid/how-to-connect-install-express)

Program Azure AD Connect można zainstalować w systemie Windows Server 2012 lub nowszym. Serwer musi być dołączony do domeny i może być kontrolerem domeny lub serwerem członkowskim. Aby uzyskać pełną listę wymagań Połączenie i wymagań wstępnych usługi Azure AD, zapoznaj się z wymaganiami wstępnymi usługi [Azure AD Połączenie.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Aby uzyskać więcej informacji o kontach usługi AADConnect, zobacz Usługa [Azure AD Połączenie: Konta i uprawnienia.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)
