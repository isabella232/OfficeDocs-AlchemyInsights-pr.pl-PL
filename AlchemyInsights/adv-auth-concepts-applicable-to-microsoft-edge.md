---
title: Pojęcia zaawansowanego uwierzytelniania dotyczące uwierzytelniania Microsoft Edge
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
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934375"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Pojęcia zaawansowanego uwierzytelniania dotyczące uwierzytelniania Microsoft Edge

Poniżej przedstawiono zaawansowane pojęcia dotyczące uwierzytelniania, które mają zastosowanie Microsoft Edge:

**Aktywne uwierzytelnianie**

Po włączeniu zasad [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) użytkownicy Microsoft Edge będą próbować aktywnie uwierzytelniać użytkowników zalogowanych za pośrednictwem usługi firmy Microsoft. W regularnych odstępach czasu usługa online będzie sprawdzać, czy w pliku manifestu nie ma zaktualizowanego pliku manifestu, który zawiera konfigurację, która działa proaktywnie.

Korzyści: Aktywne uwierzytelnianie umożliwia uwierzytelnianie w najważniejszych usługach, takich jak Office nowa karta. Ponadto jeśli Bing jako wyszukiwarka, aktywne uwierzytelnianie zwiększa wydajność paska adresu i pomaga generować wyniki wyszukiwania spersonalizowane do potrzeb Twojej firmy.

**Windows Hello CredUI do uwierzytelniania NTLM**

Jeśli logowanie jednokrotne (SSO) nie jest dostępne, gdy witryna internetowa próbuje zalogować użytkownika za pośrednictwem mechanizmu NTLM lub Negotiate, ta funkcja umożliwi użytkownikowi udostępnianie poświadczeń systemu operacyjnego witrynie internetowej i spełnianie wyzwania związanego z uwierzytelnianiem za pomocą interfejsu użytkownika Windows Hello Cred. Ten przepływ logowania będzie wyświetlany tylko w Windows 10 i tylko dla użytkowników, którzy nie mają logowania jednokrotnego podczas NTLM lub wyzwania Wynegocjuj.

**Automatyczne logowanie przy użyciu zapisanych haseł**

Użytkownicy, którzy zapisują hasła w Microsoft Edge mogą włączyć automatyczne logowanie się w witrynach internetowych, w których zapisano poświadczenia. Użytkownicy mogą włączać i wyłączać tę funkcję w edge://settings/passwords, a także skonfigurować ją w zasadach [menedżera](https://go.microsoft.com/fwlink/?linkid=2134622) haseł.
