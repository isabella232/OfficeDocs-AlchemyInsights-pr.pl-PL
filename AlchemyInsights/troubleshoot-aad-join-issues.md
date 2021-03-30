---
title: Rozwiązywanie problemów z dołączaniem do usługi Azure AD
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
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405132"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Rozwiązywanie problemów z dołączaniem do usługi Azure AD

1. Jeśli używasz rejestracji urządzeń po raz pierwszy, sprawdź wprowadzenie do zarządzania urządzeniami w usłudze [Azure Active Directory,](https://docs.microsoft.com/azure/active-directory/devices/overview) które zawiera wskazówki dotyczące sposobu kontrolowania przez urządzenia usługi Azure AD. 
1. Jeśli rejestrujesz urządzenia bezpośrednio w usłudze Azure AD i zapisujesz je w usłudze Intune, musisz najpierw upewnić się, że skonfigurowano usługę [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) i że w pierwszej kolejności są [one](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) stosowane.
1. Upewnij się, że masz uprawnienia do wykonywania operacji w usłudze Azure AD. Tylko administrator globalny w usłudze Azure AD może zarządzać ustawieniami rejestracji urządzeń.
1. Aby wykonać implementację dołączania do usługi Azure AD, zobacz [Planowanie dołączenia do usługi Azure AD.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

Aby uzyskać więcej szczegółowych informacji na temat rozwiązywania typowych problemów dotyczących dołączania do usługi Azure AD, zobacz Często zadawane pytania dotyczące dołączania do usługi [Azure Ad,](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) a w przypadku urządzeń z systemem Windows 10 Pro zobacz Nie można dołączyć komputera z systemem [Windows 10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) do usługi Azure AD — konieczność uaktualnienia do — Microsoft Community
