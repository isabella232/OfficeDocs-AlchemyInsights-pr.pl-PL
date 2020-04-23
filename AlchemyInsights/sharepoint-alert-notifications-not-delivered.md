---
title: Powiadomienia alertów programu SharePoint nie zostały dostarczone
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: a422805d11a128909e1be7bf5d08b24efc132e23
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742057"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="ef251-102">Powiadomienia alertów programu SharePoint nie zostały dostarczone</span><span class="sxs-lookup"><span data-stu-id="ef251-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="ef251-103">Sprawdź folder ŚMIECI w wiadomości e-mail, ponieważ czasami mogą tam trafić alerty.</span><span class="sxs-lookup"><span data-stu-id="ef251-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="ef251-104">Określ, czy **wszystkie alerty nie są dostarczane** lub jeśli pojedynczy **alert** z określonego pliku lub biblioteki nie jest dostarczany.</span><span class="sxs-lookup"><span data-stu-id="ef251-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="ef251-105">**Poszczególne alerty nie są dostarczane:** Jeśli pojedynczy alert z określonego pliku lub biblioteki nie zostanie dostarczony, można spróbować go usunąć i ponownie utworzyć.</span><span class="sxs-lookup"><span data-stu-id="ef251-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="ef251-106">Aby odtworzyć [alert, zobacz Zarządzanie, wyświetlanie lub usuwanie alertów programu SharePoint.](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)</span><span class="sxs-lookup"><span data-stu-id="ef251-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="ef251-107">**Wszystkie alerty nie są dostarczane:** Jeśli wszystkie alerty z wielu plików lub bibliotek nie są dostarczane, odwiedź [pulpit nawigacyjny kondycji usługi,](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) aby sprawdzić, czy nie ma żadnych porad/incydentów, które mogą występować w programie SharePoint lub Exchange.</span><span class="sxs-lookup"><span data-stu-id="ef251-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="ef251-108">Problem może dotyczyć funkcji alertu programu SharePoint lub opóźnień w wiadomościach e-mail za pośrednictwem programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="ef251-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="ef251-109">Ważne będzie również, aby pamiętać, czy inna wiadomość e-mail jest dostarczana, a jeśli nie, problem jest prawdopodobnie związany z opóźnieniami programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="ef251-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="ef251-110">Często zadawane pytania dotyczące alertów:</span><span class="sxs-lookup"><span data-stu-id="ef251-110">FAQ on alerts:</span></span>

- <span data-ttu-id="ef251-111">Nie można wysyłać alertów do grupy dystrybucyjnej, obsługiwane są tylko grupy zabezpieczeń i usługi O365.</span><span class="sxs-lookup"><span data-stu-id="ef251-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="ef251-112">Nie można dostosować szablonów alertów poczty e-mail; aby je osiągnąć, musisz użyć programu Microsoft FLOW lub SharePoint Designer Workflow.</span><span class="sxs-lookup"><span data-stu-id="ef251-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

<span data-ttu-id="ef251-113">Więcej informacji:</span><span class="sxs-lookup"><span data-stu-id="ef251-113">More Information:</span></span>

- <span data-ttu-id="ef251-114">**Konfiguracja alertów:** Aby uzyskać więcej informacji na temat konfigurowania alertów, zobacz [Tworzenie alertu, aby otrzymywać powiadomienia o zmianie pliku lub folderu w programie SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span><span class="sxs-lookup"><span data-stu-id="ef251-114">**Alert setup**: For more information about setting up alerts, see [Create an alert to get notified when a file or folder changes in SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span></span>
- <span data-ttu-id="ef251-115">**Rozwiązywanie problemów z alertami:** Aby uzyskać więcej informacji na temat alertów dotyczących rozwiązywania problemów, zobacz [Użytkownicy nie otrzymują powiadomień o alertach usługi SharePoint Online](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span><span class="sxs-lookup"><span data-stu-id="ef251-115">**Troubleshoot alerts**: For more information about troubleshooting alerts, see [Users don't receive SharePoint Online alert notifications](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span></span>
- <span data-ttu-id="ef251-116">**Zaawansowane zasady alertów zgodności usługi O365**: Aby uzyskać więcej informacji na temat konfigurowania tych alertów, zobacz [Zasady alertów zgodności](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="ef251-116">**Advanced O365 Compliance Alert Policies**: For more information about setting up these alerts, see [Compliance Alert Policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>
- <span data-ttu-id="ef251-117">**Dzienniki inspekcji programu SharePoint i OneDrive**: Aby uzyskać więcej informacji na temat pobierania tych zdarzeń, zobacz [Wyszukiwanie dziennika inspekcji](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="ef251-117">**SharePoint and OneDrive Audit Logs**: For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
- <span data-ttu-id="ef251-118">**Alerty wysyłane przez zaawansowaną ochronę przed zagrożeniami:** Zobacz [ATP dla programu SharePoint i OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="ef251-118">**Alerts sent by Advanced Threat Protection**: See [ATP for SharePoint and OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
- <span data-ttu-id="ef251-119">**Alerty wysyłane przez zasady zapobiegania utracie danych**: Zobacz [powiadomienia e-mail dla zasad DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="ef251-119">**Alerts sent by Data Loss Prevention polices**: See [Email notifications for DLP policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

## <a name="related-topics"></a><span data-ttu-id="ef251-120">Tematy pokrewne</span><span class="sxs-lookup"><span data-stu-id="ef251-120">Related Topics</span></span>

<span data-ttu-id="ef251-121">Chcesz wypróbować usługę Microsoft Flow w usłudze SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="ef251-121">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="ef251-122">Utwórz przepływ</span><span class="sxs-lookup"><span data-stu-id="ef251-122">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="ef251-123">Program SharePoint i przepływ</span><span class="sxs-lookup"><span data-stu-id="ef251-123">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
