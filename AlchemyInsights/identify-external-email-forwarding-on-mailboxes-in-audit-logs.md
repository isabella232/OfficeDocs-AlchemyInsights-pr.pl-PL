---
title: Identyfikowanie przekazywanie poczty zewnętrznej skrzynek pocztowych w dziennikach inspekcji
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539111"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="69d3e-102">Określenie, jeśli skonfigurowano przesyłanie dalej poczty e-mail zewnętrznej skrzynek pocztowych</span><span class="sxs-lookup"><span data-stu-id="69d3e-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="69d3e-103">Gdy użytkownika w usłudze Office 365 konfiguruje przekazywania zewnętrznych wiadomości e-mail w skrzynce pocztowej, działania jest różna w ramach apletu polecenia **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="69d3e-103">When an Office 365  user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="69d3e-104">Możesz zobaczyć działanie przy użyciu przeszukiwania dzienników inspekcji w & zabezpieczeń Centrum zgodności.</span><span class="sxs-lookup"><span data-stu-id="69d3e-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="69d3e-105">Zaloguj się do [Centrum zgodności Office 365 zabezpieczeń &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="69d3e-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="69d3e-106">Przejdź do **wyszukiwania** > stronę**przeszukiwania dzienników inspekcji** .</span><span class="sxs-lookup"><span data-stu-id="69d3e-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="69d3e-107">Wybierz zakres dat w polach **Data początkowa** i **Data końcowa** .</span><span class="sxs-lookup"><span data-stu-id="69d3e-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="69d3e-108">Nie musisz podać nazwę użytkownika.</span><span class="sxs-lookup"><span data-stu-id="69d3e-108">You don't need to specify a username.</span></span> <span data-ttu-id="69d3e-109">Sprawdź, czy pole **działalności** jest włączona opcja **Pokaż wyniki dla wszystkich działań**.</span><span class="sxs-lookup"><span data-stu-id="69d3e-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="69d3e-110">Kliknij przycisk **Wyszukaj**.</span><span class="sxs-lookup"><span data-stu-id="69d3e-110">Click **Search**.</span></span>

<span data-ttu-id="69d3e-111">W wynikach kliknij przycisk **Filtruj wyniki** i wpisz **Set-Mailbox** w polu Filtr aktywności.</span><span class="sxs-lookup"><span data-stu-id="69d3e-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="69d3e-112">Wybierz rekord audytu w wynikach.</span><span class="sxs-lookup"><span data-stu-id="69d3e-112">Select an audit record in the results.</span></span> <span data-ttu-id="69d3e-113">W menu wysuwane **Szczegóły** kliknij przycisk **więcej informacji**.</span><span class="sxs-lookup"><span data-stu-id="69d3e-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="69d3e-114">Należy spojrzeć na szczegóły poszczególnych rekordów inspekcji w celu określenia, jeśli działanie jest powiązane z przekazywanie wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="69d3e-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="69d3e-115">**Identyfikator obiektu**: wartość alias skrzynki pocztowej, który został zmodyfikowany.</span><span class="sxs-lookup"><span data-stu-id="69d3e-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="69d3e-116">**Parametry**: _ForwardingSmtpAddress_ wskazuje docelowy adres e-mail.</span><span class="sxs-lookup"><span data-stu-id="69d3e-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="69d3e-117">**Identyfikator użytkownika**: użytkownik, który skonfigurować przekazywanie poczty e-mail do skrzynki pocztowej w polu **identyfikator obiektu** .</span><span class="sxs-lookup"><span data-stu-id="69d3e-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="69d3e-118">Aby uzyskać więcej informacji zobacz [Określanie, która skonfigurowała przekazywanie dla skrzynki pocztowej wiadomości e-mail](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="69d3e-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
