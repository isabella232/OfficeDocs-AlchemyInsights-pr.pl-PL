---
title: Problemy z wydajnością SharePoint lub OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093774"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint lub OneDrive tryb wolny, niedostępny lub niedostępny dla wielu użytkowników

Jeśli witryna OneDrive lub SharePoint nie jest dostępna dla wielu użytkowników, którzy wcześniej mieli do nich dostęp, może wystąpić tymczasowy problem z usługą. [Sprawdź pulpit nawigacyjny kondycji usługi.](https://portal.office.com/adminportal/home#/servicehealth)

**Dodawanie i licencjonowanie użytkownika**

Upewnij się, [że przypiszesz licencje użytkownikom w Microsoft 365 dla firm.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)


**Przypisz uprawnienia**

Jeśli użytkownikowi przypisano licencję programu SharePoint i nadal otrzymuje komunikat o odmowie dostępu, upewnij się, że został mu przypisany [odpowiedni](https://docs.microsoft.com/sharepoint/understanding-permission-levels) poziom uprawnień.

**Rozważ użycie funkcji żądań dostępu**

Funkcja [żądań dostępu umożliwia](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) użytkownikom żądanie dostępu do zawartości, do których obecnie nie mają uprawnień.

**Zezwalaj na skrypty niestandardowe mogą powodować problemy z odmowami dostępu**

W niektórych sytuacjach funkcja Zezwalaj na skrypt *niestandardowy* może przedstawiać odmowa dostępu. Lista funkcji, których dotyczy problem, uwagi dotyczące zabezpieczeń i możliwość jej wyłączenia. Odwiedź stronę [Zezwalanie na skrypt niestandardowy lub uniemożliwianie tego skryptu.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

