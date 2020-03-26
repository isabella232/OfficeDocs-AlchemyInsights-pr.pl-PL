---
title: Nie można zalogować się do usługi Teams z powodu błędu autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932036"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Nie można zalogować się do usługi Teams z powodu błędu autologon.microsoftazuread-sso kropka com:443

Jeśli w uwierzytelnianiu usługi Office 365 jest włączone bezproblemowe logowanie jednokrotne, może być konieczne dodanie adresu URL „autologon.microsoftazuread-sso.com” do witryn intranetowych.  Jeśli został on wcześniej dodany do zaufanych witryn i jest używane bezproblemowe logowanie jednokrotne, należy usunąć go z witryn zaufanych.

Zapoznaj się z [listą kontrolną rozwiązywania problemów bezproblemowego logowania jednokrotnego](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Wykonaj poniższe czynności, aby dodać adres URL do listy witryn intranetowych:

1. Otwórz program Internet Explorer, klikając przycisk **Start**. W polu wyszukiwania wpisz ciąg Internet Explorer, a następnie na liście wyników kliknij pozycję **Internet Explorer**.
2. Kliknij pozycję **Narzędzia**, a następnie kliknij pozycję **Opcje internetowe**.
3. Kliknij kartę **Zabezpieczenia**.
4. Kliknij teraz pozycję **Lokalne witryny intranetowe**, po czym kliknij przycisk **witryny**, a następnie przycisk **Zaawansowane**.
5. Wprowadź adres URL witryny internetowej, a następnie kliknij pozycję **Dodaj**.
6. Po zakończeniu kliknij przycisk **Zamknij**.

Aby uzyskać więcej informacji, zobacz [Dokumentację wdrażania bezproblemowego logowania jednokrotnego w usłudze Office 365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (obejmuje oparty na zasadach proces dodawania adresu URL do witryn intranetowych w kroku 3).
