---
title: Rozwiązywanie problemów z poradami dotyczącymi bezpieczeństwa dla kontroli wykrywania nadużyć
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658420"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="f20eb-102">Rozwiązywanie problemów z poradami dotyczącymi bezpieczeństwa dla kontroli wykrywania nadużyć</span><span class="sxs-lookup"><span data-stu-id="f20eb-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="f20eb-103">Jeśli otrzymasz poradę dotyczącą bezpieczeństwa, na której znajduje się komunikat "nadawca nie mógł sprawdzić, czy nasze testy wykrywania nadużyć finansowych, i może nie być", oznacza to, że nadawca nie przeszedł testów uwierzytelniania DKIM lub SPF.</span><span class="sxs-lookup"><span data-stu-id="f20eb-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="f20eb-104">Najlepszym sposobem na rozwiązanie tego problemu jest udzielenie nadawcy autoryzacji.</span><span class="sxs-lookup"><span data-stu-id="f20eb-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="f20eb-105">Jeśli nadawca wysyła dane w Twoim imieniu, trzeba je autoryzować, dodając adres IP nadawcy do rekordu SPF.</span><span class="sxs-lookup"><span data-stu-id="f20eb-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="f20eb-106">Zobacz [Rozwiązywanie problemów z czerwonymi (podejrzanymi) wskazówkami dotyczącymi wykrywania nadużyć](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) , aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="f20eb-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="f20eb-107">Oto kilka innych linków, które mogą pomóc:</span><span class="sxs-lookup"><span data-stu-id="f20eb-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="f20eb-108">Jak firma Microsoft używa struktury zasad nadawców (SPF) w celu zapobiegania podszywaniu się</span><span class="sxs-lookup"><span data-stu-id="f20eb-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="f20eb-109">Konfigurowanie SPF w celu zapobiegania podszywaniu się</span><span class="sxs-lookup"><span data-stu-id="f20eb-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
