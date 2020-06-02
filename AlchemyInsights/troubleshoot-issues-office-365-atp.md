---
title: Rozwiązywanie problemów z zaawansowaną ochroną przed zagrożeniami usługi Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511122"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="a976b-102">Rozwiązywanie problemów z usługi Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="a976b-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="a976b-103">**Powiadomienie o opóźnieniach z dostarczaniem wiadomości e-mail?**</span><span class="sxs-lookup"><span data-stu-id="a976b-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="a976b-104">Spróbuj użyć opcji dostarczania dynamicznego dla zasad bezpiecznych załączników ATP.</span><span class="sxs-lookup"><span data-stu-id="a976b-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="a976b-105">Pozwoli to uniknąć opóźnień w dostarczaniu wiadomości e-mail, chroniąc jednocześnie adresatów przed złośliwymi plikami.</span><span class="sxs-lookup"><span data-stu-id="a976b-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="a976b-106">**Czy chcesz zgłosić fałszywe alarmy lub fałszywe negatywy?**</span><span class="sxs-lookup"><span data-stu-id="a976b-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="a976b-107">Użyj tego linku, aby przesłać plik do analizy:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="a976b-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="a976b-108">**Czy wiesz, że możesz włączyć ochronę ATP Safe Links dla poczty e-mail wysyłanej między osobami w organizacji?**</span><span class="sxs-lookup"><span data-stu-id="a976b-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="a976b-109">Wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="a976b-109">Follow these steps:</span></span>
    1. <span data-ttu-id="a976b-110">Przejdź do https://protection.office.com , i zaloguj się.</span><span class="sxs-lookup"><span data-stu-id="a976b-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="a976b-111">Przejdź do **zasad zarządzania zagrożeniami**  >  **Policy**  >  **Bezpieczne linki**.</span><span class="sxs-lookup"><span data-stu-id="a976b-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="a976b-112">W obszarze **Zasady dotyczące określonych adresatów**edytuj (lub dodaj) zasady.</span><span class="sxs-lookup"><span data-stu-id="a976b-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="a976b-113">Wybierz **pozycję Zastosuj bezpieczne łącza do wiadomości wysyłanych w organizacji**.</span><span class="sxs-lookup"><span data-stu-id="a976b-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="a976b-114">Zapisz zasady i pozwól na około 30 minut, aby zmiany działały w centrum danych.</span><span class="sxs-lookup"><span data-stu-id="a976b-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="a976b-115">Aby uzyskać więcej pomocy w temacie ATP, zobacz [Zaawansowana ochrona przed zagrożeniami usługi Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="a976b-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>