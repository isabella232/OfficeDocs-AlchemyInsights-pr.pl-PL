---
title: Rozwiązywanie problemów z odmową dostępu wiadomości
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767672"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Rozwiązywanie problemów z odmową dostępu wiadomości w programie SharePoint/centrum administracyjnym usługi OneDrive

Jeśli zostanie wyświetlony komunikat Odmowa dostępu podczas próby przełączenia się do centrum administracyjnego programu SharePoint/OneDrive, upewnij się, że [użytkownik przypisał licencję użytkownikowi](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Jeśli użytkownik ma licencję, należy również upewnić się, że jest [mu przypisana rola administratora](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , która może uzyskać dostęp do centrów administracyjnych.

Ten problem może również wystąpić, gdy użytkownik jest usuwany i tworzony ponownie przy użyciu tej samej głównej nazwy użytkownika (UPN). Nowe konto jest tworzone przy użyciu innej wartości identyfikatora PUID (unikatowy identyfikator paszportu). Gdy użytkownik usiłuje uzyskać dostęp do zbioru witryn lub jego usługi OneDrive, użytkownik ma nieprawidłowy identyfikator PUID. Drugi scenariusz obejmuje synchronizację katalogów za pomocą jednostki organizacyjnej (OU) Active Directory. Jeśli użytkownicy już zalogowali się do programu SharePoint, a następnie zostaną przesunięte do innej jednostki organizacyjnej i ponownie zsynchronizowane z programem SharePoint, mogą wystąpić ten problem.

Aby rozwiązać ten problem, należy przywrócić oryginalną główną nazwę użytkownika, wykonując czynności opisane w artykule, [przywracanie użytkownika w programie Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Uwaga: Jeśli centrum administracyjne usługi OneDrive lub programu SharePoint nie jest dostępne dla wielu użytkowników, którzy wcześniej mieli dostęp, może to być tymczasowy problem z usługą.  [Sprawdź pulpit nawigacyjny kondycji usługi](https://portal.office.com/adminportal/home#/servicehealth).


