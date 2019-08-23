---
title: Synchronizacji profilu
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554343"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kiedy moje zmiany profilu synchronizację aplikacji profilu użytkownika programu SharePoint?

SharePoint Online używa zadanie czasomierza importu usługi Active Directory (AD Import) do importowania użytkowników i grup do aplikacji profilu użytkownika. 
  
1. Importuj AD synchronizuje zmiany z magazynu katalogu Online programu SharePoint do aplikacji profilu użytkownika. Te zmiany są przetwarzane w plikach wsadowych.
    
2. Zadanie czasomierza jest uruchamiany, dopóki zmiany są synchronizowane.
    
> [!NOTE]
> Czas uruchomienia zadania zależy od liczby zmian do procesu. Dużej liczby zmian trwa dłużej. Umowy poziomu usług (SLA) stwierdza, że zmiany do użytkownika w katalogu Online programu SharePoint będą uwzględniane w aplikacji profilu użytkownika w ciągu 24 godzin. 
  
[Więcej informacji o synchronizacji profilu użytkownika w dokumentacji Online programu SharePoint](https://go.microsoft.com/fwlink/?linkid=875671)
  

