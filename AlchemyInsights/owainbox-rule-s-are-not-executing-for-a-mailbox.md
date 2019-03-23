---
title: 1332 OWA - reguł skrzynki odbiorczej są nie może być wykonane dla skrzynki pocztowej
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9e782faa59bb9a16c271f7c46c79635961e88aed
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30784351"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="1b52c-102">Reguły skrzynki odbiorczej nie działa zgodnie z oczekiwaniami</span><span class="sxs-lookup"><span data-stu-id="1b52c-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="1b52c-103">Sprawdź następujące ustawienia:</span><span class="sxs-lookup"><span data-stu-id="1b52c-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="1b52c-104">Wiadomości mogą być przekierowane, przekazany został lub odpowiedzi automatycznie na podstawie reguł skrzynki odbiorczej tylko jeden raz.</span><span class="sxs-lookup"><span data-stu-id="1b52c-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="1b52c-105">Trwa przeadresowanie reguła (reguła skrzynki odbiorczej lub reguły przepływu poczty, znany również jako reguły transportu) można dodać maksymalnie dziesięć adresatów przekazywanie do wiadomości.</span><span class="sxs-lookup"><span data-stu-id="1b52c-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="1b52c-106">Aby uzyskać więcej informacji zobacz [ograniczenia reguły dziennika, transportu i skrzynki odbiorczej](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="1b52c-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="1b52c-107">Reguły skrzynki odbiorczej nie działają na Skrzynka pocztowa dziennika alternatywny.</span><span class="sxs-lookup"><span data-stu-id="1b52c-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="1b52c-108">Aby uzyskać więcej informacji o skrzynce pocztowej rejestrowanie alternatywny zobacz [Skrzynka pocztowa dziennika alternatywny](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="1b52c-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="1b52c-109">Aby rozwiązać te problemy, zobacz [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="1b52c-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="1b52c-110">Jeżeli nie stosuje się poprzednie wydania, uruchom raport diagnostyczny reguły skrzynki odbiorczej przed zgłosić ten problem firmie Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="1b52c-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="1b52c-111">Otwieranie skrzynki pocztowej w programie Outlook w sieci web, a następnie kliknij przycisk **Ustawienia** \> **Opcje** \> **e-mail Organizuj** \> **reguł skrzynki odbiorczej**.</span><span class="sxs-lookup"><span data-stu-id="1b52c-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="1b52c-112">U dołu strony kliknij przycisk **Jeśli reguły nie działają kliknij tutaj, aby wygenerować raport diagnostyczny**.</span><span class="sxs-lookup"><span data-stu-id="1b52c-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    

