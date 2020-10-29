---
title: Rozwiązywanie problemów z programem Microsoft Defender dla pakietu Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801453"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="91d2d-102">Rozwiązywanie problemów z programem Microsoft Defender dla pakietu Office 365</span><span class="sxs-lookup"><span data-stu-id="91d2d-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="91d2d-103">Czy zauważysz opóźnienia dostarczenia wiadomości?</span><span class="sxs-lookup"><span data-stu-id="91d2d-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="91d2d-104">Użyj opcji [dostarczania dynamicznego](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) w zasadach bezpiecznych załączników ATP.</span><span class="sxs-lookup"><span data-stu-id="91d2d-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="91d2d-105">Pomoże to uniknąć opóźnień w wiadomościach chroniących adresatów przed złośliwymi plikami.</span><span class="sxs-lookup"><span data-stu-id="91d2d-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="91d2d-106">Czy chcesz zgłosić fałszywie dodatnie lub fałszywe wartości ujemne firmie Microsoft?</span><span class="sxs-lookup"><span data-stu-id="91d2d-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="91d2d-107">Użyj tego [linku](https://www.microsoft.com/wdsi/filesubmission/) , aby przesłać pliki do analizy.</span><span class="sxs-lookup"><span data-stu-id="91d2d-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="91d2d-108">Czy wiesz, że możesz włączyć ochronę przed linkami dla wewnętrznych wiadomości e-mail wysyłanych między adresatami w organizacji?</span><span class="sxs-lookup"><span data-stu-id="91d2d-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="91d2d-109">Wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="91d2d-109">Follow these steps:</span></span>

  1. <span data-ttu-id="91d2d-110">Przejdź do [https://protection.office.com](https://protection.office.com) i zaloguj się przy użyciu konta administratora globalnego lub administratora zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="91d2d-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="91d2d-111">W lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami** wybierz pozycję **zasady** \> **bezpieczne linki** .</span><span class="sxs-lookup"><span data-stu-id="91d2d-111">In the left navigation pane under **Threat management** , choose **Policy** \> **Safe Links** .</span></span>

  3. <span data-ttu-id="91d2d-112">W **zasadach, które dotyczą całej sekcji organizacji** , zaznacz odpowiednie zasady i kliknij pozycję **Edytuj** .</span><span class="sxs-lookup"><span data-stu-id="91d2d-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit** .</span></span>

  4. <span data-ttu-id="91d2d-113">W obszarze **Ustawienia** Włącz opcję **Zastosuj bezpieczne linki do wiadomości wysłanych w organizacji** .</span><span class="sxs-lookup"><span data-stu-id="91d2d-113">Under **Settings** , enable **Apply safe links to messages sent within the organization** .</span></span>
