---
title: Rozwiązywanie problemów z wiadomościami odmowy dostępu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505389"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Rozwiązywanie problemów z wiadomościami odmowy dostępu w Centrum administracyjnym programu Sharepoint/OneDrive

Jeśli podczas próby przeglądania programu Sharepoint/OneDrive Admin Center jest wyświetlany komunikat o odmowie dostępu, należy [przypisać licencję do użytkownika](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Jeśli użytkownik ma licencję, należy również upewnić się, że [przypisano mu rolę administratora,](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) która może uzyskać dostęp do centrów administracyjnych.

Ten problem może również wystąpić, gdy użytkownik jest usuwany i ponownie tworzony przy tej samej głównej nazwie użytkownika (UPN). Nowe konto jest tworzone przy użyciu innej wartości PUID (Passport Unique ID). Gdy użytkownik próbuje uzyskać dostęp do zbioru witryn lub ich OneDrive, użytkownik ma niepoprawny PUID. Drugi scenariusz obejmuje synchronizację katalogów z jednostką organizacyjną usługi Active Directory.A second scenario involves directory synchronizacji with an Active Directory organizational unit (OU). Jeśli użytkownicy już zalogowali się do programu SharePoint, a następnie zostaną przeniesieni do innej usługi organizacyjnej i ponownie zsynchronizowani za pomocą programu SharePoint, może wystąpić ten problem.

Aby rozwiązać ten problem, należy przywrócić oryginalną nazwy UPN z krokami w artykule, [Przywracanie użytkownika w usłudze Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Uwaga: Jeśli usługa OneDrive lub centrum administracyjne programu SharePoint nie jest dostępna dla wielu użytkowników, którzy wcześniej mieli do nich dostęp, może to być tymczasowy problem z usługą.  [Sprawdź pulpit nawigacyjny kondycji usługi](https://portal.office.com/adminportal/home#/servicehealth).


