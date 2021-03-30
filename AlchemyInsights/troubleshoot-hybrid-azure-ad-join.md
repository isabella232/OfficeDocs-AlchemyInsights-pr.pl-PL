---
title: Rozwiązywanie problemów z dołączeniem hybrydowym do usługi Microsoft Azure Active Directory
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401917"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Rozwiązywanie problemów z dołączeniem hybrydowym do usługi Microsoft Azure Active Directory

Zdecydowanie zalecane: upewnij się, że urządzenie może uzyskać dostęp do punktów końcowych usługi Device Registration w ramach konta systemowego przy użyciu [skryptu Testowanie łączności rejestracji urządzeń](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Jeśli po raz pierwszy konfigurujesz rejestracje urządzeń, upewnij się, że przejrzany został artykuł W[prowadzenie do zarządzania urządzeniami w usłudze Microsoft Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/), aby dowiedzieć się, w jaki sposób kontrolować urządzenia w usłudze Microsoft Azure Active Directory.
1. Jeśli rejestrujesz urządzenia bezpośrednio w usłudze Microsoft Azure Active Directory i zapisujesz je w usłudze Intune, upewnij się najpierw, że [usługa Intune jest skonfigurowana](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) i posiada [licencjonowanie](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Upewnij się, że masz uprawnienia do wykonywania operacji w usłudze Microsoft Azure Active Directory i lokalnej usłudze Active Directory. Tylko administrator globalny w usłudze Microsoft Azure Active Directory może zarządzać ustawieniami w przypadku rejestracji urządzeń. Jeśli dodatkowo konfigurujesz automatyczne rejestracje w lokalnej usłudze Active Directory, musisz być administratorem usługi Active Directory i usług federacyjnych Active Directory (o ile mają zastosowanie).

W celu uzyskania więcej informacji szczegółowych na temat rozwiązywania potencjalnych problemów, zobacz artykuł [Rozwiązywanie problemów z dołączeniem hybrydowym](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) w zakresie konfiguracji przyłączonej hybrydowo do usługi Azure AD, a w przypadku Zarządzania urządzeniami przy użyciu portalu usługi Azure AD, zobacz [Konfigurowanie urządzeń przyłączonych hybrydowo do usługi Azure AD (przyłączonych do domeny lokalnej)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) i [Zarządzanie urządzeniami przy użyciu Azure Portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Aby rozwiązać typowe problemy z dołączaniem hybrydowym do usługi Microsoft Azure Active Directory, zobacz [Dołączanie hybrydowe do usługi Azure AD — często zadawane pytania](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
