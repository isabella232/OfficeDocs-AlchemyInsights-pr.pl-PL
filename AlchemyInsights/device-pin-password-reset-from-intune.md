---
title: Resetowanie numeru PIN/hasła urządzenia z usługi Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1278"
- "6700008"
ms.openlocfilehash: fd3bb957b0da22dfab5a9988a82e398757e12ee5
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440088"
---
# <a name="device-pinpassword-reset-from-intune"></a><span data-ttu-id="e653e-102">Resetowanie numeru PIN/hasła urządzenia z usługi Intune</span><span class="sxs-lookup"><span data-stu-id="e653e-102">Device pin/password reset from Intune</span></span>

<span data-ttu-id="e653e-103">Możesz usunąć kod dostępu lub wymusić na użytkowniku utworzenie nowego kodu dostępu w usłudze Intune dla urządzenia z systemem iOS lub Android przy użyciu akcji Usuń kod dostępu.</span><span class="sxs-lookup"><span data-stu-id="e653e-103">You can remove a passcode or force a user to create a new passcode in Intune for a device running iOS or Android by using the Remove Passcode action.</span></span>

<span data-ttu-id="e653e-104">Ta akcja obsługuje tylko określone typy systemów operacyjnych i profil pracy.</span><span class="sxs-lookup"><span data-stu-id="e653e-104">Only specific operating system types and work profile types support this action.</span></span>

<span data-ttu-id="e653e-105">Aby uzyskać szczegółowe informacje na temat obsługiwanych platform i sposobu wyzwalania akcji resetowania kodu dostępu, zobacz [Resetowanie lub usuwanie kodu dostępu urządzenia w usłudze Intune](https://docs.microsoft.com/intune/device-passcode-reset).</span><span class="sxs-lookup"><span data-stu-id="e653e-105">For details about supported platforms and how to trigger the reset passcode action, see [Reset or remove a device passcode in Intune](https://docs.microsoft.com/intune/device-passcode-reset).</span></span>

<span data-ttu-id="e653e-106">Istniejący pin można zresetować do nowej wartości, korzystając z akcji Resetowanie pinów na urządzeniach z systemem operacyjnym Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="e653e-106">You can reset an existing pin to a new value using the Pin Reset action on devices running the Windows 10 Mobile operating system.</span></span> <span data-ttu-id="e653e-107">Dzięki temu użytkownik może odblokować urządzenie i odpowiednio ustawić nowy kod PIN.</span><span class="sxs-lookup"><span data-stu-id="e653e-107">This allows the user to unlock the device and set a new pin as appropriate.</span></span> <span data-ttu-id="e653e-108">Aby uzyskać więcej informacji, zobacz [Resetowanie kodu na urządzeniach z systemem Windows przy użyciu usługi Intune](https://docs.microsoft.com/intune/device-windows-pin-reset).</span><span class="sxs-lookup"><span data-stu-id="e653e-108">For more info, see [Reset the passcode on Windows devices using Intune](https://docs.microsoft.com/intune/device-windows-pin-reset).</span></span>