---
title: Uprawnienia i zgody interfejsu API
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
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932107"
---
# <a name="api-permissions-and-consent"></a>Uprawnienia i zgody interfejsu API

Aplikacje integrują się z Platforma tożsamości Microsoft modelem autoryzacji, który zapewnia użytkownikom i administratorom kontrolę nad dostępem do danych. Implementacja modelu autoryzacji została zaktualizowana w punkcie Platforma tożsamości Microsoft końcowym. Zmienia to sposób interakcji aplikacji z Platforma tożsamości Microsoft. [Uprawnienia i zgody w punkcie Platforma tożsamości Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) to podstawowe pojęcia związane z tym modelem autoryzacji, w tym zakresy, uprawnienia i zgody.

Platforma [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) ułatwia opracowywanie wielodostępnych aplikacji klienckich w sieci Web i natywnych. Te aplikacje umożliwiają logowanie się przez konta użytkowników z dzierżawy usługi Azure AD, które różnią się od tej, w której aplikacja jest zarejestrowana. Oprócz własnych interfejsów API sieci Web mogą również być konieczne uzyskiwanie dostępu do interfejsów API sieci Web, takich jak interfejs API usługi Microsoft Graph (w celu uzyskania dostępu do usług Azure AD, Intune i usług w systemie Microsoft 365) oraz innych interfejsów API usługi usługi firmy Microsoft.

