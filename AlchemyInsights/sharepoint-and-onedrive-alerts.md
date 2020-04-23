---
title: Opóźnienia w odbieraniu alertów w programie SharePoint i OneDrive
ms.author: v-todmc
author: todmccoy
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
ms.openlocfilehash: fb7ab6e8139c46d89b1cae1ee0ab9b9a601c8b64
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742011"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="c6619-102">Opóźnienia w odbieraniu alertów w programie SharePoint i OneDrive</span><span class="sxs-lookup"><span data-stu-id="c6619-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="c6619-103">Najpierw sprawdź folder Wiadomości-śmieci lub Spam w wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="c6619-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="c6619-104">Jeśli **wszystkie alerty z wielu plików lub bibliotek są opóźnione,** odwiedź [pulpit nawigacyjny kondycji usługi,](https://portal.office.com/adminportal/home?ref=/servicehealth) aby sprawdzić, czy nie ma żadnych porad/incydentów, które mogą występować w programie SharePoint lub Exchange.</span><span class="sxs-lookup"><span data-stu-id="c6619-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="c6619-105">Problem może dotyczyć funkcji alertu programu SharePoint lub opóźnień w wiadomościach e-mail za pośrednictwem programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="c6619-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="c6619-106">Zwróć również uwagę, czy inna wiadomość e-mail jest dostarczana — jeśli nie, problem jest prawdopodobnie opóźniany w programie Exchange.</span><span class="sxs-lookup"><span data-stu-id="c6619-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="c6619-107">Jeśli **pojedynczy alert z określonego pliku lub biblioteki nie zostanie dostarczony,** spróbuj go usunąć i ponownie utworzyć.</span><span class="sxs-lookup"><span data-stu-id="c6619-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="c6619-108">Aby odtworzyć [alert, zobacz Zarządzanie, wyświetlanie lub usuwanie alertów programu SharePoint.](https://support.microsoft.com/office/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)</span><span class="sxs-lookup"><span data-stu-id="c6619-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="c6619-109">Alertów nie można wysyłać do grupy dystrybucyjnej.</span><span class="sxs-lookup"><span data-stu-id="c6619-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="c6619-110">Obsługiwane są tylko grupy zabezpieczeń i O365.</span><span class="sxs-lookup"><span data-stu-id="c6619-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="c6619-111">Nie można dostosować szablonów alertów wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="c6619-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="c6619-112">Aby je osiągnąć, należy użyć usługi Microsoft Flow lub SharePoint Designer Workflow.</span><span class="sxs-lookup"><span data-stu-id="c6619-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
