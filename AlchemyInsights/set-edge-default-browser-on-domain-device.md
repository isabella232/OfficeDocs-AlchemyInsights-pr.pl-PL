---
title: Ustawianie programu Microsoft Edge jako domyślnej przeglądarki na urządzeniu przyłączony do domeny
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491883"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="d9abf-102">Ustawianie programu Microsoft Edge jako domyślnej przeglądarki na urządzeniu przyłączony do domeny</span><span class="sxs-lookup"><span data-stu-id="d9abf-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="d9abf-103">Ustaw przeglądarkę Microsoft Edge jako domyślną:</span><span class="sxs-lookup"><span data-stu-id="d9abf-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="d9abf-104">[Utwórz plik konfiguracji skojarzeń domyślnych](https://go.microsoft.com/fwlink/?linkid=2132437) i przechowuj go lokalnie lub w udziału sieciowym.</span><span class="sxs-lookup"><span data-stu-id="d9abf-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="d9abf-105">Otwórz edytor zasady grupy, a następnie przejdź do strony **Szablony** administracyjne konfiguracji komputera Eksplorator plików składników  >    >    >  **systemu** Windows.</span><span class="sxs-lookup"><span data-stu-id="d9abf-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="d9abf-106">Wybierz **pozycję Ustaw plik konfiguracji skojarzeń domyślnych**.</span><span class="sxs-lookup"><span data-stu-id="d9abf-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="d9abf-107">Wybierz **ustawienie zasad**, a następnie wybierz pozycję **Włączone**.</span><span class="sxs-lookup"><span data-stu-id="d9abf-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="d9abf-108">W **obszarze** Opcje wprowadź lokalizację pliku konfiguracji skojarzeń domyślnych, a następnie wybierz przycisk **OK.**</span><span class="sxs-lookup"><span data-stu-id="d9abf-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
