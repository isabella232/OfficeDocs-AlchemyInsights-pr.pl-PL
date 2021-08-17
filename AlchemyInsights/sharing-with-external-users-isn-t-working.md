---
title: Udostępnianie użytkownikom zewnętrznym nie działa
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 02d79c1b1e112eb41e8c60ffa2ef28e429f76ada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58304379"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Rozwiązywanie problemów z udostępnianiem SharePoint zawartości użytkownikom zewnętrznym

Upewnij się, że w organizacji włączona jest udostępnianie zewnętrzne:
  
1. Przejdź do [strony Dodatki usług w &amp; centrum administracyjne platformy Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), a następnie kliknij pozycję **Witryny.**
    
2. Upewnij się, że to ustawienie jest włączone. Jeśli zaznaczono opcję "Tylko istniejący użytkownicy zewnętrzni", upewnij się, że na liście znajduje się centrum administracyjne platformy Microsoft 365.
    
Upewnij się, że udostępnianie zewnętrzne jest włączone dla witryny. W przypadku klasycznego zbioru witryn:
  
1. W nowym centrum SharePoint administracyjnego w okienku po lewej stronie kliknij pozycję **witryny**.
    
2. Wybierz witrynę lub witryny, a następnie na wstążce kliknij pozycję **Udostępnianie**.
    
W przypadku witryny zespołu, która należy Microsoft 365 grupy lub witryny do komunikacji:
  
- Te nowe typy witryn mają to samo ustawienie udostępniania co ustawienie dla całej organizacji, chyba że ustawienie dla całej organizacji umożliwia udostępnianie plików przy użyciu linków, które nie wymagają logowania. W takim przypadku witryny umożliwiają udostępnianie nowym i istniejącym użytkownikom zewnętrznym, którzy się logują. Aby zmienić ustawienie dla konkretnych witryn, użyj nowego centrum administracyjnego programu SharePoint lub programu PowerShell. [Dowiedz się więcej](https://go.microsoft.com/fwlink/?linkid=871863).
    
**Uwaga:** Ustawienie udostępniania zewnętrznego dla dowolnej witryny może być bardziej restrykcyjne niż ustawienie w całej organizacji, ale nie może być bardziej restrykcyjne niż ustawienie dla całej organizacji. 
  

