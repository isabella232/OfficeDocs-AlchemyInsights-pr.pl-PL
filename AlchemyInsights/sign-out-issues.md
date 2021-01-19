---
title: Problemy z wylogowaniem się
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7793"
- "9004355"
ms.openlocfilehash: 794e5c43340ba4b5c653eda4c11b4480cd3fa710
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901306"
---
# <a name="sign-out-issues"></a>Problemy z wylogowaniem się

Aby wyeliminować problemy związane z wylogowaniem się, wykonaj następujące czynności:

1. Jeśli użytkownik jest zalogowany lub odbierał aplikacje, należy postępować zgodnie z instrukcjami zawartymi w artykułach [Konfigurowanie zarządzania sesjami uwierzytelniania za pomocą dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) lub [konfigurowania okresów ważności tokenów na platformie Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Większość innych błędów logowania lub problemów można rozwiązać przez Rozwiązywanie problemów z integracją usługi Azure Active Directory (Azure AD) z określoną aplikacją. Wskazówki dotyczące konkretnej integracji można znaleźć, przechodząc do tego [zestawu samouczków dotyczących integrowania aplikacji z usługą Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list), w tym:
    - Samouczki aplikacji SaaS
    - Samouczki rejestracji jednokrotnej
    - Samouczki użytkowników