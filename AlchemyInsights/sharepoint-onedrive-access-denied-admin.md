---
title: Rozwiązywanie problemów z wiadomościami odmowa dostępu
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760350"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Rozwiązywanie problemów z wiadomościami odmowa dostępu w Centrum administracyjnego programu Sharepoint/OneDrive

Jeśli otrzymujesz podczas próby przejdź do Centrum administracyjnego programu Sharepoint/OneDrive komunikat o odmowie dostępu, upewnij się, że możesz [przypisać jedną licencję do użytkownika](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Jeśli użytkownik ma licencję, należy również upewnij się, że są one [przypisaną rolę administratora](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) można uzyskać dostęp do centrów admin.

Ten problem może również wystąpić, gdy użytkownik jest usunięty i utworzony ponownie z samą główną nazwę użytkownika (UPN). Nowe konto jest tworzone przy użyciu różnych wartości PUID (unikatowy identyfikator usługi Passport). Gdy użytkownik próbuje uzyskać dostęp do zbioru witryn lub ich OneDrive, użytkownik ma niepoprawne PUID. Drugi scenariusz obejmuje synchronizacji katalogów z jednostki organizacyjnej (OU) usługi Active Directory. Jeśli użytkownicy mają już zarejestrowany w programie SharePoint, a następnie są przenoszone do innej jednostki Organizacyjnej i resynced z programem SharePoint, mogą oni napotkać ten problem.

Aby rozwiązać ten problem, należy przywrócić oryginalny UPN czynności opisanych w artykule, [przywracania przez użytkownika w usłudze Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Uwaga: Jeśli Centrum OneDrive lub administracji programu SharePoint nie jest dostępne dla wielu użytkowników, którzy uprzednio uzyskiwała dostęp, może istnieć problem tymczasowej usługi.  [Sprawdź pulpit nawigacyjny kondycji usługi](https://portal.office.com/adminportal/home#/servicehealth).


