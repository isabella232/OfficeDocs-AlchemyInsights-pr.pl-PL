---
title: Stan domeny — nie wybrano usług
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 1ddf6475e7cf466a39f76486e0f809097917657bc8f4ae7f7f2b516657308f39
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947453"
---
# <a name="domain-status---no-services-selected"></a>Stan domeny — nie wybrano usług

**Brak** zaznaczonych usług oznacza, że nie wybrano żadnych usług Microsoft 365, takich jak Exchange Online, Skype dla firm lub Intune, oraz Zarządzanie urządzeniami przenośnymi dla usługi Microsoft 365 do użytku z domeną niestandardową. Jeśli używasz hybrydowego programu Exchange (Exchange lokalnego z usługą Exchange Online) lub zewnętrznego filtrowania spamu z usługą Exchange i nie używasz żadnego innego usługi firmy Microsoft, możesz zignorować ten komunikat. Stan kondycji domeny jest dostępny tylko dla domen połączonych bezpośrednio z usługą.

Aby wybrać usługi dla swojej domeny:

1. Z **Ustawienia** Domains (Domeny) zaznacz pole wyboru obok domeny z komunikatem  >  [](https://admin.microsoft.com/Adminportal/Home)o stanie **Brak zaznaczonych usług.**
1. Wybierz **pozycję Zarządzaj systemem DNS,** aby uruchomić Kreatora konfiguracji domeny.
    - Jeśli wybierzesz **pozycję Dodaj własne rekordy DNS,** pamiętaj, aby po wyświetleniu monitu wybrać usługę. Więcej usług może być dostępnych w **obszarze Opcje zaawansowane.**
    - Jeśli wybierzesz **pozycję Pozwól firmie Microsoft dodać rekordy DNS** lub Więcej opcji Skonfiguruj moje usługi online dla mnie wszystkie dostępne usługi są sugerowane   >   i wybierane automatycznie.
1. Kontynuuj korzystanie z kreatora, aby ukończyć konfigurację systemu DNS i wybrać usługi.
 
Aby uzyskać dodatkową pomoc na temat konfigurowania domeny, zobacz [Dodawanie rekordów DNS w celu połączenia domeny.](/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

