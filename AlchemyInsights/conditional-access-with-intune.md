---
title: Dostęp warunkowy z usłudze Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706031"
---
# <a name="conditional-access-with-intune"></a>Dostęp warunkowy z usłudze Intune

Korzystanie z **dostępu warunkowego** z usłudze Intune wymaga 3 kroków: 
  
- Utwórz **zasady dostępu warunkowego,** który określa, jakie zasoby są chronione i jakie warunki muszą być spełnione, aby uzyskać dostęp do tych zasobów. Na przykład urządzenie musi być zgodne przed dostępem do firmowej poczty e-mail. 
    
- Utwórz **zasady zgodności,** aby zdefiniować ustawienia, które muszą być spełnione, zanim urządzenie zostanie uznane za zgodne. Na przykład urządzenie musi mieć pin co najmniej 6 cyfr, zanim zostanie uznane za zgodne. 
    
- Zapewnienie zarówno **zasad zgodności,** jak i **zasad dostępu warunkowego** są kierowane do pożądanych grup użytkowników. Może to wymagać utworzenia określonych grup użytkowników w usłudze Azure Active Directory. 
    
Czytaj więcej:
  
- [Najważniejsze wskazówki dotyczące dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Wprowadzenie do dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

