---
title: Rozwiązywanie problemów z komunikatami odmowa dostępu
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751286"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Rozwiązywanie problemów z odmową dostępu wiadomości w centrum administracyjnym programu SharePoint/OneDrive

Jeśli otrzymujesz komunikat o odmowie dostępu podczas próby przejdź do centrum administracyjnego programu SharePoint/OneDrive, upewnij się, że [przypisać licencję do użytkownika](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Jeśli użytkownik ma licencję, należy również upewnić się, że [przypisano rolę administratora](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , która może uzyskiwać dostęp do centrów administracyjnych.

Ten problem może również wystąpić, gdy użytkownik zostanie usunięty i utworzony ponownie z tej samej głównej nazwy użytkownika (UPN). Nowe konto jest tworzone przy użyciu innego PUID (Passport Unique ID) wartość. Gdy użytkownik próbuje uzyskać dostęp do zbioru witryn lub ich OneDrive, użytkownik ma niepoprawny PUID. Drugi scenariusz obejmuje synchronizację katalogów z jednostką organizacyjną (OU) usługi Active Directory. Jeśli użytkownicy już zalogowali się do programu SharePoint, a następnie są przenoszone do innej jednostki organizacyjnej i resynced z programu SharePoint, mogą wystąpić ten problem.

Aby rozwiązać ten problem, należy przywrócić oryginalną nazwę UPN z krokami w artykule, [Przywróć użytkownika w pakiecie Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Uwaga: Jeśli centrum administracyjnego usługi OneDrive lub programu SharePoint nie jest dostępne dla wielu użytkowników, którzy wcześniej mieli dostęp, może to być problem z usługą tymczasową.  [Sprawdź pulpit nawigacyjny kondycji usługi](https://portal.office.com/adminportal/home#/servicehealth).


