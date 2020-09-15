---
title: Identyfikowanie zewnętrznych przekierowywania wiadomości e-mail dotyczących skrzynek pocztowych w dziennikach inspekcji
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696307"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="1f9d3-102">Określanie, czy w skrzynkach pocztowych jest skonfigurowana zewnętrzna przekierowywanie poczty e-mail</span><span class="sxs-lookup"><span data-stu-id="1f9d3-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="1f9d3-103">Gdy użytkownik programu Microsoft 365 skonfiguruje zewnętrzną przekierowywanie poczty e-mail w skrzynce pocztowej, działanie jest poddawane inspekcji w ramach polecenia cmdlet **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="1f9d3-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="1f9d3-104">Działanie można wyświetlić przy użyciu funkcji wyszukiwania dziennika inspekcji w centrum zabezpieczeń & zgodności.</span><span class="sxs-lookup"><span data-stu-id="1f9d3-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="1f9d3-105">Zaloguj się do [Centrum zabezpieczeń & programu Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="1f9d3-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="1f9d3-106">Przejdź do strony **Search**  >  **wyszukiwania dziennika inspekcji** wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="1f9d3-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="1f9d3-107">Wybierz zakres dat w polach **Data rozpoczęcia** i **Data zakończenia** .</span><span class="sxs-lookup"><span data-stu-id="1f9d3-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="1f9d3-108">Nie musisz określać nazwy użytkownika.</span><span class="sxs-lookup"><span data-stu-id="1f9d3-108">You don't need to specify a username.</span></span> <span data-ttu-id="1f9d3-109">Upewnij się, że w polu **działania** jest ustawiona wartość **Pokaż wyniki dla wszystkich działań**.</span><span class="sxs-lookup"><span data-stu-id="1f9d3-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="1f9d3-110">Kliknij przycisk **Wyszukaj**.</span><span class="sxs-lookup"><span data-stu-id="1f9d3-110">Click **Search**.</span></span>

<span data-ttu-id="1f9d3-111">W wynikach kliknij pozycję **Filtruj wyniki** i wpisz wpis **Set-Skrzynka pocztowa** w polu Filtr aktywności.</span><span class="sxs-lookup"><span data-stu-id="1f9d3-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="1f9d3-112">Wybierz rekord inspekcji w wynikach.</span><span class="sxs-lookup"><span data-stu-id="1f9d3-112">Select an audit record in the results.</span></span> <span data-ttu-id="1f9d3-113">W menu wysuwanym **szczegóły** kliknij pozycję **więcej informacji**.</span><span class="sxs-lookup"><span data-stu-id="1f9d3-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="1f9d3-114">Aby określić, czy działanie jest powiązane z przesyłaniem wiadomości e-mail, należy przejrzeć szczegóły każdego rekordu inspekcji.</span><span class="sxs-lookup"><span data-stu-id="1f9d3-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="1f9d3-115">**Objectid**: wartość aliasu skrzynki pocztowej, która została zmodyfikowana.</span><span class="sxs-lookup"><span data-stu-id="1f9d3-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="1f9d3-116">**Parametry**: _ForwardingSmtpAddress_ wskazuje docelowy adres e-mail.</span><span class="sxs-lookup"><span data-stu-id="1f9d3-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="1f9d3-117">**UserID**: użytkownik, który skonfigurował przesyłanie dalej wiadomości e-mail w skrzynce pocztowej w polu **objectid** .</span><span class="sxs-lookup"><span data-stu-id="1f9d3-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="1f9d3-118">Aby uzyskać więcej informacji, zobacz [Określanie, kto konfiguruje przekierowywanie poczty e-mail dla skrzynki pocztowej](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="1f9d3-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
