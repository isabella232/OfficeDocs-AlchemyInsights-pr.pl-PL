---
title: Odmowa dostępu podczas wyświetlania przepływu pracy
ms.author: pebaum
author: pebaum
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 1cfda8e08ada05858a28f2bede8c31261f9de351
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050535"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="f85ae-102">Odmowa dostępu podczas wyświetlania przepływu pracy</span><span class="sxs-lookup"><span data-stu-id="f85ae-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="f85ae-103">SharePoint 2013 przepływy pracy, które próbują wysłać wiadomość e-mail do grupy programu SharePoint może zakończyć się niepowodzeniem z komunikatem o błędzie "odmowa dostępu", jeśli członkostwo w grupie programu SharePoint nie jest ustawiona na wszyscy.</span><span class="sxs-lookup"><span data-stu-id="f85ae-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="f85ae-104">**Aby rozwiązać ten problem, wykonaj następujące kroki:**</span><span class="sxs-lookup"><span data-stu-id="f85ae-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="f85ae-105">Zezwalaj wszystkim, aby zobaczyć członków grupy programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f85ae-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="f85ae-106">Usuń grupę programu SharePoint z wiersza do lub DW wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="f85ae-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="f85ae-107">Jawnie dodać użytkowników do do lub DW wiersza, jeśli nie można zmienić widoczność członkostwa dla grupy programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f85ae-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="f85ae-108">Aby wyświetlić więcej szczegółów, zapoznaj się z [http nieautoryzowane do/_vti_bin/Client.svc/Sp.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="f85ae-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  