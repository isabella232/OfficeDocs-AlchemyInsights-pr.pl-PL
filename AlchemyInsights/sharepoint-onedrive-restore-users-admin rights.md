---
title: Rozwiązywanie problemów z komunikatami o odmowie dostępu OneDrive dla Firm witryn
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
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957803"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Rozwiązywanie problemów z komunikatami o odmowie dostępu OneDrive dla Firm witryn

Ten problem najczęściej występuje, gdy użytkownik jest usuwany i ponownie tworzony przy użyciu tej samej głównej nazwy użytkownika (UPN). Nowe konto jest tworzone przy użyciu innej wartości identyfikatora PUID (Passport Unique ID). Gdy użytkownik próbuje uzyskać dostęp do zbioru witryn lub swojego OneDrive, ma nieprawidłowy identyfikator PUID. Drugi scenariusz obejmuje synchronizację katalogów z jednostką organizacyjną usługi Active Directory. Jeśli użytkownicy już zalogowali się do usługi SharePoint, a następnie zostaną przeniesioni do innej usługi OU i ponownie zsynchroniznini z programem SharePoint, mogą doświadczyć tego problemu.

1. Aby rozwiązać ten problem, przywróć pierwotną nazwę upn zgodnie z krokami z artykułu, Przywróć użytkownika w [programie Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)
2. Jeśli nie możesz przywrócić pierwotnego użytkownika, usuń starego użytkownika z witryny OneDrive, korzystając z tej procedury, usuń użytkownika [z listy informacji o użytkowniku.]() 
3. Gdy to zrobisz, możesz sprawdzić, czy użytkownik ma prawa administratora do witryny OneDrive, korzystając z procedury Dodawanie administratorów dla witryny [OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Aby uzyskać więcej informacji na temat poziomów uprawnień, zobacz artykuł Opis poziomów uprawnień w [programie SharePoint.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
