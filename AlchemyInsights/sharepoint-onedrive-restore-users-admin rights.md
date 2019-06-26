---
title: Rozwiązywanie problemów z dostępem odmowa wiadomości do OneDrive dla witryn biznesu
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: b394cc1441187133d8829cfc5fb0c1edbd71fd96
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223434"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Rozwiązywanie problemów z dostępem odmowa wiadomości do OneDrive dla witryn biznesu

Ten problem najczęściej występuje, gdy użytkownik jest usunięty i utworzony ponownie z samą główną nazwę użytkownika (UPN). Nowe konto jest tworzone przy użyciu różnych wartości PUID (unikatowy identyfikator usługi Passport). Gdy użytkownik próbuje uzyskać dostęp do zbioru witryn lub ich OneDrive, użytkownik ma niepoprawne PUID. Drugi scenariusz obejmuje synchronizacji katalogów z jednostki organizacyjnej (OU) usługi Active Directory. Jeśli użytkownicy mają już zarejestrowany w programie SharePoint, a następnie są przenoszone do innej jednostki Organizacyjnej i resynced z programem SharePoint, mogą oni napotkać ten problem.

Aby rozwiązać ten problem, należy przywrócić oryginalny UPN czynności opisanych w artykule,[przywracania przez użytkownika w usłudze Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Po tej czynności można sprawdzić, czy użytkownik posiada uprawnienia administratora do witryny OneDrive przez wykonanie kroków do [administratora Dodaj użytkownika dla użytkownika OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Aby uzyskać więcej informacji dotyczących poziomów uprawnień zobacz artykuł, [Opis poziomów uprawnień w programie SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
