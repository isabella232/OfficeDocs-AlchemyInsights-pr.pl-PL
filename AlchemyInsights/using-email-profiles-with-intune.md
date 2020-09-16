---
title: Korzystanie z profilów e-mail w usłudze Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653298"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="467a2-102">Korzystanie z profilów e-mail w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="467a2-102">Using email profiles with Intune</span></span>

<span data-ttu-id="467a2-103">Usługa Intune może służyć do tworzenia i wdrażania profilów e-mail dla macierzystego (wbudowanego) klienta poczty e-mail na wielu platformach urządzeń.</span><span class="sxs-lookup"><span data-stu-id="467a2-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="467a2-104">Aby uzyskać informacje na temat ograniczeń dotyczących profilów e-mail, w tym sposobu obsługi obecności istniejących profilów i usuwania profilów poczty e-mail, zobacz [Dodawanie ustawień poczty e-mail do urządzeń przy użyciu usługi Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="467a2-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="467a2-105">Aby uzyskać więcej informacji na temat tworzenia profilów poczty e-mail dla poszczególnych platform urządzeń, zobacz:</span><span class="sxs-lookup"><span data-stu-id="467a2-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="467a2-106">Ustawienia urządzeń z systemem Android umożliwiające konfigurowanie poczty e-mail, uwierzytelniania i synchronizacji w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="467a2-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="467a2-107">Dodawanie ustawień poczty e-mail dla urządzeń z systemem iOS i iPadOS w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="467a2-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="467a2-108">Ustawienia profilu e-mail w usłudze Microsoft Intune dla urządzeń z systemem Windows Phone 8,1</span><span class="sxs-lookup"><span data-stu-id="467a2-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="467a2-109">Ustawienia profilu e-mail dotyczące urządzeń z systemem Windows 10 w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="467a2-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="467a2-110">**Typowy problem z synchronizacją**</span><span class="sxs-lookup"><span data-stu-id="467a2-110">**Common syncing issue**</span></span>

<span data-ttu-id="467a2-111">**Profil e-mail w programie KNOX w systemie Android uniemożliwia zsynchronizowanie z innymi użytkownikami kontaktów, kalendarza i zadań.**</span><span class="sxs-lookup"><span data-stu-id="467a2-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="467a2-112">Profil e-mail KNOX w systemie Android KNOX oferuje administratorowi możliwość podjęcia decyzji, które typy zawartości są synchronizowane z urządzeniem przez ustawienie każdego do włączenia.</span><span class="sxs-lookup"><span data-stu-id="467a2-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="467a2-113">Jeśli ustawienie dla dowolnego typu zawartości jest skonfigurowane jako **Nieskonfigurowane** (domyślne), ten typ zawartości nie jest synchronizowany automatycznie.</span><span class="sxs-lookup"><span data-stu-id="467a2-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="467a2-114">Użytkownik może włączyć ten typ zawartości bezpośrednio na urządzeniu, ale ta konfiguracja zostanie zastąpiona przez ustawienie zasad usługi Intune, a synchronizacja zostanie zatrzymana dla tego typu zawartości.</span><span class="sxs-lookup"><span data-stu-id="467a2-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

