---
title: Wprowadzenie do usługi SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700717"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="aba0d-102">Przepływy pracy w programie SharePoint</span><span class="sxs-lookup"><span data-stu-id="aba0d-102">Workflows in SharePoint</span></span>

<span data-ttu-id="aba0d-103">Jeśli przepływy pracy programu SharePoint nie są wysyłane pocztą e-mail, być może Twoja organizacja napotkała limity nadawców usługi Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="aba0d-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="aba0d-104">Komunikat o błędzie "przepływ pracy został zawieszony" może wystąpić w przypadku posiadania jednego z następujących elementów:</span><span class="sxs-lookup"><span data-stu-id="aba0d-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="aba0d-105">Masz przepływ pracy w usłudze SharePoint Online, w którym jest używany typ platformy przepływ pracy programu SharePoint 2010 lub SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="aba0d-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="aba0d-106">W ramach przepływu pracy skonfigurowano wysyłanie niestandardowej wiadomości e-mail do ponad 200 użytkowników jednocześnie, ponad 10 000 adresatów dziennie lub więcej niż 30 wiadomości na minutę.</span><span class="sxs-lookup"><span data-stu-id="aba0d-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="aba0d-107">Po uruchomieniu przepływu pracy wiadomość e-mail nie jest wysyłana, a komunikat o błędzie jest wyświetlany, stan wewnętrzny jest ustawiony na zawieszone lub nie można wysłać do adresata.</span><span class="sxs-lookup"><span data-stu-id="aba0d-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="aba0d-108">Aby uzyskać więcej informacji, zapoznaj się z następującym [artykułem](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="aba0d-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

