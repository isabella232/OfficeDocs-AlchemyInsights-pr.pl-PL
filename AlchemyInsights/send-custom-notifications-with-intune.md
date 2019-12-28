---
title: Wysyłanie niestandardowych powiadomień za pomocą usługi Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886867"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Jak wysyłać niestandardowe powiadomienia do użytkowników zarządzanych urządzeń z systemem iOS i Android

Niestandardowe powiadomienia dla usługi Intune są przetwarzane przez aplikację Portal firmy na urządzeniu użytkownika. Następnie aplikacja utworzy powiadomienie push na tym urządzeniu.

Poniżej przedstawiono wymagania wstępne dotyczące urządzeń do obsługi otrzymania niestandardowych powiadomień, a dla aplikacji, aby następnie utworzyć powiadomienie push:

- Urządzenie musi mieć zainstalowaną aplikację Portal firmy.  

- Urządzenie musi zezwalać aplikacji Portal firmy na wysyłanie powiadomień wypychanych. Po zainstalowaniu lub zaktualizowaniu aplikacji będzie monitować użytkownika o zezwolenie na powiadomienia.

- Urządzenia z Androidem muszą mieć zainstalowane usługi Google Play.

- Urządzenie musi być zarejestrowane w usłudze Intune.

Aby uzyskać więcej informacji, w tym jak wysłać wiadomość, zobacz [dokumentację funkcji](https://docs.microsoft.com/intune/custom-notifications).
