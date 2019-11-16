---
title: Dostęp warunkowy z usługą Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/15/2019
ms.locfileid: "36505004"
---
# <a name="conditional-access-with-intune"></a>Dostęp warunkowy z usługą Intune

Korzystanie z **dostępu warunkowego** w usłudze Intune wymaga 3 kroków: 
  
- Utwórz **zasadę dostępu warunkowego** , która określa, jakie zasoby są chronione i jakie warunki muszą być spełnione, aby uzyskać dostęp do tych zasobów. Na przykład urządzenie musi być zgodne przed uzyskaniem dostępu do firmowej poczty e-mail. 
    
- Utwórz **zasadę zgodności** , aby zdefiniować ustawienia, które muszą zostać spełnione, zanim urządzenie zostanie uznane za zgodne. Na przykład urządzenie musi mieć PIN co najmniej 6 cyfr, zanim zostanie uznane za zgodne. 
    
- Zapewnienie, że zarówno **zasady zgodności** , jak i **zasady dostępu warunkowego** są kierowane do żądanych grup użytkowników. Może to wymagać utworzenia określonych grup użytkowników w usłudze Azure Active Directory. 
    
Czytaj więcej:
  
- [Najważniejsze wskazówki dotyczące dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Rozpoczynanie korzystania z dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

