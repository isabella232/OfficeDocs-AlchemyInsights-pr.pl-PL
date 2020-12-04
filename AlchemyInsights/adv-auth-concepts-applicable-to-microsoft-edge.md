---
title: Zaawansowane pojęcia dotyczące uwierzytelniania dotyczące przeglądarki Microsoft Edge
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573526"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Zaawansowane pojęcia dotyczące uwierzytelniania dotyczące przeglądarki Microsoft Edge

Poniżej przedstawiono zaawansowane koncepcje uwierzytelniania dotyczące przeglądarki Microsoft Edge:

**Aktywne uwierzytelnianie**

Po włączeniu zasad [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) program Microsoft Edge będzie próbować aktywnie uwierzytelniać zalogowanych użytkowników za pośrednictwem usług firmy Microsoft. W regularnych odstępach czasu będzie używana usługa online, aby sprawdzić, czy jest dostępny zaktualizowany manifest zawierający konfigurację regulującą aktywne uwierzytelnianie.

Korzyści: aktywne uwierzytelnianie umożliwia uwierzytelnianie na najważniejszych usługach, takich jak strona nowej karty pakietu Office. Ponadto, jeśli usługa Bing jest używana jako wyszukiwarka, Funkcja aktywnego uwierzytelniania zwiększa wydajność paska adresu i pomaga wygenerować wyniki wyszukiwania, które są personalizowane do potrzeb Twojej firmy.

**Windows Hello CredUI dla uwierzytelniania NTLM**

Jeśli funkcja logowania jednokrotnego (SSO) jest niedostępna, gdy witryna sieci Web usiłuje zalogować się do użytkownika za pomocą mechanizmu NTLM lub Negotiate, ta funkcja umożliwi użytkownikowi udostępnianie poświadczeń systemu operacyjnego w witrynie sieci Web i zaspokojenie tego wezwania uwierzytelniania przy użyciu interfejsu użytkownika usługi Windows Hello Credentials. Ten przepływ logowania będzie wyświetlany tylko w systemie Windows 10 i tylko dla użytkowników, którzy nie korzystają z rejestracji jednokrotnej w protokole NTLM lub negocjacyjnym.

**Automatyczne logowanie przy użyciu zapisanych haseł**

Użytkownicy, którzy zapisują hasła w przeglądarce Microsoft Edge, mogą włączyć automatyczne logowanie do witryn internetowych, w których mają zapisane poświadczenia. Użytkownicy mogą włączać i wyłączać tę funkcję w edge://settings/passwords, a także można ją skonfigurować w zasadach [Menedżera haseł](https://go.microsoft.com/fwlink/?linkid=2134622) .
