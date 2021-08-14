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
ms.openlocfilehash: b223bad66fb7cc6d1d7c0a2b3ccc7a081c061b4974060dbcafec84dfb24eb782
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923654"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kiedy mój profil zmieni się na zsynchronizowany z aplikacją SharePoint profilu użytkownika?

SharePoint Usługa Online używa zadania czasomierza importu usługi Active Directory (importowania ad) do importowania użytkowników i grup do aplikacji profilu użytkownika. 
  
1. Import usługi AD synchronizuje zmiany z SharePoint katalogów online do aplikacji profilu użytkownika. Te zmiany są przetwarzane partiami.
    
2. Zadanie czasomierza jest uruchamiane do momentu zsynchronizowania zmian.
    
> [!NOTE]
> Czas przetwarzania zadania zależy od liczby zmian w procesie. Duża liczba zmian trwa dłużej. Umowa o poziomie usług (SLA) stanowi, że zmiana użytkownika w katalogu usługi SharePoint Online zostanie odzwierciedlona w aplikacji profilu użytkownika w ciągu 24 godzin. 
  
[Więcej informacji na temat synchronizacji profilu użytkownika w aplikacji SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

