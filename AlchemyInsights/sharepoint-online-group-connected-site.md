---
title: Dodawanie grupy do witryny programu SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771218"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemy podczas tworzenia witryny połączonej z grupą w programie SharePoint

1. Napotkano niektóre typowe problemy podczas tworzenia lub ponownego tworzenia witryny połączonej z grupą.
Jeśli usunięto grupę i jej połączoną witrynę i chcesz utworzyć inną witrynę o tym samym adresie URL, musisz trwale usunąć poprzednią witrynę.

   - Pobierz [powłokę zarządzania usługi spo](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Aby uzyskać więcej informacji na temat rozpoczynania pracy z programem PowerShell, zobacz [wprowadzenie do powłoki zarządzania usługi SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Usuń witrynę z witryn usuniętych za pomocą polecenia cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) programu PowerShell. Do trwałego usunięcia witryn grupy jest wymagany program PowerShell.

1. Jeśli tworzysz witrynę połączoną z grupą i otrzymujesz Ostrzeżenie: **inna grupa o tym samym aliasie już istnieje**, Sprawdź istniejące grupy w [centrum administracyjnym usługi Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Aby rozwiązać ten problem, Usuń istniejącą grupę, jeśli nie jest już potrzebna, lub Utwórz witrynę z przypisanym innym aliasem.

1. Istnieją różne sposoby tworzenia i używania nowoczesnych grup w programie SharePoint.

   - Istniejące witryny można połączyć z grupą programu Microsoft 365. Aby uzyskać więcej informacji, zobacz [łączenie grupy programu Microsoft 365 za pomocą interfejsu użytkownika programu SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Aby utworzyć witrynę połączoną z grupą programu Microsoft 365, należy utworzyć [witrynę zespołu](https://admin.microsoft.com/sharepoint).
