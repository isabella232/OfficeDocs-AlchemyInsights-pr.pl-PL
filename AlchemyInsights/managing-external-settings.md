---
title: Zarządzanie ustawieniami zewnętrznymi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294313"
---
# <a name="managing-external-settings"></a>Zarządzanie ustawieniami zewnętrznymi

**Ogłoszenie**

- [Od 4 stycznia 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support)r. firma Google wyloguje obsługę logowania WebView. Sprawdź, czy na Twoje aplikacje mają wpływ wytyczne firmy Google dotyczące testowania zgodności
- Korzystanie z funkcji System WebView lub przeglądarki systemowej podczas logowania się do użytkowników za pomocą kont Google dla klientów indywidualnych

**Zarządzanie ustawieniami zaproszenia**

Upewnij się, że ustawienia współpracy zewnętrznej zostały skonfigurowane [w](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) celu umożliwienia odpowiednim osobom wysyłania zaproszeń.

**Zarządzanie uprawnieniami dostępu użytkownika gościa**

1. Administratorzy globalni mogą zarządzać uprawnieniami dostępu gości w katalogu za pośrednictwem portalu Azure Portal, konfigurując uprawnienia dostępu gościa na stronie Ustawienia współpracy zewnętrznej. [Dowiedz się więcej o tym ustawieniu.](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support)
2. Jeśli chcesz, aby goście mieli dostęp do aplikacji, takich jak Teams lub SharePoint, potwierdź, że te aplikacje zostały skonfigurowane tak, aby zezwalały na dostęp gości. Dowiedz się więcej o [ustawieniach aplikacji Teams i](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) [programie SharePoint.](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)

**Konfigurowanie zaproszeń:**

- [Włączanie współpracy zewnętrznej B2B i zarządzanie tym, kto może zapraszać gości](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Zezwalanie na zaproszenia do użytkowników z określonych organizacji lub blokowanie ich](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

**Konfigurowanie dozwolonych dostawców tożsamości:**

- [Federacja Google](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Federacja bezpośrednia](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Uwierzytelnianie za pomocą adresu e-mail z kodem dostępu w wiadomości e-mail](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
