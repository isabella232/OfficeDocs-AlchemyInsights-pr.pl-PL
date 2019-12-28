---
title: Wysyłanie niestandardowych powiadomień za pomocą usługi Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886867"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="ed2ae-102">Jak wysyłać niestandardowe powiadomienia do użytkowników zarządzanych urządzeń z systemem iOS i Android</span><span class="sxs-lookup"><span data-stu-id="ed2ae-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="ed2ae-103">Niestandardowe powiadomienia dla usługi Intune są przetwarzane przez aplikację Portal firmy na urządzeniu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="ed2ae-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="ed2ae-104">Następnie aplikacja utworzy powiadomienie push na tym urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="ed2ae-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="ed2ae-105">Poniżej przedstawiono wymagania wstępne dotyczące urządzeń do obsługi otrzymania niestandardowych powiadomień, a dla aplikacji, aby następnie utworzyć powiadomienie push:</span><span class="sxs-lookup"><span data-stu-id="ed2ae-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="ed2ae-106">Urządzenie musi mieć zainstalowaną aplikację Portal firmy.</span><span class="sxs-lookup"><span data-stu-id="ed2ae-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="ed2ae-107">Urządzenie musi zezwalać aplikacji Portal firmy na wysyłanie powiadomień wypychanych.</span><span class="sxs-lookup"><span data-stu-id="ed2ae-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="ed2ae-108">Po zainstalowaniu lub zaktualizowaniu aplikacji będzie monitować użytkownika o zezwolenie na powiadomienia.</span><span class="sxs-lookup"><span data-stu-id="ed2ae-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="ed2ae-109">Urządzenia z Androidem muszą mieć zainstalowane usługi Google Play.</span><span class="sxs-lookup"><span data-stu-id="ed2ae-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="ed2ae-110">Urządzenie musi być zarejestrowane w usłudze Intune.</span><span class="sxs-lookup"><span data-stu-id="ed2ae-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="ed2ae-111">Aby uzyskać więcej informacji, w tym jak wysłać wiadomość, zobacz [dokumentację funkcji](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="ed2ae-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
