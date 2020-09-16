---
title: Wysyłanie powiadomień niestandardowych za pomocą usługi Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720656"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="65c12-102">Jak wysyłać powiadomienia niestandardowe do użytkowników zarządzanych urządzeń z systemem iOS i Android</span><span class="sxs-lookup"><span data-stu-id="65c12-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="65c12-103">Niestandardowe powiadomienia usługi Intune są przetwarzane przez aplikację Portal firmy na urządzeniu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="65c12-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="65c12-104">Aplikacja następnie utworzy powiadomienie o wypychaniu na tym urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="65c12-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="65c12-105">Poniżej przedstawiono wymagania wstępne dotyczące urządzeń, które umożliwiają otrzymywanie powiadomień niestandardowych, a następnie aplikację do tworzenia powiadomień wypychanych:</span><span class="sxs-lookup"><span data-stu-id="65c12-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="65c12-106">Na urządzeniu musi być zainstalowana aplikacja Portal firmy.</span><span class="sxs-lookup"><span data-stu-id="65c12-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="65c12-107">Urządzenie musi umożliwiać aplikacji Portal firmy wysyłanie powiadomień wypychanych.</span><span class="sxs-lookup"><span data-stu-id="65c12-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="65c12-108">Po zainstalowaniu lub zaktualizowaniu aplikacji zostanie wyświetlony monit o zezwolenie użytkownikowi na powiadomienia.</span><span class="sxs-lookup"><span data-stu-id="65c12-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="65c12-109">Na urządzeniach z systemem Android muszą być zainstalowane usługi Google Play.</span><span class="sxs-lookup"><span data-stu-id="65c12-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="65c12-110">Urządzenie musi być zarejestrowane za pomocą usługi Intune.</span><span class="sxs-lookup"><span data-stu-id="65c12-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="65c12-111">Aby uzyskać więcej informacji, w tym jak wysłać wiadomość, zapoznaj się z [dokumentacją funkcji](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="65c12-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
