---
title: Praca z iOS 1018 identyfikator reguły aplikacji VPP
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: a0bbc1f49f251ef4f16300c8cca98e219008d17e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558015"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="30dce-102">Praca z iOS aplikacje VPP</span><span class="sxs-lookup"><span data-stu-id="30dce-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="30dce-103">Przeczytaj, [jak zarządzać aplikacje iOS kupione za pośrednictwem programu zakupu woluminu z usługi Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) Dowiedz się więcej o cechy, ograniczenia i czynności, aby poprawić wykorzystanie programu zakupu zbiorowego Apple i wsparcie dla niego w Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="30dce-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="30dce-104">**Typowych problemów:** "Aplikacja VPP iOS przypisane do moich użytkowników, ale instalacja nie powiodła się".</span><span class="sxs-lookup"><span data-stu-id="30dce-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="30dce-105">Może się to zdarzyć, jeśli pojedynczy token VPP jest używana na wielu dostawców zarządzania urządzenia przenośnego.</span><span class="sxs-lookup"><span data-stu-id="30dce-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="30dce-106">Tokeny VPP, Apple może służyć wyłącznie u jednego dostawcy.</span><span class="sxs-lookup"><span data-stu-id="30dce-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="30dce-107">Jeśli użyto VPP token z wieloma dostawcami, możesz ponownie przesłać token Windows Intune.</span><span class="sxs-lookup"><span data-stu-id="30dce-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="30dce-108">Instalacja może się nie udać, jeśli całkowita ilość instalacji przekracza liczbę licencji.</span><span class="sxs-lookup"><span data-stu-id="30dce-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="30dce-109">Aby wyświetlić raport użycia dla swoich licencji, przejdź do strony **Windows Intune aplikacje** \> strony **licencji aplikacji** .</span><span class="sxs-lookup"><span data-stu-id="30dce-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="30dce-110">Aby dowiedzieć się, jak odzyskać licencje w użyciu, zobacz [w tym artykule.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="30dce-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
