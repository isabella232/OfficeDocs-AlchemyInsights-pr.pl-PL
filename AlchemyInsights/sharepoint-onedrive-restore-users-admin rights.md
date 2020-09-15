---
title: Rozwiązywanie problemów z odmową dostępu wiadomości do witryn usługi OneDrive dla firm
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670626"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Rozwiązywanie problemów z odmową dostępu wiadomości do witryn usługi OneDrive dla firm

Ten problem występuje najczęściej, gdy użytkownik jest usuwany i tworzony ponownie przy użyciu tej samej głównej nazwy użytkownika (UPN). Nowe konto jest tworzone przy użyciu innej wartości identyfikatora PUID (unikatowy identyfikator paszportu). Gdy użytkownik usiłuje uzyskać dostęp do zbioru witryn lub jego usługi OneDrive, użytkownik ma nieprawidłowy identyfikator PUID. Drugi scenariusz obejmuje synchronizację katalogów za pomocą jednostki organizacyjnej (OU) Active Directory. Jeśli użytkownicy już zalogowali się do programu SharePoint, a następnie zostaną przesunięte do innej jednostki organizacyjnej i ponownie zsynchronizowane z programem SharePoint, mogą wystąpić ten problem.

1. Aby rozwiązać ten problem, należy przywrócić oryginalną główną nazwę użytkownika, wykonując czynności opisane w artykule, [przywracanie użytkownika w programie Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Jeśli nie można przywrócić oryginalnego użytkownika, należy usunąć starego użytkownika z witryny usługi OneDrive, wykonując poniższe czynności, [a następnie usunąć użytkownika z listy informacje o użytkowniku](). 
3. Po wykonaniu tej czynności można sprawdzić, czy użytkownik ma uprawnienia administratora witryny usługi OneDrive, wykonując kroki opisane w temacie [Dodawanie administratora do usługi OneDrive użytkownika](https://docs.microsoft.com/sharepoint/manage-user-profiles) .

Aby uzyskać więcej informacji na temat poziomów uprawnień, zobacz artykuł [Opis poziomów uprawnień w programie SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
