---
title: Usługa OneDrive dla firm w sieci Web usługi OneDrive umożliwia przekierowanie do aplikacji Delve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776389"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="8bae2-102">Przekierowano do aplikacji Delve po kliknięciu usługi OneDrive</span><span class="sxs-lookup"><span data-stu-id="8bae2-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="8bae2-103">Zobacz szczegółowy [Przewodnik dotyczący rozwiązywania problemów](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span><span class="sxs-lookup"><span data-stu-id="8bae2-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="8bae2-104">Aby rozwiązać ten problem, administrator musi udzielić użytkownikom prawa do tworzenia witryny Moja witryna.</span><span class="sxs-lookup"><span data-stu-id="8bae2-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="8bae2-105">Jest to spowodowane tym, że w witrynach Moja witryna jest tworzona Strona usługi OneDrive dla firm.</span><span class="sxs-lookup"><span data-stu-id="8bae2-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="8bae2-106">Aby udzielić tego prawa, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="8bae2-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="8bae2-107">W centrum administracyjnym programu SharePoint kliknij pozycję **Profile użytkowników**.</span><span class="sxs-lookup"><span data-stu-id="8bae2-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="8bae2-108">W sekcji **kontakty** kliknij pozycję **Zarządzaj uprawnieniami użytkownika**.</span><span class="sxs-lookup"><span data-stu-id="8bae2-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="8bae2-109">Dodaj użytkowników, którzy wymagają uprawnień do tworzenia witryny Moja witryna.</span><span class="sxs-lookup"><span data-stu-id="8bae2-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="8bae2-110">Domyślnie to ustawienie jest ustawione dla **wszystkich użytkowników poza użytkownikami zewnętrznymi**.</span><span class="sxs-lookup"><span data-stu-id="8bae2-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="8bae2-111">Po dodaniu użytkownika, użytkowników lub grupy upewnij się, że jest zaznaczony dodany użytkownik, użytkownicy lub Grupa, przewiń do sekcji **uprawnienia** , a następnie zaznacz pole wyboru obok pozycji **Utwórz witrynę osobistą (wymagane dla magazynu osobistego, kanału aktualności i obserwowanej zawartości)**.</span><span class="sxs-lookup"><span data-stu-id="8bae2-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="8bae2-112">Kliknij przycisk **OK**, a następnie przejdź do strony usługi OneDrive, aby utworzyć witrynę.</span><span class="sxs-lookup"><span data-stu-id="8bae2-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
