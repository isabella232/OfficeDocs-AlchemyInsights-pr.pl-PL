---
title: Single-Sign na urządzeniach przyłączony do usługi Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405052"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Logowanie pojedyncze dla urządzeń przyłącznych do usługi Azure Active Directory

Jeśli masz lokalne środowisko usługi Active Directory (AD) i chcesz dołączyć komputery przyłączone do domeny usługi AD do usługi Azure AD, możesz to zrobić, wykonując hybrydowe dołączanie do usługi Azure AD. [Jak to zrobić: Planowanie hybrydowej implementacji](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) dołączania do usługi Azure Active Directory zawiera powiązane kroki implementacji hybrydowego sprzężenia usługi Azure AD w środowisku.

[Konfigurowanie urządzeń przyłącznych do usługi Azure AD dla aplikacji lokalnych Single-Sign przy użyciu funkcji Windows Hello dla firm](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Problemy z tokenem odświeżania podstawowego (PRT)** Token odświeżania podstawowego (PRT) to kluczowy artefakt uwierzytelniania usługi Azure AD na urządzeniach z systemem Windows 10, Windows Server 2016 i nowszych wersjach oraz urządzeniach z systemami iOS i Android. Jest to token sieci Web JSON (JWT) specjalnie wydany dla pierwszego tokenu tokenu zabezpieczającego firmy Microsoft w celu umożliwienia logowania jednokrotnego (SSO) w aplikacjach używanych na tych urządzeniach. [W tece Co to jest token odświeżania podstawowego?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)zostaną ci szczegółowe informacje o tym, jak jest wydany, używany i chroniony prt na urządzeniach z systemem Windows 10.

**WamDefaultSet: YES i AzureADPrt: YES** Te pola wskazują, czy użytkownik pomyślnie uwierzytelnił się w usłudze Azure AD podczas logowania się na urządzeniu. Jeśli wartości to **NIE,** może to być spowodowane:

- Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).
- Alternatywny identyfikator logowania
- Nie znaleziono serwera proxy HTTP

Rozwiązywanie problemów z urządzeniami przy użyciu polecenia dsregcmd — [stan logowania jednokrotnego](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
