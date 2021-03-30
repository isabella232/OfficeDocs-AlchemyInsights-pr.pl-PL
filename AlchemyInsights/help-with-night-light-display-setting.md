---
title: Pomoc w ustawieniu wyświetlania wyświetlania nocnego
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404668"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="cfa09-102">Pomoc w ustawieniu wyświetlania wyświetlania nocnego</span><span class="sxs-lookup"><span data-stu-id="cfa09-102">Help with the night light display setting</span></span>

<span data-ttu-id="cfa09-103">Aby dowiedzieć się więcej o ustawieniach wyświetlania nocnego, zobacz Ustawianie czasu wyświetlania nocnego w [systemie Windows 10.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)</span><span class="sxs-lookup"><span data-stu-id="cfa09-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="cfa09-104">Jeśli opcje wyświetlania nocnego są wyszarowane w ustawieniach, sprawdź sterownik ekranu:</span><span class="sxs-lookup"><span data-stu-id="cfa09-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="cfa09-105">Kliknij pole wyszukiwania na pasku zadań i wpisz **Menedżer urządzeń**, a następnie wybierz pozycję **Menedżer urządzeń** w wynikach wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="cfa09-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="cfa09-106">Rozwiń **kartę graficzną**.</span><span class="sxs-lookup"><span data-stu-id="cfa09-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="cfa09-107">Niestety, funkcja wyświetlania nocnego nie jest dostępna, jeśli w urządzeniu jest używany sterownik DisplayLink lub sterownik Ekranu podstawowego.</span><span class="sxs-lookup"><span data-stu-id="cfa09-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="cfa09-108">Funkcja wyświetlania nocnego korzysta z najnowszej technologii graficznej, więc może być konieczne zaktualizowanie sterownika ekranu:</span><span class="sxs-lookup"><span data-stu-id="cfa09-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="cfa09-109">Sprawdź aktualizacje, przechodząc do menu **Start**  >  **Settings**  >  **Update & Security** Windows  >    >  **UpdateS sprawdzaj aktualizacje.**</span><span class="sxs-lookup"><span data-stu-id="cfa09-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="cfa09-110">LUB</span><span class="sxs-lookup"><span data-stu-id="cfa09-110">OR</span></span>

- <span data-ttu-id="cfa09-111">Aby ręcznie pobrać i zainstalować najnowsze sterowniki ekranu, odwiedź witrynę internetową pomocy technicznej producenta sprzętu.</span><span class="sxs-lookup"><span data-stu-id="cfa09-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="cfa09-112">Resetowanie nocnego światła w rejestrze</span><span class="sxs-lookup"><span data-stu-id="cfa09-112">Reset night light in the registry</span></span>

<span data-ttu-id="cfa09-113">Jeśli aktualizacja sterownika ekranu nie działa, może być konieczne zresetowanie wyświetlania nocnego w rejestrze.</span><span class="sxs-lookup"><span data-stu-id="cfa09-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="cfa09-114">**Przestroga:** Ten krok rozwiązywania problemów jest zalecany tylko dla użytkowników zaawansowanych.</span><span class="sxs-lookup"><span data-stu-id="cfa09-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="cfa09-115">Niepoprawne zmodyfikowanie rejestru może być związane z poważnych problemami.</span><span class="sxs-lookup"><span data-stu-id="cfa09-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="cfa09-116">Aby uzyskać dodatkową ochronę, przed zmodyfikowaniem rejestru należy utworzyć jego kopię zapasową, aby można było przywrócić go w przypadku wystąpienia problemów.</span><span class="sxs-lookup"><span data-stu-id="cfa09-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="cfa09-117">W polu wyszukiwania wpisz **regedit**, a następnie wybierz pozycję **Edytor rejestru** w wynikach wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="cfa09-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="cfa09-118">Przejdź do następującego klucza rejestru:</span><span class="sxs-lookup"><span data-stu-id="cfa09-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="cfa09-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="cfa09-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="cfa09-120">Eksportuj, a następnie usuń następujący podklucz:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="cfa09-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="cfa09-121">Wyeksportuj, a następnie usuń następujący podklucz:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="cfa09-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="cfa09-122">Uruchom ponownie system Windows i sprawdź, czy są dostępne opcje światła nocnego.</span><span class="sxs-lookup"><span data-stu-id="cfa09-122">Restart Windows and verify if the night light options are available.</span></span>


