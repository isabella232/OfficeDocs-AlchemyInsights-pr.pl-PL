---
title: Problemy z zalogowaniem się do aplikacji pakietu Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938295"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Puste — ekran logowania w aplikacjach pakietu Office

Aby rozwiązać ten problem, spróbuj wykonać następujące czynności:
- Zainstaluj najnowsze aktualizacje dla [systemu Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [pakietu Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Resetowanie opcji programu Internet Explorer: Przejdź do **Narzędzia** > **Opcje internetowe** > **Zaawansowane** > **Resetowanie ustawień programu Internet Explorer** (należy zauważyć, że ustawienia niestandardowe zostaną utracone), a następnie spróbuj ponownie zalogować się do urzędu.
- Wyłącz Windows Defender aplikacji Guard (WDAG) lub podobny program zapory lub oprogramowania antywirusowego:
    1. W Panelu sterowania przejdź do **apletu Programy**, a następnie wybierz polecenie **Włącz lub wyłącz funkcje systemu Windows**.
    2. Jeśli straży aplikacji systemu Windows Defender jest włączona, spróbuj ją wyłączyć.<br/>
    **Uwaga:** Konieczne może być ponowne uruchomienie komputera.
- Upewnij się, że Microsoft.AAD.BrokerPlugin [WAM AAD dodatek typu plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nie są blokowane przez aplikację lub program zapory/anty-wirus.
- [Wyczyść Office poświadczeń](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) przy użyciu Menedżera poświadczeń systemu Windows.<br/>
    **Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zostały zmienione na 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Aby uzyskać więcej informacji zobacz [w logowanie po aktualizacji do pakietu Office 2016 build 16.0.7967 w systemie Windows 10 problemy z połączeniem](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).