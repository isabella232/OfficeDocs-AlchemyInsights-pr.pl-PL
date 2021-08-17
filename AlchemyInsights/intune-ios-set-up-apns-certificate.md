---
title: Konfigurowanie certyfikatu APNS dla usługi Intune na urządzeniu z systemem iOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "3543"
ms.openlocfilehash: 3dd0b42558f7543de84f45690596f2829195db9f4972c54ed239add7fe87b37c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054961"
---
# <a name="intune-ios-set-up-apns-certificate"></a>Konfigurowanie certyfikatu APNS dla usługi Intune na urządzeniu z systemem iOS

Certyfikat Apple dla aktywnej komunikacji MDM (nazywany również Usługą powiadomień w trybie push firmy Apple — APNS) nie został skonfigurowany dla Twojej subskrypcji.

Bez skonfigurowania certyfikatu Apple dla aktywnej komunikacji MDM nie można rejestrować w usłudze urządzeń z systemem iOS i MacOS ani zarządzać tymi urządzeniami. Po dodaniu certyfikatu do usługi Intune użytkownicy będą mogli zainstalować aplikację Portal firmy, aby zarejestrować swoje urządzenia z systemem iOS.

W artykule dostępnym po kliknięciu poniższego linku znajdziesz przewodnik opisujący krok po kroku dodawanie certyfikat APNS do dzierżawy usługi Intune:

- [Pobierz certyfikat Apple dla aktywnej komunikacji MDM](https://docs.microsoft.com/mem/intune/enrollment/apple-mdm-push-certificate-get)

Jeśli występują problemy z certyfikatem Apple dla aktywnej komunikacji MDM (APNs), zapoznaj się z tym wpisem na blogu: [Usługa Intune i certyfikat APNs — często zadawane pytania i typowe problemy](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)
