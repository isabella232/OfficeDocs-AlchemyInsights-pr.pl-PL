---
title: Rozwiązywanie problemów z wskazówką dotyczącą bezpieczeństwa podczas kontroli wykrywania oszustw
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759522"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="a3073-102">Rozwiązywanie problemów z wskazówką dotyczącą bezpieczeństwa podczas kontroli wykrywania oszustw</span><span class="sxs-lookup"><span data-stu-id="a3073-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="a3073-103">Jeśli otrzymujesz wskazówkę dotyczącą bezpieczeństwa z napisem "Nadawca nie przeszedł naszych kontroli wykrywania oszustw i może nie być tym, kim wydają się być", nadawca nie przeszedł kontroli uwierzytelniania DKIM lub SPF.</span><span class="sxs-lookup"><span data-stu-id="a3073-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="a3073-104">Najlepszą metodą rozwiązania tego problemu jest autoryzowanie przez nadawcę.</span><span class="sxs-lookup"><span data-stu-id="a3073-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="a3073-105">Jeśli nadawca wysyła w Twoim imieniu, musisz je autoryzować, dodając adres IP nadawcy do rekordu SPF.</span><span class="sxs-lookup"><span data-stu-id="a3073-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="a3073-106">Aby uzyskać więcej informacji, zobacz [Rozwiązywanie problemów z czerwoną (podejrzaną) wskazówką dotyczącą bezpieczeństwa, aby uzyskać](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="a3073-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="a3073-107">Oto kilka innych linków, które mogą pomóc:</span><span class="sxs-lookup"><span data-stu-id="a3073-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="a3073-108">Jak firma Microsoft korzysta z struktury zasad nadawców (SPF), aby zapobiec fałszowaniu</span><span class="sxs-lookup"><span data-stu-id="a3073-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="a3073-109">Konfigurowanie filtra SPF w celu zapobiegania fałszowaniu</span><span class="sxs-lookup"><span data-stu-id="a3073-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
