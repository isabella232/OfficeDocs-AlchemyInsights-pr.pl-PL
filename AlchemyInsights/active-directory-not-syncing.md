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
ms.openlocfilehash: d4615d335b9aeef69148cd93ff9f44bec6d7d876
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314214"
---
# <a name="active-directory-not-syncing"></a>Nie można zsynchronizować usługi Active Directory

Jeśli otrzymujesz błędy synchronizacji, takie jak "ostatnia synchronizacja", lub zauważysz stan synchronizacji katalogów w portalu administracyjnym usługi Office "Ostatnia synchronizacja ponad 3 dni temu", może to oznaczać, że program AADConnect ma nieprawidłowe ustawienia lub niewystarczające uprawnienia do przeprowadzenia synchronizacji.  

Ponowne zainstalowanie programu AADConnect przy użyciu ustawień ekspresowych może szybko rozwiązać ten problem:

1. [Pobierz najnowszą wersję programu AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Postępuj zgodnie z instrukcjami dotyczącymi instalacji ekspresowej.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Program Azure AD Connect można zainstalować w systemie Windows Server 2012 lub nowszym. Serwer musi być dołączony do domeny i może być kontrolerem domeny lub serwerem członkowskim. Aby uzyskać pełną listę wymagań Połączenie i wymagań wstępnych usługi Azure AD, zapoznaj się z wymaganiami wstępnymi usługi [Azure AD Połączenie.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Aby uzyskać więcej informacji o kontach usługi AADConnect, zobacz Usługa [Azure AD Połączenie: Konta i uprawnienia.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
