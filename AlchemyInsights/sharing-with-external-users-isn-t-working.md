---
title: Udostępnianie użytkownikom zewnętrznym nie działa
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502241"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Rozwiązywanie problemów z udostępnianiem zawartości programu SharePoint użytkownikom zewnętrznym

Upewnij się, że w organizacji jest włączone udostępnianie zewnętrzne:
  
1. Przejdź do [strony dodatków &amp; usług w centrum administracyjnym Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)i kliknij przycisk **witryny**.
    
2. Upewnij się, że ustawienie jest włączone. Jeśli wybrano "tylko istniejący użytkownicy zewnętrzni", upewnij się, że użytkownik zewnętrzny jest wymieniony w centrum administracyjnym Microsoft 365.
    
Upewnij się, że udostępnianie zewnętrzne jest włączone dla witryny. Dla klasycznego zbioru witryn:
  
1. W nowym centrum administracyjnym programu SharePoint w lewym okienku kliknij pozycję **witryny**.
    
2. Wybierz witrynę lub witryny, a na wstążce kliknij przycisk **udostępnianie**.
    
W przypadku witryny zespołu należącej do grupy 365 pakietu Office lub witryny komunikacyjnej:
  
- Te nowe typy witryn mają takie samo ustawienie udostępniania jak ustawienia dla całej organizacji, chyba że ustawienie dla całej organizacji umożliwia udostępnianie plików za pomocą łączy, które nie wymagają logowania. W takim przypadku witryny umożliwiają udostępnianie nowym i istniejącym użytkownikom zewnętrznym, którzy się zalogują. Aby zmienić ustawienie dla określonych witryn, należy użyć nowego centrum administracyjnego programu SharePoint lub programu PowerShell. [Dowiedz się więcej](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Ustawienie udostępniania zewnętrznego dla dowolnej witryny może być bardziej restrykcyjne niż ustawienie dla całej organizacji, ale nie jest to więcej niż ustawienie dla całej organizacji. 
  

