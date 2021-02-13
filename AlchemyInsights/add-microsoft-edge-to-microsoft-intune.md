---
title: Dodawanie programu Microsoft Edge do usługi Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194515"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="39e6d-102">Dodawanie programu Microsoft Edge do usługi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="39e6d-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="39e6d-103">Aby móc wdrażać, konfigurować, monitorować i chronić program Microsoft Edge dla systemu Windows 10, musisz najpierw dodać go do usługi Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="39e6d-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="39e6d-104">Intune obsługuje program Microsoft Edge 77 i nowsze wersje.</span><span class="sxs-lookup"><span data-stu-id="39e6d-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="39e6d-105">Usługa Intune wykryje wszystkie istniejące wcześniej instalacje przeglądarki Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="39e6d-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="39e6d-106">Jeśli program Microsoft Edge jest zainstalowany w kontekście użytkownika, instalacja systemowa zastąpi instalację w kontekście użytkownika.</span><span class="sxs-lookup"><span data-stu-id="39e6d-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="39e6d-107">Jeśli przeglądarka Microsoft Edge jest zainstalowana w kontekście systemowym, zostanie zgłoszony sukces instalacji.</span><span class="sxs-lookup"><span data-stu-id="39e6d-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="39e6d-108">Preinstalowana przeglądarka Microsoft Edge 77 i nowsze wersje dla wszystkich kanałów w kontekście użytkownika zostaną zastąpione programem Microsoft Edge zainstalowanym w kontekście systemowym.</span><span class="sxs-lookup"><span data-stu-id="39e6d-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="39e6d-109">**Wymagania wstępne**</span><span class="sxs-lookup"><span data-stu-id="39e6d-109">**Prerequisite**</span></span>

<span data-ttu-id="39e6d-110">Windows 10 w wersji 1709 lub nowszej</span><span class="sxs-lookup"><span data-stu-id="39e6d-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="39e6d-111">**Procedura dodawania edge do usługi Intune**</span><span class="sxs-lookup"><span data-stu-id="39e6d-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="39e6d-112">[Skonfiguruj aplikację w usłudze Intune.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="39e6d-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="39e6d-113">[Skonfiguruj informacje o aplikacji.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="39e6d-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="39e6d-114">[Konfigurowanie ustawień aplikacji.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="39e6d-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="39e6d-115">[Wybierz tagi zakresu (opcjonalnie).](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="39e6d-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="39e6d-116">[Dodaj aplikację.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="39e6d-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="39e6d-117">Aby uzyskać więcej pomocy, zobacz [Rozwiązywanie problemów.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="39e6d-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




