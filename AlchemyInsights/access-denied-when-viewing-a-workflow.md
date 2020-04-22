---
title: Odmowa dostępu podczas wyświetlania przepływu pracy
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687340"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="c21b1-102">Odmowa dostępu podczas wyświetlania przepływu pracy</span><span class="sxs-lookup"><span data-stu-id="c21b1-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="c21b1-103">Przepływy pracy programu SharePoint 2013, które próbują wysłać wiadomość e-mail do grupy programu SharePoint, mogą zakończyć się niepowodzeniem, za pomocą komunikatu o błędzie "Odmowa dostępu", jeśli członkostwo w grupie programu SharePoint nie jest ustawione na Wszyscy.</span><span class="sxs-lookup"><span data-stu-id="c21b1-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="c21b1-104">**Aby rozwiązać ten problem, wykonaj następujące czynności:**</span><span class="sxs-lookup"><span data-stu-id="c21b1-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="c21b1-105">Zezwalaj wszystkim na wyświetlanie członków grupy programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c21b1-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="c21b1-106">Usuń grupę programu SharePoint z wiersza Do lub DW wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="c21b1-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="c21b1-107">Jawnie dodaj użytkowników do linii Do lub DW, jeśli nie można zmienić widoczności członkostwa dla grupy programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c21b1-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="c21b1-108">Aby wyświetlić więcej szczegółów, zapoznaj się z [http nieautoryzowane do /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="c21b1-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  