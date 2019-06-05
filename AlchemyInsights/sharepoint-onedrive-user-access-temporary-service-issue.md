---
title: Wydajność problemów programu SharePoint lub OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719526"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint lub OneDrive wolno, niedostępne lub niedostępny dla wielu użytkowników

Jeśli witryny programu SharePoint lub OneDrive nie jest dostępny dla wielu użytkowników, którzy uprzednio uzyskiwała dostęp, może to być problem tymczasowy usługi. [Sprawdź pulpit nawigacyjny kondycji usługi](https://portal.office.com/adminportal/home#/servicehealth).

## <a name="add-and-license-the-user"></a>Dodaj i licencję użytkownika

Zapewnić, że można [przypisywać licencje dla użytkowników w usłudze Office 365 dla firm](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


## <a name="assign-permissions"></a>Przypisywanie uprawnień

Jeśli użytkownik został przypisany licencji programu Sharepoint i nadal otrzymuje komunikat o odmowie dostępu, upewnij się, że mają [odpowiedni poziom uprawnień](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) przypisanych.

## <a name="consider-using-the-access-request-feature"></a>Należy rozważyć użycie funkcji żądania dostępu

[Funkcja żądania dostępu](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) umożliwia osobom na żądanie dostępu do treści, które aktualnie nie mają uprawnień do przeglądania.

## <a name="allow-custom-script-may-cause-access-denied-issues"></a>Zezwalanie na skrypt niestandardowy może powodować problemów odmowa dostępu

Istnieją pewne scenariusze, gdzie może prezentować funkcja *Zezwalaj na skrypty niestandardowe* o odmowie dostępu. Aby uzyskać listę funkcji, których dotyczy problem, zagadnienia dotyczące zabezpieczeń i możliwości, aby wyłączyć tę funkcję. Przejdź do strony [Zezwalaj lub zapobiegania niestandardowy skrypt](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).

