---
title: Powiadomienia alertów programu SharePoint nie są dostarczane
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: d01d985f34d782fe14b3e2e6e6696c0101002db1
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36744651"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="201b5-102">Powiadomienia alertów programu SharePoint nie są dostarczane</span><span class="sxs-lookup"><span data-stu-id="201b5-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="201b5-103">Proszę sprawdzić folder wiadomości-śmieci w wiadomości e-mail, ponieważ czasami alerty mogą tam iść.</span><span class="sxs-lookup"><span data-stu-id="201b5-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="201b5-104">Określić, czy **wszystkie alerty nie są dostarczane** lub jeśli **pojedynczy alert** z określonego pliku lub biblioteki nie jest dostarczany.</span><span class="sxs-lookup"><span data-stu-id="201b5-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="201b5-105">**Poszczególne alerty nie są dostarczane**: Jeśli pojedynczy alert z określonego pliku lub biblioteki nie zostanie dostarczony, można spróbować usunąć i odtworzyć go.</span><span class="sxs-lookup"><span data-stu-id="201b5-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="201b5-106">Zobacz [Zarządzanie, wyświetlanie lub usuwanie alertów programu SharePoint,](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=&ad=US#ID0EAADAAA=Online) aby odtworzyć alert.</span><span class="sxs-lookup"><span data-stu-id="201b5-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=&ad=US#ID0EAADAAA=Online) to recreate the alert.</span></span>
- <span data-ttu-id="201b5-107">**Wszystkie alerty nie są dostarczane**: Jeśli wszystkie alerty z wielu plików lub bibliotek nie są dostarczane, odwiedź [pulpit nawigacyjny kondycji usługi](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , aby sprawdzić, czy nie ma żadnych porad/incydentów, które mogą występować w programie SharePoint lub Exchange.</span><span class="sxs-lookup"><span data-stu-id="201b5-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="201b5-108">Problem może być z funkcji alertu programu SharePoint lub opóźnienia w wiadomościach e-mail za pośrednictwem programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="201b5-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="201b5-109">Ważne będzie również, aby pamiętać, czy inne wiadomości e-mail są dostarczane, a jeśli nie, problem jest prawdopodobne z opóźnień Exchange.</span><span class="sxs-lookup"><span data-stu-id="201b5-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="201b5-110">FAQ na temat alertów:</span><span class="sxs-lookup"><span data-stu-id="201b5-110">FAQ on alerts:</span></span>

- <span data-ttu-id="201b5-111">Nie jest możliwe wysyłanie alertów do grupy dystrybucyjnej, obsługiwane są tylko grupy zabezpieczeń i 365.</span><span class="sxs-lookup"><span data-stu-id="201b5-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="201b5-112">Nie można dostosować szablony wiadomości e-mail alertu; należy użyć przepływu pracy programu Microsoft FLOW lub SharePoint Designer do osiągnięcia tych.</span><span class="sxs-lookup"><span data-stu-id="201b5-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

<span data-ttu-id="201b5-113">Więcej informacji:</span><span class="sxs-lookup"><span data-stu-id="201b5-113">More Information:</span></span>

- <span data-ttu-id="201b5-114">**Ustawienia alertów**: Aby uzyskać więcej informacji na temat konfigurowania alertów, zobacz [Tworzenie alertu, aby otrzymywać powiadomienia, gdy plik lub folder zmieni się w programie SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span><span class="sxs-lookup"><span data-stu-id="201b5-114">**Alert setup**: For more information about setting up alerts, see [Create an alert to get notified when a file or folder changes in SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span></span>
- <span data-ttu-id="201b5-115">**Rozwiązywanie problemów z alertami**: Aby uzyskać więcej informacji na temat rozwiązywania problemów z alertami, zobacz [Użytkownicy nie otrzymują powiadomienia alertów online programu SharePoint](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span><span class="sxs-lookup"><span data-stu-id="201b5-115">**Troubleshoot alerts**: For more information about troubleshooting alerts, see [Users don't receive SharePoint Online alert notifications](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span></span>
- <span data-ttu-id="201b5-116">**Zaawansowane zasady alertów zgodności**z programem 365: Aby uzyskać więcej informacji na temat konfigurowania tych alertów, zobacz [zasady alertów zgodności](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="201b5-116">**Advanced O365 Compliance Alert Policies**: For more information about setting up these alerts, see [Compliance Alert Policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>
- <span data-ttu-id="201b5-117">**Dzienniki inspekcji programu SharePoint i OneDrive**: Aby uzyskać więcej informacji dotyczących sposobu pobierania tych zdarzeń, zobacz [przeszukiwanie dziennika inspekcji](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="201b5-117">**SharePoint and OneDrive Audit Logs**: For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
- <span data-ttu-id="201b5-118">**Alerty wysyłane przez zaawansowaną ochronę przed zagrożeniami**: zobacz [ATP dla programu SharePoint i OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="201b5-118">**Alerts sent by Advanced Threat Protection**: See [ATP for SharePoint and OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
- <span data-ttu-id="201b5-119">**Alerty wysyłane przez zasady zapobiegania utracie danych**: zobacz [powiadomienia E-mail dotyczące zasad DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="201b5-119">**Alerts sent by Data Loss Prevention polices**: See [Email notifications for DLP policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

## <a name="related-topics"></a><span data-ttu-id="201b5-120">Tematy pokrewne</span><span class="sxs-lookup"><span data-stu-id="201b5-120">Related Topics</span></span>

<span data-ttu-id="201b5-121">Chcesz wypróbować usługi Microsoft Flow w usłudze SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="201b5-121">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="201b5-122">Utwórz przepływ</span><span class="sxs-lookup"><span data-stu-id="201b5-122">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="201b5-123">SharePoint i przepływu</span><span class="sxs-lookup"><span data-stu-id="201b5-123">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
