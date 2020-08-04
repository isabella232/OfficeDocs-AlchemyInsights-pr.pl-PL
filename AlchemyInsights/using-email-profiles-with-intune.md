---
title: Korzystanie z profili poczty e-mail w usłudze Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555249"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="3b134-102">Korzystanie z profili poczty e-mail w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="3b134-102">Using email profiles with Intune</span></span>

<span data-ttu-id="3b134-103">Usługa Intune może służyć do tworzenia i wdrażania profilów poczty e-mail dla macierzystego (wbudowanego) klienta poczty e-mail na wielu platformach urządzeń.</span><span class="sxs-lookup"><span data-stu-id="3b134-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="3b134-104">Aby uzyskać informacje o niektórych ograniczeniach związanych z profilami poczty e-mail, w tym o sposobie obsługi obecności istniejących profili i usuwaniu profilów poczty e-mail, zobacz [Dodawanie ustawień poczty e-mail do urządzeń korzystających z usługi Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="3b134-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="3b134-105">Aby uzyskać więcej informacji na temat tworzenia profilów poczty e-mail dla każdej platformy urządzeń, zobacz:</span><span class="sxs-lookup"><span data-stu-id="3b134-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="3b134-106">Ustawienia urządzenia z systemem Android do konfigurowania poczty e-mail, uwierzytelniania i synchronizacji w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="3b134-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="3b134-107">Dodawanie ustawień poczty e-mail dla urządzeń z systemem iOS i iPadOS w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3b134-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="3b134-108">Ustawienia profilu poczty e-mail w usłudze Microsoft Intune dla urządzeń z systemem Windows Phone 8.1</span><span class="sxs-lookup"><span data-stu-id="3b134-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="3b134-109">Ustawienia profilu poczty e-mail dla urządzeń z systemem Windows 10 w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3b134-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="3b134-110">**Typowy problem z synchronizacją**</span><span class="sxs-lookup"><span data-stu-id="3b134-110">**Common syncing issue**</span></span>

<span data-ttu-id="3b134-111">**Knox w profilu e-mail systemu Android uniemożliwia synchronizację kontaktów użytkownika, kalendarza i zadań z urządzeniami użytkownika.**</span><span class="sxs-lookup"><span data-stu-id="3b134-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="3b134-112">Knox na Android KNOX profil e-mail oferuje administratorowi możliwość zdecydować, które typy zawartości są sync'd do urządzenia, ustawiając każdy z nich włączone.</span><span class="sxs-lookup"><span data-stu-id="3b134-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="3b134-113">Jeśli ustawienie dla dowolnego typu zawartości jest ustawione na **Nie skonfigurowano (domyślnie),** ten typ zawartości nie jest synchronizowany automatycznie.</span><span class="sxs-lookup"><span data-stu-id="3b134-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="3b134-114">Użytkownik może ręcznie włączyć żądany typ zawartości bezpośrednio na urządzeniu, ale ta konfiguracja jest zastępowana przez ustawienie zasad usługi Intune, a synchronizacja zostanie zatrzymana dla tego typu zawartości.</span><span class="sxs-lookup"><span data-stu-id="3b134-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

