---
title: Pisanie zwrotne urządzenia
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256857"
---
# <a name="device-writeback"></a>Pisanie zwrotne urządzenia

Dane zwrotne urządzenia są używane w następujących scenariuszach:

- Włączanie [funkcji Windows Hello dla firm przy użyciu wdrożenia hybrydowego zaufania certyfikatów](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Włączanie dostępu warunkowego opartego na urządzeniach w aplikacjach chronionych usługami ADFS (2012 R2 lub wyższym) (zaufania jednostki zależnej)

    > [!NOTE]
    > Do zapisu zwrotnego urządzenia wymagana jest subskrypcja usługi Azure AD Premium.

Zapewnia to dodatkowe zabezpieczenia i zapewnia, że dostęp do aplikacji jest udzielany tylko zaufanym aplikacjom. Aby uzyskać więcej informacji [](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) na temat dostępu warunkowego, zobacz Zarządzanie ryzykiem za pomocą dostępu warunkowego i konfigurowanie dostępu warunkowego w środowisku lokalnym przy użyciu rejestracji [urządzeń usługi Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/devices/overview)

Aby uzyskać więcej informacji na temat włączania funkcji zapisu zwrotnego urządzenia dla urządzeń, zobacz ["Włączanie funkcji zapisu urządzenia".](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)
