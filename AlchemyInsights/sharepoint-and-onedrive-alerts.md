---
title: Opóźnienia w otrzymywaniu alertów programu SharePoint i usługi OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 92e517ae6e83aa91b9838047ec77759dc893bc57
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/17/2020
ms.locfileid: "46785675"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="63920-102">Opóźnienia w otrzymywaniu alertów programu SharePoint i usługi OneDrive</span><span class="sxs-lookup"><span data-stu-id="63920-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="63920-103">Najpierw sprawdź folder wiadomości-śmieci lub spam w wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="63920-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="63920-104">Jeśli **wszystkie alerty z wielu plików lub bibliotek są opóźnione**, odwiedź [pulpit nawigacyjny kondycja usługi](https://portal.office.com/adminportal/home?ref=/servicehealth) , aby sprawdzić, jakie klasyfikatory/incydenty mogą wystąpić w programie SharePoint lub programie Exchange.</span><span class="sxs-lookup"><span data-stu-id="63920-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="63920-105">Problem może dotyczyć funkcji alertów programu SharePoint lub opóźnień w wiadomościach e-mail za pośrednictwem programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="63920-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="63920-106">Sprawdź także, czy jest dostarczany inny adres e-mail — Jeśli nie, prawdopodobnie problem dotyczy opóźnień programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="63920-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="63920-107">Jeśli **pojedynczy alert z określonego pliku lub biblioteki nie jest dostarczany**, spróbuj go usunąć i utworzyć ponownie.</span><span class="sxs-lookup"><span data-stu-id="63920-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="63920-108">Zobacz [Zarządzanie, wyświetlanie lub usuwanie alertów programu SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) w celu ponownego utworzenia alertu.</span><span class="sxs-lookup"><span data-stu-id="63920-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="63920-109">Nie można wysyłać alertów do grupy dystrybucyjnej.</span><span class="sxs-lookup"><span data-stu-id="63920-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="63920-110">Obsługiwane są tylko grupy zabezpieczeń i usługi Office 365.</span><span class="sxs-lookup"><span data-stu-id="63920-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="63920-111">Nie można dostosowywać szablonów wiadomości e-mail dotyczących alertów.</span><span class="sxs-lookup"><span data-stu-id="63920-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="63920-112">Aby uzyskać te zmiany, należy użyć przepływu pracy Microsoft Flow lub SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="63920-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
