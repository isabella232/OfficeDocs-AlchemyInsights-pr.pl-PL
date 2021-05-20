---
title: Rozwiązywanie problemów z usługą Microsoft Defender dla Office 365
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
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545278"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="0e7f7-102">Rozwiązywanie problemów z usługą Microsoft Defender dla Office 365</span><span class="sxs-lookup"><span data-stu-id="0e7f7-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="0e7f7-103">**Czy zauważysz opóźnienia w dostarczania wiadomości?**</span><span class="sxs-lookup"><span data-stu-id="0e7f7-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="0e7f7-104">Użyj opcji [Dostarczanie dynamiczne](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) w programie Microsoft Defender dla Office 365 Sejf załączników.</span><span class="sxs-lookup"><span data-stu-id="0e7f7-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="0e7f7-105">Pozwoli to uniknąć opóźnień wiadomości podczas ochrony adresatów przed złośliwymi plikami.</span><span class="sxs-lookup"><span data-stu-id="0e7f7-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="0e7f7-106">**Czy chcesz zgłosić do firmy Microsoft wyniki fałszywie dodatnie lub ujemne?**</span><span class="sxs-lookup"><span data-stu-id="0e7f7-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="0e7f7-107">Użyj [Eksploratora przesyłania](https://protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="0e7f7-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="0e7f7-108">-\*\* Czy wiesz, że możesz włączyć ochronę linków Sejf-mail dla wewnętrznej poczty e-mail wysyłanej między adresatami w organizacji?\*\* Wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="0e7f7-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="0e7f7-109">Przejdź do konta administratora globalnego lub administratora zabezpieczeń i [https://protection.office.com](https://protection.office.com) zaloguj się do tego konta.</span><span class="sxs-lookup"><span data-stu-id="0e7f7-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="0e7f7-110">W lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami** wybierz **pozycję Linki** \> **Sejf zasad.**</span><span class="sxs-lookup"><span data-stu-id="0e7f7-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="0e7f7-111">W **sekcji Zasady stosowane do całej organizacji** wybierz zasady, a następnie kliknij pozycję **Edytuj**.</span><span class="sxs-lookup"><span data-stu-id="0e7f7-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="0e7f7-112">W **Ustawienia** wiadomości włącz opcję **Zastosuj bezpieczne linki do wiadomości wysyłanych w ramach organizacji.**</span><span class="sxs-lookup"><span data-stu-id="0e7f7-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
