---
title: Rozwiązywanie problemów z odmowa dostępu wiadomości do OneDrive dla witryn biznesowych
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051615"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Rozwiązywanie problemów z odmowa dostępu wiadomości do OneDrive dla witryn biznesowych

Ten problem występuje najczęściej, gdy użytkownik zostanie usunięty i utworzony ponownie z tej samej głównej nazwy użytkownika (UPN). Nowe konto jest tworzone przy użyciu innego PUID (Passport Unique ID) wartość. Gdy użytkownik próbuje uzyskać dostęp do zbioru witryn lub ich OneDrive, użytkownik ma niepoprawny PUID. Drugi scenariusz obejmuje synchronizację katalogów z jednostką organizacyjną (OU) usługi Active Directory. Jeśli użytkownicy już zalogowali się do programu SharePoint, a następnie są przenoszone do innej jednostki organizacyjnej i resynced z programu SharePoint, mogą wystąpić ten problem.

1. Aby rozwiązać ten problem, należy przywrócić oryginalną nazwę UPN z krokami w artykule, [Przywróć użytkownika w pakiecie Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Jeśli nie można przywrócić oryginalnego użytkownika, należy usunąć starego użytkownika z witryny OneDrive, wykonując następujące kroki, [Usuń użytkownika z listy informacji o]()użytkowniku. 
3. Po wykonaniu tej czynności można sprawdzić, czy użytkownik ma uprawnienia administratora do witryny OneDrive, wykonując kroki, aby [dodać administratora dla użytkownika OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Aby uzyskać więcej informacji na temat poziomów uprawnień, zobacz artykuł, [zrozumienie poziomów uprawnień w programie SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
