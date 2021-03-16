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
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="7a7df-102">Usuwanie usługi tła dla usługi Microsoft Search z usługi Bing</span><span class="sxs-lookup"><span data-stu-id="7a7df-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="7a7df-103">Aby usunąć usługę tła dla usługi Microsoft Search w usłudze Bing, możesz użyć następujących środków zaradczych:</span><span class="sxs-lookup"><span data-stu-id="7a7df-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="7a7df-104">Aby przywrócić oryginalne ustawienia wyszukiwarki, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="7a7df-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="7a7df-105">a.</span><span class="sxs-lookup"><span data-stu-id="7a7df-105">a.</span></span> <span data-ttu-id="7a7df-106">Wyłącz przełącznik Użyj usługi Bing jako domyślnej **[wyszukiwarki.](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)**</span><span class="sxs-lookup"><span data-stu-id="7a7df-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="7a7df-107">b.</span><span class="sxs-lookup"><span data-stu-id="7a7df-107">b.</span></span> <span data-ttu-id="7a7df-108">[Przejdź do centrum administracyjnego platformy Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) i wyczyść ustawienie dotyczące wszystkich użytkowników w organizacji.</span><span class="sxs-lookup"><span data-stu-id="7a7df-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="7a7df-109">Aby usunąć usługę w tle z pojedynczego urządzenia, wykonaj następujące zadania:</span><span class="sxs-lookup"><span data-stu-id="7a7df-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="7a7df-110">a.</span><span class="sxs-lookup"><span data-stu-id="7a7df-110">a.</span></span> <span data-ttu-id="7a7df-111">Wybierz **pozycję Panel sterowania > a > a następnie pozycję Programy i funkcje.**</span><span class="sxs-lookup"><span data-stu-id="7a7df-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="7a7df-112">b.</span><span class="sxs-lookup"><span data-stu-id="7a7df-112">b.</span></span> <span data-ttu-id="7a7df-113">Kliknij prawym przyciskiem **myszy pozycję Microsoft Search w uwitrynie Bing** pod listą zainstalowanych programów, a następnie kliknij polecenie Odinstaluj . </span><span class="sxs-lookup"><span data-stu-id="7a7df-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="7a7df-114">Aby usunąć usługę w tle z wielu urządzeń w organizacji, zaloguj się jako administrator i uruchom następujące polecenie w skrypcie:</span><span class="sxs-lookup"><span data-stu-id="7a7df-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
