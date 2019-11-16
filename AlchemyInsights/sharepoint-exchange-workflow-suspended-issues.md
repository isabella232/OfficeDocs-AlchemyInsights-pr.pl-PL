---
title: Rozpoczynanie pracę z programem SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 5e61491b626bfe75fd26a15ee54be82d9efa19a7
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/15/2019
ms.locfileid: "37766901"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="5e175-102">Przepływy pracy w programie SharePoint</span><span class="sxs-lookup"><span data-stu-id="5e175-102">Workflows in SharePoint</span></span>

<span data-ttu-id="5e175-103">Jeśli przepływy pracy programu SharePoint nie są wysyłanie wiadomości e-mail, organizacja mogła napotkała limity nadawcy Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="5e175-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="5e175-104">Komunikat o błędzie "przepływ pracy jest zawieszone" może wystąpić, jeśli masz jeden z następujących elementów:</span><span class="sxs-lookup"><span data-stu-id="5e175-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="5e175-105">Masz przepływu pracy w programie SharePoint w trybie online, który używa programu SharePoint 2010 lub SharePoint 2013 typ platformy przepływu pracy.</span><span class="sxs-lookup"><span data-stu-id="5e175-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="5e175-106">Przepływ pracy jest skonfigurowany do wysyłania niestandardowej wiadomości e-mail do więcej niż 200 użytkowników w czasie, więcej niż 10 000 adresatów dziennie lub więcej niż 30 wiadomości na minutę.</span><span class="sxs-lookup"><span data-stu-id="5e175-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="5e175-107">Po uruchomieniu przepływu pracy, wiadomość e-mail nie jest wysyłana i można zauważyć komunikat o błędzie, stan wewnętrzny jest ustawiona na zawieszone lub nie można wysłać do adresata jest wyświetlany.</span><span class="sxs-lookup"><span data-stu-id="5e175-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="5e175-108">Aby uzyskać więcej informacji, zapoznaj się z następującym [artykułem](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="5e175-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

