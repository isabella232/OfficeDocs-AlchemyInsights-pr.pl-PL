---
title: Niesynchronizowanie usługi Active Directory
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265266"
---
# <a name="active-directory-not-syncing"></a>Niesynchronizowanie usługi Active Directory

Jeśli otrzymujesz błędy synchronizacji, takie jak "brak niedawnej synchronizacji" lub zauważysz stan synchronizacji katalogów w portalu administracyjnym pakietu Office mówi: "Ostatnia synchronizacja sprzed ponad 3 dni", może się okazać, że AADConnect ma nieprawidłowe ustawienia lub niewystarczające uprawnienia do wykonywania synchronizacji.  

Ponowna instalacja usługi AADConnect przy użyciu ustawień ekspresowych może szybko rozwiązać problem:

1. [Pobierz najnowszą wersję AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Postępuj zgodnie z instrukcjami dotyczącymi instalacji ekspresowej](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Aby uzyskać więcej informacji o kontach usług AADConnect, zobacz [Azure AD Connect: Konta i uprawnienia](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
