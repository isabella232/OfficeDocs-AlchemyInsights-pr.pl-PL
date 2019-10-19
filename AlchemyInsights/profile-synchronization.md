---
title: Synchronizacja profilu
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554343"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kiedy mój profil zmienia synchronizację z aplikacją profilu użytkownika programu SharePoint?

Program SharePoint Online używa zadania czasomierza importu usługi Active Directory (AD import) do importowania użytkowników i grup do aplikacji profilu użytkownika. 
  
1. Import AD synchronizuje zmiany z magazynu usługi SharePoint Online Directory do aplikacji profilu użytkownika. Te zmiany są przetwarzane w partiach.
    
2. Zadanie czasomierza jest uruchamiane, dopóki zmiany są synchronizowane.
    
> [!NOTE]
> Czas potrzebny do uruchomienia zadania zależy od liczby zmian do przetworzenia. Duża liczba zmian trwa dłużej. Umowa dotycząca poziomu usług (SLA) stwierdza, że zmiana użytkownika w katalogu online programu SharePoint zostaną uwzględnione w aplikacji profilu użytkownika w ciągu 24 godzin. 
  
[Więcej informacji o synchronizacji profilu użytkownika w programie SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

