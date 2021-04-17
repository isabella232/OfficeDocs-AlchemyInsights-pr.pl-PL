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
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822861"
---
# <a name="active-directory-not-syncing"></a>Nie można zsynchronizować usługi Active Directory

Jeśli otrzymujesz błędy synchronizacji, takie jak "nie masz ostatniej synchronizacji", lub zwróć uwagę na stan synchronizacji katalogów w portalu administracyjnym pakietu Office o treści "Ostatnia synchronizacja ponad 3 dni temu", może to oznaczać, że program AADConnect ma nieprawidłowe ustawienia lub niewystarczające uprawnienia do przeprowadzenia synchronizacji.  

Ponowne zainstalowanie programu AADConnect przy użyciu ustawień ekspresowych może szybko rozwiązać ten problem:

1. [Pobierz najnowszą wersję programu AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Postępuj zgodnie z instrukcjami dotyczącymi instalacji ekspresowej.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Aby uzyskać więcej informacji o kontach usługi AADConnect, zobacz [Azure AD Connect: konta i uprawnienia.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
