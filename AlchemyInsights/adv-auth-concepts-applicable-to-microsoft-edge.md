---
title: Pojęcia zaawansowanego uwierzytelniania dotyczące programu Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398595"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Pojęcia zaawansowanego uwierzytelniania dotyczące programu Microsoft Edge

Poniżej przedstawiono pojęcia zaawansowanego uwierzytelniania, które mają zastosowanie do programu Microsoft Edge:

**Aktywne uwierzytelnianie**

Po włączeniu zasad [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) przeglądarka Microsoft Edge będzie próbować aktywnie uwierzytelniać użytkowników zalogowanych za pośrednictwem usług firmy Microsoft. W regularnych odstępach czasu usługa online będzie sprawdzać, czy w pliku manifestu nie ma zaktualizowanego pliku manifestu, który zawiera konfigurację, która działa proaktywnie.

Korzyści: Aktywne uwierzytelnianie umożliwia uwierzytelnianie w najważniejszych usługach, takich jak strona nowej karty pakietu Office. Ponadto jeśli wyszukiwarka jest używana za pomocą usługi Bing, aktywne uwierzytelnianie zwiększa wydajność paska adresu i pomaga generować wyniki wyszukiwania spersonalizowane do potrzeb Twojej firmy.

**Funkcja CredUI funkcji Windows Hello do uwierzytelniania NTLM**

Jeśli logowanie jednokrotne (SSO) nie jest dostępne, gdy witryna internetowa próbuje zalogować użytkownika za pośrednictwem mechanizmu NTLM lub Negotiate, ta funkcja umożliwi użytkownikowi udostępnianie poświadczeń systemu operacyjnego witrynie internetowej i spełnienie wyzwania związanego z uwierzytelnianiem przy użyciu interfejsu użytkownika Wer. Windows Hello. Ten przepływ logowania jest wyświetlany tylko w systemie Windows 10 i tylko dla użytkowników, którzy nie uzyskają logowania jednokrotnego podczas NTLM lub wyzwania Wynegocjuj.

**Automatyczne logowanie przy użyciu zapisanych haseł**

Użytkownicy, którzy zapisują hasła w programie Microsoft Edge, mogą włączyć automatyczne logowanie się do witryn internetowych, w których zapisano poświadczenia. Użytkownicy mogą włączać i wyłączać tę funkcję w edge://settings/passwords, a także skonfigurować ją w zasadach [menedżera](https://go.microsoft.com/fwlink/?linkid=2134622) haseł.
