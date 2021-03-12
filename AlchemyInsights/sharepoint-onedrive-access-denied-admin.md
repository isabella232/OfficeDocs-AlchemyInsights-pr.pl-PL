---
title: Rozwiązywanie problemów z wiadomościami o odmowie dostępu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707964"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Rozwiązywanie problemów z komunikatami o odmowie dostępu w centrum administracyjnym programu SharePoint/usługi OneDrive

Jeśli podczas próby przeglądania centrum administracyjnego programu SharePoint/usługi OneDrive jest wyświetlany komunikat o odmowie dostępu, upewnij się, że przypisano licencję [do użytkownika.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Jeśli użytkownik ma licencję, należy również upewnić się, że ma przypisaną rolę [administratora,](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) która może uzyskać dostęp do centrów aadministracyjnym.

Ten problem może również wystąpić, gdy użytkownik zostanie usunięty i utworzony ponownie z tą samą główną nazwą użytkownika (UPN). Nowe konto jest tworzone przy użyciu innej wartości identyfikatora PUID (Passport Unique ID). Gdy użytkownik próbuje uzyskać dostęp do zbioru witryn lub usługi OneDrive, ma on nieprawidłowy identyfikator PUID. Drugi scenariusz obejmuje synchronizację katalogów z jednostką organizacyjną usługi Active Directory. Ten problem może wystąpić, jeśli użytkownicy już zalogowali się do programu SharePoint, a następnie zostali przeniesioni do innej społeczności użytkownika i ponownie zsynchroniznini z programem SharePoint.

Aby rozwiązać ten problem, przywróć pierwotną nazwę upn zgodnie z instrukcjami w artykule Przywróć użytkownika na platformie [Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

Uwaga: Jeśli centrum administracyjne usługi OneDrive lub programu SharePoint nie jest dostępne dla wielu użytkowników, którzy wcześniej mieli dostęp, może wystąpić tymczasowy problem z usługą.  [Sprawdź pulpit nawigacyjny kondycji usługi.](https://portal.office.com/adminportal/home#/servicehealth)


