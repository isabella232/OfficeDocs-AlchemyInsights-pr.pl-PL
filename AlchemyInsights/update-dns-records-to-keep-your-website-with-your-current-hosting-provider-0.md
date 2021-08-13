---
title: Aktualizowanie rekordów DNS w celu zachowania witryny sieci Web u obecnego dostawcy hostingu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f868ce25d68f61da30d2db4de88aa83675c97857b3c1371cf2039e0b03895a64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007692"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Aktualizowanie rekordów DNS w celu zachowania witryny sieci Web u obecnego dostawcy hostingu

1. W centrum administracyjne platformy Microsoft 365 przejdź do strony Konfiguracja domen i z listy domen wybierz domenę, która jest twoją  >  [](https://admin.microsoft.com/Adminportal#/Domains) witryną internetową.

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
