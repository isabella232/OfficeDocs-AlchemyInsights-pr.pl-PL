---
title: Rozwiązywanie problemów z usługą Microsoft Defender dla pakietu Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801417"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="cdef3-102">Rozwiązywanie problemów z pakietem Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="cdef3-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="cdef3-103">**Powiadomienia o opóźnieniu dostarczenia wiadomości e-mail** ?</span><span class="sxs-lookup"><span data-stu-id="cdef3-103">**Notice delays with email message delivery** ?</span></span> <span data-ttu-id="cdef3-104">Spróbuj skorzystać z opcji dostarczania dynamicznego dla zasad dotyczących bezpiecznych załączników ATP.</span><span class="sxs-lookup"><span data-stu-id="cdef3-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="cdef3-105">Spowoduje to uniknięcie opóźnień dostarczania wiadomości e-mail podczas ochrony adresatów przed złośliwymi plikami.</span><span class="sxs-lookup"><span data-stu-id="cdef3-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="cdef3-106">**Czy chcesz zgłosić fałszywą liczbę dodatnią, czy fałszywą negatywną** ?</span><span class="sxs-lookup"><span data-stu-id="cdef3-106">**Do you want to report false positives or false negatives** ?</span></span> <span data-ttu-id="cdef3-107">Użyj tego linku, aby przesłać plik do analizy: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="cdef3-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="cdef3-108">**Czy wiesz, że możesz włączyć ochronę za pośrednictwem linków bezpiecznego łącza dla wiadomości e-mail wysyłanych między osobami w organizacji** ?</span><span class="sxs-lookup"><span data-stu-id="cdef3-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization** ?</span></span> <span data-ttu-id="cdef3-109">Wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="cdef3-109">Follow these steps:</span></span>
    1. <span data-ttu-id="cdef3-110">Przejdź do https://protection.office.com i zaloguj się.</span><span class="sxs-lookup"><span data-stu-id="cdef3-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="cdef3-111">Przejdź do **Threat management**  >  **Policy**  >  **bezpiecznych linków** zasad zarządzania zagrożeniami.</span><span class="sxs-lookup"><span data-stu-id="cdef3-111">Go to **Threat management** > **Policy** > **Safe Links** .</span></span>
    3. <span data-ttu-id="cdef3-112">W obszarze **zasady dotyczące określonych adresatów** Edytuj (lub Dodaj) zasady.</span><span class="sxs-lookup"><span data-stu-id="cdef3-112">Under **Policies that apply to specific recipients** , edit (or add) a policy.</span></span>
    4. <span data-ttu-id="cdef3-113">Wybierz pozycję **stosuj bezpieczne linki do wiadomości wysłanych w organizacji** .</span><span class="sxs-lookup"><span data-stu-id="cdef3-113">Select **Apply safe links to messages sent within the organization** .</span></span>
    5. <span data-ttu-id="cdef3-114">Zapisz swoje zasady i pozwól na 30 minut na wprowadzenie zmian w celu ich współdziałania z centrum danych.</span><span class="sxs-lookup"><span data-stu-id="cdef3-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="cdef3-115">Aby uzyskać dodatkową pomoc dotyczącą ATP, zobacz [Microsoft Defender dla Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="cdef3-115">To get more help with ATP, see [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>