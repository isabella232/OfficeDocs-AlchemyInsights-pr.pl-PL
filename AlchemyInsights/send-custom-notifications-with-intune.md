---
title: Wysyłanie niestandardowych powiadomień za pomocą usługi Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992322"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Jak wysyłać niestandardowe powiadomienia do użytkowników zarządzanych urządzeń z systemem iOS i Android

Niestandardowe powiadomienia dla usługi Intune są przetwarzane przez aplikację Portal firmy na urządzeniu użytkownika. Następnie aplikacja utworzy powiadomienie push na tym urządzeniu.

Poniżej przedstawiono wymagania wstępne dotyczące urządzeń do obsługi otrzymania niestandardowych powiadomień, a dla aplikacji, aby następnie utworzyć powiadomienie push:

- Urządzenie musi mieć zainstalowaną aplikację Portal firmy.  

- Urządzenie musi zezwalać aplikacji Portal firmy na wysyłanie powiadomień wypychanych. Po zainstalowaniu lub zaktualizowaniu aplikacji będzie monitować użytkownika o zezwolenie na powiadomienia.

- Urządzenia z Androidem muszą mieć zainstalowane usługi Google Play.

- Urządzenie musi być zarejestrowane w usłudze Intune.

Aby uzyskać więcej informacji, w tym jak wysłać wiadomość, zobacz [dokumentację funkcji](https://docs.microsoft.com/intune/custom-notifications).
