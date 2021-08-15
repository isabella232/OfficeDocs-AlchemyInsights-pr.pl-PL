---
title: Rozwiązywanie problemów z logowaniem pojedynczym dla urządzeń przyłącznych do usługi Azure AD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039256"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Rozwiązywanie problemów z logowaniem pojedynczym dla urządzeń przyłącznych do usługi Azure AD

Jeśli masz lokalne środowisko usługi Active Directory (AD) i chcesz dołączyć komputery przyłączone do domeny usługi AD do usługi Azure AD, możesz to zrobić, wykonując hybrydowe dołączanie do usługi Azure AD. [Jak to zrobić: Planowanie wdrożenia hybrydowego Azure Active Directory dołączania](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) zawiera powiązane kroki implementacji hybrydowego dołączania do usługi Azure AD w Twoim środowisku.

Aby uzyskać więcej informacji, zobacz Konfigurowanie urządzeń przyłącznych do usługi Azure AD dla urządzeń lokalnych Single-Sign Korzystanie z programu [Windows Hello dla firm.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

**Problemy z tokenem odświeżania podstawowego (PRT)**

Token odświeżania podstawowego (PRT, Primary Refresh Token) to kluczowy artefakt uwierzytelniania usługi Azure AD na urządzeniach Windows 10, Windows Server 2016 i nowszych wersjach oraz urządzeniach z systemami iOS i Android. Jest to token sieci Web JSON (JWT) specjalnie wydany dla pierwszego tokenu tokenu zabezpieczającego firmy Microsoft w celu umożliwienia logowania jednokrotnego (SSO) w aplikacjach używanych na tych urządzeniach. Aby uzyskać szczegółowe informacje o tym, jak jest wystawiany, używany i chroniony prt na Windows 10, zobacz Co to jest [token odświeżania podstawowego?.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

**WamDefaultSet: YES i AzureADPrt: YES**

Te pola wskazują, czy użytkownik pomyślnie uwierzytelnił się w usłudze Azure AD podczas logowania się na urządzeniu. Jeśli wartości to **NIE,** może to być spowodowane:

- Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)
- Alternatywny identyfikator logowania
- Nie znaleziono serwera proxy HTTP

Aby rozwiązać problemy z urządzeniami przy użyciu polecenia dsregcmd, zobacz [Stan logowania jednokrotnego.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
