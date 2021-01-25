---
title: Uprawnienia interfejsu API i zgoda
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974989"
---
# <a name="api-permissions-and-consent"></a>Uprawnienia interfejsu API i zgoda

Aplikacje, które są integrowane z platformą tożsamości firmy Microsoft, korzystają z modelu autoryzacji, który umożliwia użytkownikom i administratorom kontrolę nad sposobem uzyskiwania dostępu do danych. Implementacja modelu autoryzacji została zaktualizowana w punkcie końcowym Microsoft Identity platform. Zmiana sposobu, w jaki aplikacja musi współpracować z platformą Microsoft Identity. [Uprawnienia i zgoda w punkcie końcowym Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) obejmują podstawowe pojęcia tego modelu autoryzacji, w tym zakresy, uprawnienia i sposób wyrażania zgody.

[Struktura zgody na usługę Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) ułatwia tworzenie wielodostępnych i natywnych aplikacji klienckich. Te aplikacje umożliwiają logowanie się na kontach użytkowników z dzierżawy usługi Azure AD innej niż ta, w której zarejestrowano aplikację. Mogą także mieć dostęp do interfejsów API sieci Web, takich jak Microsoft Graph API (Aby uzyskać dostęp do usługi Azure AD, usługi Intune i usług w systemie Microsoft 365) oraz innych interfejsów API usług firmy Microsoft, oprócz własnych interfejsów API sieci Web.

