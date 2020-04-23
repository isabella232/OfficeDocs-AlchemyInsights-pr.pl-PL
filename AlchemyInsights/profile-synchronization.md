---
title: Synchronizacja profilu
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768123"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kiedy zmiany profilu są synchronizowane z aplikacją profilu użytkownika programu SharePoint?

Usługa SharePoint Online używa zadania czasomierza importu usługi Active Directory (Import usługi AD) do importowania użytkowników i grup do aplikacji profilu użytkownika. 
  
1. Import usługi AD synchronizuje zmiany ze sklepu sharepoint online do aplikacji profilu użytkownika. Zmiany te są przetwarzane w partiach.
    
2. Zadanie czasomierza jest uruchamiane do momentu zsynchronizowania zmian.
    
> [!NOTE]
> Czas potrzebny do uruchomienia zadania zależy od liczby zmian do przetworzenia. Duża liczba zmian trwa dłużej. Umowa dotyczącej poziomu usług (SLA) stanowi, że zmiana użytkownika w katalogu SharePoint Online zostanie odzwierciedlona w aplikacji profilu użytkownika w ciągu 24 godzin. 
  
[Więcej informacji o synchronizacji profilu użytkownika w usłudze SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

