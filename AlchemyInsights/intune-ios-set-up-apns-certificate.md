---
title: Konfigurowanie certyfikatu APNS dla usługi Intune na urządzeniu z systemem iOS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "3543"
ms.openlocfilehash: 027e1e0fa3b625fa0f619bc6d74844f6ec5be769
ms.sourcegitcommit: 75346a972c2174248de3bb55a19d714cee43c1cc
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/09/2020
ms.locfileid: "43211442"
---
# <a name="intune-ios-set-up-apns-certificate"></a>Konfigurowanie certyfikatu APNS dla usługi Intune na urządzeniu z systemem iOS

Certyfikat Apple dla aktywnej komunikacji MDM (nazywany również Usługą powiadomień w trybie push firmy Apple — APNS) nie został skonfigurowany dla Twojej subskrypcji.

Bez skonfigurowania certyfikatu Apple dla aktywnej komunikacji MDM nie można rejestrować w usłudze urządzeń z systemem iOS i MacOS ani zarządzać tymi urządzeniami. Po dodaniu certyfikatu do usługi Intune użytkownicy będą mogli zainstalować aplikację Portal firmy, aby zarejestrować swoje urządzenia z systemem iOS.

W artykule dostępnym po kliknięciu poniższego linku znajdziesz przewodnik opisujący krok po kroku dodawanie certyfikat APNS do dzierżawy usługi Intune:

- [Pobierz certyfikat Apple dla aktywnej komunikacji MDM](https://docs.microsoft.com/mem/intune/enrollment/apple-mdm-push-certificate-get)

Jeśli występują problemy z certyfikatem Apple dla aktywnej komunikacji MDM (APNs), zapoznaj się z tym wpisem na blogu: [Usługa Intune i certyfikat APNs — często zadawane pytania i typowe problemy](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)
