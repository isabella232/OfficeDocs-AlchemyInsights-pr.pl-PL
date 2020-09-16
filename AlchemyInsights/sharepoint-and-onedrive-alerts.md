---
title: Opóźnienia w otrzymywaniu alertów programu SharePoint i usługi OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727253"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="057dc-102">Opóźnienia w otrzymywaniu alertów programu SharePoint i usługi OneDrive</span><span class="sxs-lookup"><span data-stu-id="057dc-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="057dc-103">Najpierw sprawdź folder wiadomości-śmieci lub spam w wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="057dc-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="057dc-104">Jeśli **wszystkie alerty z wielu plików lub bibliotek są opóźnione**, odwiedź [pulpit nawigacyjny kondycja usługi](https://portal.office.com/adminportal/home?ref=/servicehealth) , aby sprawdzić, jakie klasyfikatory/incydenty mogą wystąpić w programie SharePoint lub programie Exchange.</span><span class="sxs-lookup"><span data-stu-id="057dc-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="057dc-105">Problem może dotyczyć funkcji alertów programu SharePoint lub opóźnień w wiadomościach e-mail za pośrednictwem programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="057dc-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="057dc-106">Sprawdź także, czy jest dostarczany inny adres e-mail — Jeśli nie, prawdopodobnie problem dotyczy opóźnień programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="057dc-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="057dc-107">Jeśli **pojedynczy alert z określonego pliku lub biblioteki nie jest dostarczany**, spróbuj go usunąć i utworzyć ponownie.</span><span class="sxs-lookup"><span data-stu-id="057dc-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="057dc-108">Zobacz [Zarządzanie, wyświetlanie lub usuwanie alertów programu SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) w celu ponownego utworzenia alertu.</span><span class="sxs-lookup"><span data-stu-id="057dc-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="057dc-109">Nie można wysyłać alertów do grupy dystrybucyjnej.</span><span class="sxs-lookup"><span data-stu-id="057dc-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="057dc-110">Obsługiwane są tylko grupy zabezpieczeń i usługi Office 365.</span><span class="sxs-lookup"><span data-stu-id="057dc-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="057dc-111">Nie można dostosowywać szablonów wiadomości e-mail dotyczących alertów.</span><span class="sxs-lookup"><span data-stu-id="057dc-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="057dc-112">Aby uzyskać te zmiany, należy użyć przepływu pracy Microsoft Flow lub SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="057dc-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
