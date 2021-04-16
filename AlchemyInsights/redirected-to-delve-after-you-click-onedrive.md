---
title: OneDrive dla Firm Web OneDrive przekierowuje do aplikacji Delve
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799999"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="98807-102">Przekierowywany do aplikacji Delve po kliknięciu przycisku OneDrive</span><span class="sxs-lookup"><span data-stu-id="98807-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="98807-103">Zobacz nasz szczegółowy [przewodnik po rozwiązywaniu problemów.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)</span><span class="sxs-lookup"><span data-stu-id="98807-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="98807-104">Aby rozwiązać ten problem, administrator musi udzielić użytkownikom prawa do tworzenia swoich witryn Moja witryna.</span><span class="sxs-lookup"><span data-stu-id="98807-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="98807-105">Jest tak, ponieważ w moich witrynach jest tworzona strona usługi OneDrive dla Firm.</span><span class="sxs-lookup"><span data-stu-id="98807-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="98807-106">Aby przyznać to prawo, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="98807-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="98807-107">W centrum administracyjnym programu SharePoint kliknij pozycję **Profile użytkowników**.</span><span class="sxs-lookup"><span data-stu-id="98807-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="98807-108">W sekcji **Osoby** kliknij pozycję **Zarządzaj uprawnieniami użytkowników**.</span><span class="sxs-lookup"><span data-stu-id="98807-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="98807-109">Dodaj użytkowników wymagających uprawnień do utworzenia witryny Moja witryna.</span><span class="sxs-lookup"><span data-stu-id="98807-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="98807-110">Domyślnie to ustawienie jest ustawione na Wszyscy **oprócz użytkowników zewnętrznych.**</span><span class="sxs-lookup"><span data-stu-id="98807-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="98807-111">Po dodaniu użytkownika, użytkowników lub grupy upewnij się, że zaznaczono dodanego użytkownika,  użytkowników lub grupę, przewiń do sekcji uprawnień, a następnie zaznacz pole wyboru obok przycisku Utwórz witrynę osobistą (wymagane w przypadku przechowywania osobistego, kanału aktualności i obserwowanej **zawartości).**</span><span class="sxs-lookup"><span data-stu-id="98807-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="98807-112">Kliknij **przycisk OK,** a następnie zachęć użytkownika do przeglądania strony usługi OneDrive w celu utworzenia witryny.</span><span class="sxs-lookup"><span data-stu-id="98807-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
