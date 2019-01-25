---
title: Aktualizowanie rekordów DNS w celu zachowania witryny sieci Web u obecnego dostawcy hostingu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29482900"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Aktualizowanie rekordów DNS w celu zachowania witryny sieci Web u obecnego dostawcy hostingu

1. Na stronie [Domeny](https://portal.office.com/adminportal/home#/Domains) wybierz z listy domen tę domenę, której używasz dla witryny internetowej, a następnie w okienku zarządzania wybierz pozycję **Ustawienia DNS**. 
    
2. Wybierz pozycję **+ Nowy rekord niestandardowy** i wprowadź następujące wartości: 
    
  - W polu **Typ DNS** wprowadź: **A (Adres)**
    
  - W polu **Nazwa hosta lub alias** wpisz następujący tekst: **@**
    
  - W polu **Adres IP** wpisz statyczny adres IP, pod którym witryna sieci Web jest obecnie hostowana (na przykład 172.16.140.1). 
    
    Adres IP musi być  *statyczny*  , a nie  *dynamiczny*  . Skontaktuj się z dostawcą hostingu i upewnij się, że możesz uzyskać statyczny adres IP swojej publicznej witryny sieci Web. 
    
3. Wybierz pozycję **Zapisz**. 
    
Możesz też utworzyć rekord CNAME, aby ułatwić klientom odnalezienie Twojej witryny sieci Web.
  
1. Wybierz pozycję **+ Nowy rekord niestandardowy** i wprowadź następujące wartości: 
    
  - W polu **Typ DNS** wprowadź: **CNAME (Alias)**
    
  - W polu **Nazwa hosta lub alias** wpisz następujący tekst: **www**.
    
  - W polu **Wskazywany adres** wpisz w pełni kwalifikowaną nazwę domeny (FQDN) swojej witryny sieci Web (na przykład contoso.com). 
    
2. Wybierz pozycję **Zapisz**. 
    

