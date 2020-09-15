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
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801779"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kiedy zmiany w profilu są synchronizowane z aplikacją profilu użytkownika programu SharePoint?

Usługa SharePoint Online używa zadania czasomierza importu usługi Active Directory (importu AD) do importowania użytkowników i grup do aplikacji profilu użytkownika. 
  
1. Import usługi AD powoduje zsynchronizowanie zmian z magazynu katalogów usługi SharePoint Online w aplikacji profilu użytkownika. Te zmiany są przetwarzane w partiach.
    
2. Zadanie czasomierza zostanie uruchomione do momentu zsynchronizowania zmian.
    
> [!NOTE]
> Czas potrzebny na uruchomienie zadania zależy od liczby zmian, które należy przetworzyć. Duża liczba zmian trwa dłużej. Umowa dotycząca poziomu usług (SLA) określa, że zmiana dotycząca użytkownika w katalogu usługi SharePoint Online będzie odzwierciedlana w aplikacji profilu użytkownika w ciągu 24 godzin. 
  
[Więcej informacji na temat synchronizacji profilu użytkownika w usłudze SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

