---
title: Usługa OneDrive dla Firm Web OneDrive przekierowuje do aplikacji Delve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: cbf3db148e16ba6631e9077f893a18d3e1b977af
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722820"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="647ae-102">Przekierowano do aplikacji Delve po kliknięciu przycisku OneDrive</span><span class="sxs-lookup"><span data-stu-id="647ae-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="647ae-103">Zapoznaj się ze [szczegółowym przewodnikiem rozwiązywania problemów](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span><span class="sxs-lookup"><span data-stu-id="647ae-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="647ae-104">Aby rozwiązać ten problem, administrator musi przyznać użytkownikom prawo do utworzenia witryny Moje witryny.</span><span class="sxs-lookup"><span data-stu-id="647ae-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="647ae-105">Dzieje się tak, ponieważ strona OneDrive dla Firm jest tworzona w witrynach Moje witryny.</span><span class="sxs-lookup"><span data-stu-id="647ae-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="647ae-106">Aby udzielić tego prawa, wykonaj następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="647ae-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="647ae-107">W centrum administracyjnym programu SharePoint kliknij pozycję **Profile użytkowników**.</span><span class="sxs-lookup"><span data-stu-id="647ae-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="647ae-108">W sekcji **Kontakty** kliknij pozycję **Zarządzaj uprawnieniami użytkowników**.</span><span class="sxs-lookup"><span data-stu-id="647ae-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="647ae-109">Dodaj użytkowników, którzy potrzebują uprawnień, do utworzenia witryny Moje witryny.</span><span class="sxs-lookup"><span data-stu-id="647ae-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="647ae-110">Domyślnie to ustawienie jest ustawione na **Wszyscy z wyjątkiem użytkowników zewnętrznych**.</span><span class="sxs-lookup"><span data-stu-id="647ae-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="647ae-111">Po dodaniu użytkownika, użytkowników lub grupy upewnij się, że dodano użytkownika, użytkowników lub grupę, przewiń do sekcji **uprawnień,** a następnie zaznacz pole wyboru **obok pozycji Utwórz witrynę osobistą (wymagane do przechowywania osobistego, kanału aktualności i obserwowanej zawartości).**</span><span class="sxs-lookup"><span data-stu-id="647ae-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="647ae-112">Kliknij **przycisk OK**, a następnie przejdź do strony usługi OneDrive, aby utworzyć witrynę.</span><span class="sxs-lookup"><span data-stu-id="647ae-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
