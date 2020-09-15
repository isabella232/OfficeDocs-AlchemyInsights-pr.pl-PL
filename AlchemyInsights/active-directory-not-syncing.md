---
title: Usługa Active Directory nie jest synchronizowana
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697639"
---
# <a name="active-directory-not-syncing"></a>Usługa Active Directory nie jest synchronizowana

Jeśli otrzymujesz błędy synchronizacji, na przykład "Brak ostatniej synchronizacji", lub Zwróć uwagę, że stan synchronizacji katalogów w portalu Office Admin zawiera komunikat "Ostatnia synchronizacja: ponad 3 dni temu", być może AADConnect ma niepoprawne ustawienia lub nie masz wystarczających uprawnień do przeprowadzenia synchronizacji.  

Ponowna instalacja AADConnect za pomocą ustawień ekspresowych może szybko rozwiązać ten problem:

1. [Pobierz najnowszą wersję programu AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Postępuj zgodnie z instrukcjami dotyczącymi instalacji ekspresowej](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Aby uzyskać więcej informacji na temat kont usługi AADConnect, zobacz [usługa Azure AD Connect: konta i uprawnienia](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
