---
title: Umożliwianie użytkownikowi synchronizowania konta osobistego z kontem służbowym w aplikacji Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813402"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Umożliwianie użytkownikowi synchronizowania konta osobistego z kontem służbowym w aplikacji Microsoft Edge

Upewnij się, że są spełnione następujące kryteria:

- Enterprise Roaming województwa jest włączony w centrum administracyjnym usługi Azure Active Directory, co wymaga subskrypcji usługi Azure Active Directory — wersja Premium lub Enterprise Mobility + Security (EMS). Aby uzyskać więcej informacji, zobacz [Włączanie roamingu Enterprise w sieci Azure Active Directory.](/azure/active-directory/devices/enterprise-state-roaming-enable)
- Spełniliśmy jedno lub oba z następujących kryteriów:
    - Usługa Azure Information Protection jest włączona dla Twojej dzierżawy. Aby uzyskać szczegółowe informacje, [zobacz Aktywowanie ochrony usługi Azure Rights Management z poziomu centrum administracyjne platformy Microsoft 365.](/azure/information-protection/activate-office365)
    - Funkcja Azure Active Directory Enterprise roamingu województwa (ERR) jest włączona dla dowolnego użytkownika lub dzierżawy. Aby uzyskać więcej informacji, zobacz [Co to jest roaming w stanie przedsiębiorstwa?](/azure/active-directory/devices/enterprise-state-roaming-overview).

Jeśli obie opcje, AIP i SYNCHRONIZ, zostaną wyłączone, zostanie wyświetlony komunikat o błędzie informujący użytkowników, że synchronizacja jest niedostępna dla ich kont.
