---
title: Rozwiązywanie problemów z poradami w zakresie bezpieczeństwa podczas sprawdzania wykrywania oszustw
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834741"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="57396-102">Rozwiązywanie problemów z poradami w zakresie bezpieczeństwa podczas sprawdzania wykrywania oszustw</span><span class="sxs-lookup"><span data-stu-id="57396-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="57396-103">Jeśli jest wyświetlana porada o bezpieczeństwie z treścią informacji "Nadawca zakończył testy wykrywania oszustw i może nie być tym, kto tak jest", oznacza to, że nadawca nie przejdzie testów uwierzytelniania DKIM lub SPF.</span><span class="sxs-lookup"><span data-stu-id="57396-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="57396-104">Najlepszą metodą rozwiązania tego problemu jest autoryzacja siebie przez nadawcę.</span><span class="sxs-lookup"><span data-stu-id="57396-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="57396-105">Jeśli nadawca wysyła w Twoim imieniu, musisz autoryzować go, dodając adres IP nadawcy do Twojego rekordu SPF.</span><span class="sxs-lookup"><span data-stu-id="57396-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="57396-106">Aby uzyskać więcej informacji, zobacz Rozwiązywanie problemów dotyczących [czerwonej (podejrzanej) porady](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) dotyczącej bezpieczeństwa w przypadku wykrywania oszustw.</span><span class="sxs-lookup"><span data-stu-id="57396-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="57396-107">Oto kilka innych linków, które mogą pomóc:</span><span class="sxs-lookup"><span data-stu-id="57396-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="57396-108">Jak firma Microsoft używa struktury zasad dotyczących nadawców (SPF) w celu zapobiegania fałszowania</span><span class="sxs-lookup"><span data-stu-id="57396-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="57396-109">Konfigurowanie spf w celu zapobiegania fałszerszem</span><span class="sxs-lookup"><span data-stu-id="57396-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
