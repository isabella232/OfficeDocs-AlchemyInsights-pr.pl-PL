---
title: Aktualizowanie rekordów DNS w celu zachowania witryny sieci Web u obecnego dostawcy hostingu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665770"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Aktualizowanie rekordów DNS w celu zachowania witryny sieci Web u obecnego dostawcy hostingu

1. W centrum administracyjnym usługi Microsoft 365 przejdź do strony **Domeny instalacji,**  >  [Domains](https://portal.office.com/adminportal/home#/Domains) a na liście domen wybierz domenę używanej w witrynie sieci Web.

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
