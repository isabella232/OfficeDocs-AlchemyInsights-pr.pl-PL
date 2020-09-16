---
title: Wysyłanie powiadomień niestandardowych za pomocą usługi Intune
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
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720656"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Jak wysyłać powiadomienia niestandardowe do użytkowników zarządzanych urządzeń z systemem iOS i Android

Niestandardowe powiadomienia usługi Intune są przetwarzane przez aplikację Portal firmy na urządzeniu użytkownika. Aplikacja następnie utworzy powiadomienie o wypychaniu na tym urządzeniu.

Poniżej przedstawiono wymagania wstępne dotyczące urządzeń, które umożliwiają otrzymywanie powiadomień niestandardowych, a następnie aplikację do tworzenia powiadomień wypychanych:

- Na urządzeniu musi być zainstalowana aplikacja Portal firmy.  

- Urządzenie musi umożliwiać aplikacji Portal firmy wysyłanie powiadomień wypychanych. Po zainstalowaniu lub zaktualizowaniu aplikacji zostanie wyświetlony monit o zezwolenie użytkownikowi na powiadomienia.

- Na urządzeniach z systemem Android muszą być zainstalowane usługi Google Play.

- Urządzenie musi być zarejestrowane za pomocą usługi Intune.

Aby uzyskać więcej informacji, w tym jak wysłać wiadomość, zapoznaj się z [dokumentacją funkcji](https://docs.microsoft.com/intune/custom-notifications).
