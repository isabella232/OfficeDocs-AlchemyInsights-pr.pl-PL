---
title: Identyfikator reguły aplikacji VPP systemu iOS 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719967"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="fb728-102">Praca z aplikacjami VPP na iOS</span><span class="sxs-lookup"><span data-stu-id="fb728-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="fb728-103">Przeczytaj [jak zarządzać aplikacjami na iOS zakupionymi za pośrednictwem programu zakupu zbiorczego w usłudze Microsoft Intune,](https://docs.microsoft.com/intune/vpp-apps-ios) aby dowiedzieć się więcej o funkcjach, ograniczeniach i krokach ułatwiania korzystania z programu zakupów zbiorczych Firmy Apple i obsługi technicznej w usłudze Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="fb728-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="fb728-104">**Typowe problemy:** "Przypisano aplikację VPP dla systemu iOS do moich użytkowników, ale instalacja nie powiodła się."</span><span class="sxs-lookup"><span data-stu-id="fb728-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="fb728-105">Może się tak zdarzyć, jeśli pojedynczy token VPP jest używany przez wielu dostawców zarządzania urządzeniami przenośnymi.</span><span class="sxs-lookup"><span data-stu-id="fb728-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="fb728-106">Tokeny VPP firmy Apple mogą być używane tylko z jednym dostawcą.</span><span class="sxs-lookup"><span data-stu-id="fb728-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="fb728-107">Jeśli użyto tokenu VPP z wieloma dostawcami, należy ponownie przekazać token do usługi Intune.</span><span class="sxs-lookup"><span data-stu-id="fb728-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="fb728-108">Instalacja może również zakończyć się niepowodzeniem, jeśli całkowita liczba instalacji przekroczy liczbę licencji.</span><span class="sxs-lookup"><span data-stu-id="fb728-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="fb728-109">Aby wyświetlić raport użycia licencji, przejdź do strony **Licencje** **aplikacji aplikacji intune mobile.** \></span><span class="sxs-lookup"><span data-stu-id="fb728-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="fb728-110">Aby dowiedzieć się, jak odzyskać używane licencje, zobacz [ten artykuł.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="fb728-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
