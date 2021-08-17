---
title: Synchronizacja profilu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320719"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kiedy mój profil zostanie zsynchronizowany z aplikacją profilu SharePoint profilu użytkownika?

SharePoint W trybie online do importowania użytkowników i grup do aplikacji profilu użytkownika jest używane zadanie czasomierza importu usługi Active Directory (importowanie ad). 
  
1. Import usługi AD synchronizuje zmiany z SharePoint katalogów online do aplikacji profilu użytkownika. Te zmiany są przetwarzane partiami.
    
2. Zadanie czasomierza jest uruchamiane do momentu zsynchronizowania zmian.
    
**Uwaga:** Czas trwania zadania zależy od liczby zmian w procesie. Duża liczba zmian trwa dłużej. Umowa o poziomie usług (SLA) stanowi, że zmiana dla użytkownika w katalogu SharePoint Online zostanie odzwierciedlona w aplikacji profilu użytkownika w ciągu 24 godzin. 
  
[Więcej informacji na temat synchronizacji profilu użytkownika w aplikacji SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

