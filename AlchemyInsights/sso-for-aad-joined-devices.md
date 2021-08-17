---
title: Single-Sign na urządzeniach Azure Active Directory jest wł.
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
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050020"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Logowanie pojedyncze dla Azure Active Directory dołączanych

Jeśli masz lokalne środowisko usługi Active Directory (AD) i chcesz dołączyć komputery przyłączone do domeny usługi AD do usługi Azure AD, możesz to zrobić, wykonując hybrydowe dołączanie do usługi Azure AD. [Jak to zrobić: Planowanie wdrożenia hybrydowego Azure Active Directory dołączania](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) zawiera powiązane kroki implementacji hybrydowego dołączania do usługi Azure AD w Twoim środowisku.

[Konfigurowanie urządzeń przyłączowanych do usługi Azure AD dla usługi Single-Sign Wł. przy Windows Hello dla firm](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Problemy z tokenem odświeżania podstawowego (PRT)** Token odświeżania podstawowego (PRT, Primary Refresh Token) to kluczowy artefakt uwierzytelniania usługi Azure AD na urządzeniach Windows 10, Windows Server 2016 i nowszych wersjach oraz urządzeniach z systemami iOS i Android. Jest to token sieci Web JSON (JWT) specjalnie wydany dla pierwszego tokenu tokenu zabezpieczającego firmy Microsoft w celu umożliwienia logowania jednokrotnego (SSO) w aplikacjach używanych na tych urządzeniach. [W tece Co to jest token odświeżania podstawowego?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)zostaną ci szczegółowe informacje o tym, jak jest wystawiany, używany i chroniony prt na Windows 10 urządzeniach.

**WamDefaultSet: YES i AzureADPrt: YES** Te pola wskazują, czy użytkownik pomyślnie uwierzytelnił się w usłudze Azure AD podczas logowania się na urządzeniu. Jeśli wartości to **NIE,** może to być spowodowane:

- Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).
- Alternatywny identyfikator logowania
- Nie znaleziono serwera proxy HTTP

Rozwiązywanie problemów z urządzeniami przy użyciu polecenia dsregcmd — [stan logowania jednokrotnego](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
