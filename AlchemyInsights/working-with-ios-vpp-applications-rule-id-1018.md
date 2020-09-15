---
title: Praca z regułami aplikacji VPP dla systemu iOS o identyfikatorze 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688956"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="a2107-102">Praca z aplikacjami VPP systemu iOS</span><span class="sxs-lookup"><span data-stu-id="a2107-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="a2107-103">W tym artykule [opisano, jak zarządzać aplikacjami z systemem iOS zakupionymi za pośrednictwem programu Volume Purchase Program z usługą Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) , aby uzyskać informacje o funkcjach, ograniczeniach i krokach w celu skorzystania z programu Apple Volume Purchase i pomocy technicznej dla usługi Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="a2107-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="a2107-104">**Typowe problemy:** "Przypisano Ci aplikację VPP systemu iOS do użytkowników, ale instalacja nie powiodła się".</span><span class="sxs-lookup"><span data-stu-id="a2107-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="a2107-105">Może się tak zdarzyć, jeśli jeden token VPP jest wykorzystywany przez wielu dostawców zarządzania urządzeniami przenośnymi.</span><span class="sxs-lookup"><span data-stu-id="a2107-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="a2107-106">Tokeny VPP firmy Apple mogą być używane tylko z jednym dostawcą.</span><span class="sxs-lookup"><span data-stu-id="a2107-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="a2107-107">Jeśli korzystasz z tokenu VPP z wieloma dostawcami, musisz ponownie przekazać token do usługi Intune.</span><span class="sxs-lookup"><span data-stu-id="a2107-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="a2107-108">Instalacja może również zakończyć się niepowodzeniem, jeśli łączna liczba instalacji przekracza liczbę licencji.</span><span class="sxs-lookup"><span data-stu-id="a2107-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="a2107-109">Aby wyświetlić raport użycia licencji, przejdź do **Intune Mobile apps** \> strony **licencje aplikacji** usługi Intune dla urządzeń przenośnych.</span><span class="sxs-lookup"><span data-stu-id="a2107-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="a2107-110">Aby dowiedzieć się, jak odzyskać licencje w użyciu, zobacz [ten artykuł.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="a2107-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
