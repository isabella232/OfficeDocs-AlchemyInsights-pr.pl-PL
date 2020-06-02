---
title: Rozwiązywanie problemów z odmową dostępu do wiadomości do witryn usługi OneDrive dla Firm
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511194"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Rozwiązywanie problemów z odmową dostępu do wiadomości do witryn usługi OneDrive dla Firm

Ten problem najczęściej występuje, gdy użytkownik jest usuwany i ponownie tworzony przy tej samej głównej nazwie użytkownika (UPN). Nowe konto jest tworzone przy użyciu innej wartości PUID (Passport Unique ID). Gdy użytkownik próbuje uzyskać dostęp do zbioru witryn lub ich OneDrive, użytkownik ma niepoprawny PUID. Drugi scenariusz obejmuje synchronizację katalogów z jednostką organizacyjną usługi Active Directory.A second scenario involves directory synchronizacji with an Active Directory organizational unit (OU). Jeśli użytkownicy już zalogowali się do programu SharePoint, a następnie zostaną przeniesieni do innej usługi organizacyjnej i ponownie zsynchronizowani za pomocą programu SharePoint, może wystąpić ten problem.

1. Aby rozwiązać ten problem, należy przywrócić oryginalną nazwy UPN z krokami opisanymi w artykule, [Przywróć użytkownika w usłudze Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Jeśli nie można przywrócić oryginalnego użytkownika, należy usunąć starego użytkownika z witryny usługi OneDrive, wykonując te kroki, [Usuń użytkownika z listy informacji o użytkowniku](). 
3. Po wykonaniu tej czynności możesz sprawdzić, czy użytkownik ma prawa administratora do witryny usługi OneDrive, wykonując kroki, aby [dodać administratora dla usługi OneDrive użytkownika](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Aby uzyskać więcej informacji na temat poziomów uprawnień, zobacz artykuł [Opis poziomów uprawnień w programie SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
