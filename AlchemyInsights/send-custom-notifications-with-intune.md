---
title: Wysyłanie niestandardowych powiadomień za pomocą usługi Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086174"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Jak wysyłać niestandardowe powiadomienia do użytkowników zarządzanych urządzeń z systemami iOS i Android

Niestandardowe powiadomienia dla usługi Intune są przetwarzane Portal firmy aplikacji na urządzeniu użytkownika. Aplikacja następnie utworzy powiadomienie wypychane na tym urządzeniu.

Poniżej przedstawiono wymagania wstępne dotyczące urządzeń do obsługi pokwitowania niestandardowych powiadomień oraz utworzenia przez aplikację powiadomień wypychanych:

- Urządzenie musi mieć zainstalowaną Portal firmy urządzenia.  

- Urządzenie musi zezwolić aplikacji Portal firmy wysyłania powiadomień wypychanych. Gdy aplikacja zostanie zainstalowana lub zaktualizowana, zostanie wyświetlony monit o zezwolenie na powiadomienia.

- Na urządzeniach z systemem Android muszą być zainstalowane usługi Google Play.

- Urządzenie musi zostać zarejestrowane w usłudze Intune.

Aby uzyskać więcej informacji, w tym na temat wysyłania wiadomości, zapoznaj się z [dokumentacją funkcji.](https://docs.microsoft.com/intune/custom-notifications)
