---
title: Trwałe usuwanie witryny w programie SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955243"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Trwałe usuwanie witryny w programie SharePoint

Aby ponownie użyć adresu URL z usuniętej witryny (w celu odtworzenia witryny) lub trwale usunąć witrynę, ponieważ nie jest już używana, możesz użyć pozycji **Trwale usuń** z nowego centrum administracyjnego programu SharePoint. 

1. Przejdź [na stronę usuniętych witryn nowego centrum administracyjnego programu SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) i zaloguj się przy użyciu konta z uprawnieniami administratora dla organizacji. 

2. W kolumnie po lewej stronie wybierz witrynę. 

3. Kliknij pozycję **Trwale usuń**. 

**Uwaga**: Nie można trwale usunąć witryn połączonych z grupami w nowym centrum administracyjnym programu SharePoint. Zamiast tego należy użyć polecenia [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite).  

Aby uzyskać więcej informacji, zobacz [Trwałe usuwanie witryny](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site). 
