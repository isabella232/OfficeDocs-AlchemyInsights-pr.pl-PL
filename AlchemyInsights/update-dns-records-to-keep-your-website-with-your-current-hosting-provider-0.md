---
title: Aktualizowanie rekordów DNS w celu zachowania witryny sieci Web u obecnego dostawcy hostingu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f2cdb319e56b82c09b7a9856c81a45e69dee6759
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423733"
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
    

