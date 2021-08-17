---
title: Rozwiązywanie problemów z komunikatami o odmowie dostępu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085238"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Rozwiązywanie problemów z komunikatami o odmowie dostępu w Centrum administracyjnym OneDrive SharePoint

Jeśli podczas próby przejść do Centrum administracyjnego programu SharePoint/programu OneDrive jest wyświetlany komunikat o odmowie dostępu, przypisz licencję [do użytkownika.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Jeśli użytkownik ma licencję, musisz również upewnić się, że ma on przypisaną rolę [administratora,](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) która może uzyskać dostęp do centrów aadministracyjnym.

Ten problem może również wystąpić w przypadku usunięcia i ponownego utworzenia użytkownika z tą samą główną nazwą użytkownika (UPN). Nowe konto jest tworzone przy użyciu innej wartości identyfikatora PUID (Passport Unique ID). Gdy użytkownik próbuje uzyskać dostęp do zbioru witryn lub swojego OneDrive, ma nieprawidłowy identyfikator PUID. Drugi scenariusz obejmuje synchronizację katalogów z jednostką organizacyjną usługi Active Directory. Jeśli użytkownicy już zalogowali się do usługi SharePoint, a następnie zostaną przeniesioni do innej usługi OU i ponownie zsynchroniznini z programem SharePoint, mogą doświadczyć tego problemu.

Aby rozwiązać ten problem, przywróć oryginalną nazwę użytkownika, wykonać czynności opisane w artykule Przywracanie użytkownika w [Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

Uwaga: Jeśli centrum administracyjne usługi OneDrive lub SharePoint jest niedostępne dla wielu użytkowników, którzy wcześniej mieli do niego dostęp, może wystąpić tymczasowy problem z usługą.  [Sprawdź pulpit nawigacyjny kondycji usługi.](https://portal.office.com/adminportal/home#/servicehealth)


