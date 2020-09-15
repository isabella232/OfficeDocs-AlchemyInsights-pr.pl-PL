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
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691585"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Rozwiązywanie problemów z udostępnianiem zawartości programu SharePoint użytkownikom zewnętrznym

Upewnij się, że funkcja udostępniania zewnętrznego jest włączona w Twojej organizacji:
  
1. Przejdź do [ &amp; strony Dodatki usług w centrum administracyjnym usługi Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), a następnie kliknij pozycję **witryny**.
    
2. Upewnij się, że ustawienie jest włączone. Jeśli jest zaznaczona pozycja "tylko istniejący użytkownik zewnętrzny", upewnij się, że użytkownik zewnętrzny jest wymieniony w centrum administracyjnym usługi Microsoft 365.
    
Upewnij się, że włączono udostępnianie zewnętrzne witryny. W przypadku klasycznego zbioru witryn:
  
1. W nowym centrum administracyjnym programu SharePoint w okienku po lewej stronie kliknij pozycję **witryny**.
    
2. Wybierz witrynę lub witryny, a następnie na wstążce kliknij pozycję **udostępnianie**.
    
W przypadku witryny zespołu należącej do grupy programu Microsoft 365 lub witryny do komunikacji:
  
- Te nowe typy witryn mają to samo ustawienie udostępniania, co ustawienie w całej organizacji, chyba że ustawienie całej organizacji umożliwia udostępnianie plików za pomocą linków, które nie wymagają logowania. W tym przypadku witryny umożliwiają udostępnianie nowym i istniejącym użytkownikom zewnętrznym, którzy będą logować się. Aby zmienić ustawienie dla określonych witryn, Użyj nowego centrum administracyjnego programu SharePoint lub programu PowerShell. [Dowiedz się więcej](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Ustawienia udostępniania zewnętrznego dla dowolnej witryny mogą być bardziej restrykcyjne niż ustawienia dla całej organizacji, ale nie są one ograniczane od ustawienia dla całej organizacji. 
  

