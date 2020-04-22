---
title: Identyfikowanie aktywności reguły skrzynki odbiorczej w dziennikach inspekcji
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716434"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="c5493-102">Identyfikowanie aktywności reguły skrzynki odbiorczej w dziennikach inspekcji</span><span class="sxs-lookup"><span data-stu-id="c5493-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="c5493-103">Wyszukiwanie dzienników inspekcji można użyć w Centrum zgodności zabezpieczeń & microsoft 365, aby wyświetlić zdarzenia reguł skrzynki odbiorczej (tworzenie, modyfikowanie i usuwanie reguł skrzynki odbiorczej).</span><span class="sxs-lookup"><span data-stu-id="c5493-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="c5493-104">Zaloguj się do [Centrum zgodności & zabezpieczeń usługi Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="c5493-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="c5493-105">Przejdź do strony**wyszukiwania dziennika inspekcji** **wyszukiwania.** > </span><span class="sxs-lookup"><span data-stu-id="c5493-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="c5493-106">Wybierz zakres dat w polach **Data rozpoczęcia** i **Data zakończenia.**</span><span class="sxs-lookup"><span data-stu-id="c5493-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="c5493-107">W obszarze **Działania skrzynki pocztowej programu Exchange**sprawdź, czy pole **Działania** jest ustawione na **Reguła Nowa skrzynka odbiorcza Utwórz/modyfikuj/włącz/wyłącz regułę skrzynki odbiorczej**.</span><span class="sxs-lookup"><span data-stu-id="c5493-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="c5493-108">Kliknij **pozycję Wyszukaj**.</span><span class="sxs-lookup"><span data-stu-id="c5493-108">Click **Search**.</span></span>

<span data-ttu-id="c5493-109">W wynikach wybierz rekord inspekcji.</span><span class="sxs-lookup"><span data-stu-id="c5493-109">In the results, select an audit record.</span></span> <span data-ttu-id="c5493-110">W wysu wysu wysu wysunął szczegóły kliknij pozycję **Więcej informacji**.</span><span class="sxs-lookup"><span data-stu-id="c5493-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="c5493-111">Informacje o ustawieniach reguły skrzynki odbiorczej są wyświetlane w polu **Parametry.**</span><span class="sxs-lookup"><span data-stu-id="c5493-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="c5493-112">Aby uzyskać więcej informacji, zobacz [Określanie, czy użytkownik utworzył regułę skrzynki odbiorczej](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="c5493-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
