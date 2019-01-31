---
title: Warunkowy dostęp z Windows Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 3b50bc96a879017b62e42e1849f72e68408a0d9d
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662337"
---
# <a name="conditional-access-with-intune"></a>Warunkowy dostęp z Windows Intune

Przy użyciu **Dostępu warunkowego** w usłudze Intune wymaga 3 kroki: 
  
- Utwórz **Zasadę warunkową dostępu** , który definiuje, jakie zasoby są chronione, a co warunki muszą być spełnione, aby uzyskać dostęp do tych zasobów. Na przykład urządzenie musi być zgodny, przed uzyskaniem dostępu do firmowych wiadomości e-mail. 
    
- Tworzy **Zasady zgodności** do definiowania ustawień, które muszą być spełnione, zanim urządzenie zostanie uznana za zgodną. Na przykład urządzenie musi mieć co najmniej 6 cyfr numeru pin zostanie uznany za zgodny z. 
    
- Zapewnienie zarówno **Zasady dostępu warunkowego** , jak i **Zasady zgodności** są kierowane do żądanej grupy użytkowników. To może być konieczne utworzenie określonych grup użytkowników w usłudze Active Directory Azure. 
    
Dowiedz się więcej:
  
- [Warunkowy dostęp do najlepszych praktyk](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Wprowadzenie do dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

