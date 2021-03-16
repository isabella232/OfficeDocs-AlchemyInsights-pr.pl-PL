---
title: Usuwanie usługi tła dla usługi Microsoft Search z usługi Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816332"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Usuwanie usługi tła dla usługi Microsoft Search z usługi Bing

Aby usunąć usługę tła dla usługi Microsoft Search w usłudze Bing, możesz użyć następujących środków zaradczych:

1. Aby przywrócić oryginalne ustawienia wyszukiwarki, wykonaj następujące czynności:

    a. Wyłącz przełącznik Użyj usługi Bing jako domyślnej **[wyszukiwarki.](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)**

    b. [Przejdź do centrum administracyjnego platformy Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) i wyczyść ustawienie dotyczące wszystkich użytkowników w organizacji.

2. Aby usunąć usługę w tle z pojedynczego urządzenia, wykonaj następujące zadania:

    a. Wybierz **pozycję Panel sterowania > a > a następnie pozycję Programy i funkcje.**

    b. Kliknij prawym przyciskiem **myszy pozycję Microsoft Search w uwitrynie Bing** pod listą zainstalowanych programów, a następnie kliknij polecenie Odinstaluj . 

3. Aby usunąć usługę w tle z wielu urządzeń w organizacji, zaloguj się jako administrator i uruchom następujące polecenie w skrypcie: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
