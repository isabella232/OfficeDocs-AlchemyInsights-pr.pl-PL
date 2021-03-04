---
title: Inspekcja na platformy Microsoft 365
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: c07981bfae40d74deb1a2f143ce51da69b51a69f
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430058"
---
# <a name="auditing-in-microsoft-365"></a>Inspekcja na platformy Microsoft 365

Oto kilka rzeczy, o których warto wiedzieć na temat inspekcji na platformie Microsoft 365:

1. Działania administratora programu Exchange są domyślnie włączone do inspekcji.
1. Jesteśmy w trakcie włączania domyślnej inspekcji skrzynki pocztowej dla wszystkich użytkowników. Aby dowiedzieć się więcej na ten temat, kliknij [tutaj.](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171) Do tego czasu, jeśli chcesz, aby instrukcje dotyczące ręcznego włączania tej funkcji dla jednej osoby lub całej organizacji, wybierz przycisk Włącz inspekcję skrzynki pocztowej poniżej.
1. Skrzynki pocztowe grup platformy Microsoft 365 i skrzynki pocztowe folderów publicznych nie obsługują rejestrowania inspekcji.
1. W przypadku programu SharePoint/usługi OneDrive nie jest wymagana żadna dodatkowa konfiguracja, aby włączyć inspekcję. Aby dowiedzieć się, jakie działania są podlega inspekcji, zobacz:
    1. [Działania związane z plikami](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [Działania folderów](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. [Działania związane z udostępnianiem i dostępem.](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
1. Aby uzyskać listę wszystkich działań pod kontrolą według usługi, zobacz [Działania zweryfikowane.](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities)
