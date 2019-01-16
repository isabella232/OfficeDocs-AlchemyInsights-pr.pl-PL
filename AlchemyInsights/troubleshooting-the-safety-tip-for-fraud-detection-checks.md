---
title: Rozwiązywanie problemów-wskazówka bezpieczeństwa dla wykrywania oszustw sprawdza
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 24842e8cc5c6e47fb0eb637e6a3211637ede1ed8
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28304800"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="58cf0-102">Rozwiązywanie problemów-wskazówka bezpieczeństwa dla wykrywania oszustw sprawdza</span><span class="sxs-lookup"><span data-stu-id="58cf0-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="58cf0-p101">Jeśli jesteś coraz wskazówka bezpieczeństwa, który mówi, "nadawca nie powiodło się nasze kontroli wykrywania nadużyć finansowych i nie może być kto wydają się być", a następnie nadawca nie można przekazać DKIM lub SPF uwierzytelniające. Najlepszym sposobem rozwiązania tego problemu jest dla nadawcy do autoryzowania sami. Jeśli nadawca wysyła w Twoim imieniu, musisz autoryzować ich przez dodanie adresu IP nadawcy do rekordu SPF.</span><span class="sxs-lookup"><span data-stu-id="58cf0-p101">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks. The best method to resolve this is for the sender to authorize themselves. If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="58cf0-106">Aby uzyskać więcej informacji, zobacz [Rozwiązywanie problemów-wskazówka czerwony bezpieczeństwa (podejrzane) dla wykrywania oszustw sprawdza](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="58cf0-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="58cf0-107">Oto niektóre łącza, które mogą pomóc:</span><span class="sxs-lookup"><span data-stu-id="58cf0-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="58cf0-108">Jak Office 365 używa struktury zasad dotyczących nadawców (SPF), aby zapobiec podszywaniu</span><span class="sxs-lookup"><span data-stu-id="58cf0-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/en-us/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="58cf0-109">Konfigurowanie funkcji SPF w usłudze Office 365 w celu zapobiegania fałszowaniu</span><span class="sxs-lookup"><span data-stu-id="58cf0-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/en-us/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

