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
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037339"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Rozwiązywanie problemów z logowaniem pojedynczym dla urządzeń przyłącznych do usługi Azure AD

Jeśli masz lokalne środowisko usługi Active Directory (AD) i chcesz dołączyć komputery przyłączone do domeny usługi AD do usługi Azure AD, możesz to zrobić, wykonując hybrydowe dołączanie do usługi Azure AD. [Jak to zrobić: Planowanie hybrydowej implementacji](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) dołączania do usługi Azure Active Directory zawiera powiązane kroki implementacji hybrydowego sprzężenia usługi Azure AD w środowisku.

Aby uzyskać więcej informacji, zobacz Konfigurowanie urządzeń przyłącznych do usługi Azure AD dla urządzeń lokalnychSingle-Sign [Wł. przy użyciu funkcji Windows Hello dla firm.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

**Problemy z tokenem odświeżania podstawowego (PRT)**

Token odświeżania podstawowego (PRT) to kluczowy artefakt uwierzytelniania usługi Azure AD na urządzeniach z systemem Windows 10, Windows Server 2016 i nowszych wersjach oraz urządzeniach z systemami iOS i Android. Jest to token sieci Web JSON (JWT) specjalnie wydany dla pierwszego tokenu tokenu zabezpieczającego firmy Microsoft w celu umożliwienia logowania jednokrotnego (SSO) w aplikacjach używanych na tych urządzeniach. Aby uzyskać szczegółowe informacje o tym, jak jest wystawiany, używany i chroniony prt na urządzeniach z systemem Windows 10, zobacz Co to jest [token odświeżania podstawowego?.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

**WamDefaultSet: YES i AzureADPrt: YES**

Te pola wskazują, czy użytkownik pomyślnie uwierzytelnił się w usłudze Azure AD podczas logowania się na urządzeniu. Jeśli wartości to **NIE,** może to być spowodowane:

- Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)
- Alternatywny identyfikator logowania
- Nie znaleziono serwera proxy HTTP

Aby rozwiązać problemy z urządzeniami przy użyciu polecenia dsregcmd, zobacz [Stan logowania jednokrotnego.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
