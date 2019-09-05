---
title: OneDrive dla Business Web OneDrive przekierowuje do Delve
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
ms.openlocfilehash: 8ba296c6986c767939ef51076551f95719d11aa2
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752258"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="a8d90-102">Przekierowano do Delve po kliknięciu OneDrive</span><span class="sxs-lookup"><span data-stu-id="a8d90-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="a8d90-103">Aby rozwiązać ten problem, administrator pakietu Office 365 musi przyznać użytkownikom prawo do tworzenia witryny Moje witryny.</span><span class="sxs-lookup"><span data-stu-id="a8d90-103">To resolve this problem, the Office 365 administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="a8d90-104">Dzieje się tak, ponieważ na stronie Moje witryny jest tworzona Strona OneDrive dla firm.</span><span class="sxs-lookup"><span data-stu-id="a8d90-104">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="a8d90-105">Aby udzielić tego prawa, wykonaj następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="a8d90-105">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="a8d90-106">W centrum administracyjnego programu SharePoint, kliknij przycisk **Profile użytkownika**.</span><span class="sxs-lookup"><span data-stu-id="a8d90-106">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="a8d90-107">W sekcji **osoby** kliknij przycisk **Zarządzaj uprawnieniami użytkownika**.</span><span class="sxs-lookup"><span data-stu-id="a8d90-107">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="a8d90-108">Dodaj użytkowników, którzy potrzebują uprawnień do tworzenia witryny Moje witryny.</span><span class="sxs-lookup"><span data-stu-id="a8d90-108">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="a8d90-109">Domyślnie to ustawienie jest ustawione dla **wszystkich z wyjątkiem użytkowników zewnętrznych**.</span><span class="sxs-lookup"><span data-stu-id="a8d90-109">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="a8d90-110">Po dodaniu użytkownika, użytkowników lub grupy, upewnij się, że dodano użytkownika, użytkowników lub grupy jest zaznaczone, przewiń do sekcji **uprawnienia** , a następnie zaznacz pole wyboru obok **Tworzenie witryny osobistej (wymagane dla magazynu osobistego, kanału informacyjnego i po treści)**.</span><span class="sxs-lookup"><span data-stu-id="a8d90-110">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="a8d90-111">Kliknij przycisk **OK**, a następnie użytkownik przejdź do strony OneDrive, aby utworzyć witrynę.</span><span class="sxs-lookup"><span data-stu-id="a8d90-111">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
