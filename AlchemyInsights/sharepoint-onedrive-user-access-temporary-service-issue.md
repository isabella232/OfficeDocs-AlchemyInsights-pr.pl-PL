---
title: Problemy z wydajnością — program SharePoint lub usługa OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771254"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>Program SharePoint lub usługa OneDrive jest wolny, niedostępny lub niedostępny dla wielu użytkowników

Jeśli witryna OneDrive lub SharePoint nie jest dostępna dla wielu użytkowników, którzy wcześniej mieli dostęp, może to oznaczać, że wystąpił tymczasowy problem z usługą. [Sprawdź pulpit nawigacyjny kondycji usługi](https://portal.office.com/adminportal/home#/servicehealth).

**Dodawanie i Licencjonowanie użytkownika**

Upewnij się, że [przypisujesz licencje użytkownikom w systemie Microsoft 365 dla firm](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Przypisywanie uprawnień**

Jeśli użytkownikowi przypisano licencję programu SharePoint i nadal otrzymujesz komunikat o odmowie dostępu, upewnij się, że ma przypisany [odpowiedni poziom uprawnień](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .

**Korzystanie z funkcji żądania dostępu**

[Funkcja żądania dostępu](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) umożliwia użytkownikom żądanie dostępu do zawartości, do której nie mają obecnie uprawnień.

**Zezwalaj na skrypt niestandardowy może powodować problemy z odmową dostępu**

Istnieją pewne scenariusze, w których funkcja *Zezwalaj na skrypt niestandardowy* może stanowić odmowę dostępu. Aby uzyskać listę funkcji, których dotyczy problem, zagadnienia dotyczące zabezpieczeń i możliwość wyłączenia funkcji. Zobacz [Zezwalanie lub zapobieganie skryptowi niestandardowemu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

