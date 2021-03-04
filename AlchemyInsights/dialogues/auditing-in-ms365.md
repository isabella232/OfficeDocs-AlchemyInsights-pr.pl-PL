---
title: Inspekcja na platformy Microsoft 365
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: c07981bfae40d74deb1a2f143ce51da69b51a69f
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430058"
---
# <a name="auditing-in-microsoft-365"></a><span data-ttu-id="1be9d-102">Inspekcja na platformy Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="1be9d-102">Auditing in Microsoft 365</span></span>

<span data-ttu-id="1be9d-103">Oto kilka rzeczy, o których warto wiedzieć na temat inspekcji na platformie Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="1be9d-103">Here are a few things you should know about auditing in Microsoft 365:</span></span>

1. <span data-ttu-id="1be9d-104">Działania administratora programu Exchange są domyślnie włączone do inspekcji.</span><span class="sxs-lookup"><span data-stu-id="1be9d-104">Exchange admin activities are audited by default.</span></span>
1. <span data-ttu-id="1be9d-105">Jesteśmy w trakcie włączania domyślnej inspekcji skrzynki pocztowej dla wszystkich użytkowników.</span><span class="sxs-lookup"><span data-stu-id="1be9d-105">We're in the process of turning on mailbox auditing by default for all users.</span></span> <span data-ttu-id="1be9d-106">Aby dowiedzieć się więcej na ten temat, kliknij [tutaj.](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171)</span><span class="sxs-lookup"><span data-stu-id="1be9d-106">To read more about this, click [here](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171).</span></span> <span data-ttu-id="1be9d-107">Do tego czasu, jeśli chcesz, aby instrukcje dotyczące ręcznego włączania tej funkcji dla jednej osoby lub całej organizacji, wybierz przycisk Włącz inspekcję skrzynki pocztowej poniżej.</span><span class="sxs-lookup"><span data-stu-id="1be9d-107">Until then, if you want instructions to manually enable it for one person or an entire organization, choose the Turn on mailbox auditing button below.</span></span>
1. <span data-ttu-id="1be9d-108">Skrzynki pocztowe grup platformy Microsoft 365 i skrzynki pocztowe folderów publicznych nie obsługują rejestrowania inspekcji.</span><span class="sxs-lookup"><span data-stu-id="1be9d-108">Microsoft 365 Groups mailboxes and Public Folder mailboxes do not support audit logging.</span></span>
1. <span data-ttu-id="1be9d-109">W przypadku programu SharePoint/usługi OneDrive nie jest wymagana żadna dodatkowa konfiguracja, aby włączyć inspekcję.</span><span class="sxs-lookup"><span data-stu-id="1be9d-109">For SharePoint/OneDrive, there is no additional configuration required to enabled auditing.</span></span> <span data-ttu-id="1be9d-110">Aby dowiedzieć się, jakie działania są podlega inspekcji, zobacz:</span><span class="sxs-lookup"><span data-stu-id="1be9d-110">To learn what activities are audited, see:</span></span>
    1. [<span data-ttu-id="1be9d-111">Działania związane z plikami</span><span class="sxs-lookup"><span data-stu-id="1be9d-111">File activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [<span data-ttu-id="1be9d-112">Działania folderów</span><span class="sxs-lookup"><span data-stu-id="1be9d-112">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. <span data-ttu-id="1be9d-113">[Działania związane z udostępnianiem i dostępem.](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)</span><span class="sxs-lookup"><span data-stu-id="1be9d-113">[Sharing and Access activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities).</span></span>
1. <span data-ttu-id="1be9d-114">Aby uzyskać listę wszystkich działań pod kontrolą według usługi, zobacz [Działania zweryfikowane.](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities)</span><span class="sxs-lookup"><span data-stu-id="1be9d-114">For a list of all audited activities by service, see [Audited activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>
