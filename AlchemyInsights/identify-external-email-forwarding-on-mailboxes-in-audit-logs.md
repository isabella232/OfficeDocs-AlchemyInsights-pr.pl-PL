---
title: Identyfikowanie zewnętrznego przekazywania wiadomości e-mail w skrzynkach pocztowych w dziennikach inspekcji
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716470"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="87acd-102">Identyfikowanie, kiedy zewnętrzna przekazywanie poczty e-mail jest skonfigurowane w skrzynkach pocztowych</span><span class="sxs-lookup"><span data-stu-id="87acd-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="87acd-103">Gdy użytkownik usługi Microsoft 365 konfiguruje zewnętrzne przekazywanie wiadomości e-mail w skrzynce pocztowej, działanie jest poddane inspekcji w ramach polecenia cmdlet **Set-Mailbox.**</span><span class="sxs-lookup"><span data-stu-id="87acd-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="87acd-104">Działanie można zobaczyć przy użyciu wyszukiwania dziennika inspekcji w Centrum zgodności & zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="87acd-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="87acd-105">Zaloguj się do [Centrum zgodności & zabezpieczeń usługi Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="87acd-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="87acd-106">Przejdź do strony**wyszukiwania dziennika inspekcji** **wyszukiwania.** > </span><span class="sxs-lookup"><span data-stu-id="87acd-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="87acd-107">Wybierz zakres dat w polach **Data rozpoczęcia** i **Data zakończenia.**</span><span class="sxs-lookup"><span data-stu-id="87acd-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="87acd-108">Nie musisz podawać nazwy użytkownika.</span><span class="sxs-lookup"><span data-stu-id="87acd-108">You don't need to specify a username.</span></span> <span data-ttu-id="87acd-109">Sprawdź, czy pole **Działania** jest ustawione **na Pokaż wyniki dla wszystkich działań**.</span><span class="sxs-lookup"><span data-stu-id="87acd-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="87acd-110">Kliknij **pozycję Wyszukaj**.</span><span class="sxs-lookup"><span data-stu-id="87acd-110">Click **Search**.</span></span>

<span data-ttu-id="87acd-111">W wynikach kliknij pozycję **Filtruj wyniki** i wpisz **ustaw skrzynkę pocztową** w polu filtru aktywności.</span><span class="sxs-lookup"><span data-stu-id="87acd-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="87acd-112">Wybierz rekord inspekcji w wynikach.</span><span class="sxs-lookup"><span data-stu-id="87acd-112">Select an audit record in the results.</span></span> <span data-ttu-id="87acd-113">W wysu **nakreślenia szczegółów** kliknij pozycję **Więcej informacji**.</span><span class="sxs-lookup"><span data-stu-id="87acd-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="87acd-114">Musisz spojrzeć na szczegóły każdego rekordu inspekcji, aby ustalić, czy działanie jest związane z przekazywaniem wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="87acd-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="87acd-115">**ObjectId**: Wartość aliasu zmodyfikowanej skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="87acd-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="87acd-116">**Parametry**: _ForwardingSmtpAddress_ wskazuje docelowy adres e-mail.</span><span class="sxs-lookup"><span data-stu-id="87acd-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="87acd-117">**Identyfikator użytkownika:** Użytkownik, który skonfigurował przekazywanie wiadomości e-mail w skrzynce pocztowej w polu **ObjectId.**</span><span class="sxs-lookup"><span data-stu-id="87acd-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="87acd-118">Aby uzyskać więcej informacji, zobacz [Określanie, kto skonfigurował przekazywanie poczty e-mail dla skrzynki pocztowej](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="87acd-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
