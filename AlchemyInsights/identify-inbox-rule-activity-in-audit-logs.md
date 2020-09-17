---
title: Identyfikator aktywności reguły skrzynki odbiorczej w dziennikach inspekcji
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779061"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="38ae4-102">Identyfikator aktywności reguły skrzynki odbiorczej w dziennikach inspekcji</span><span class="sxs-lookup"><span data-stu-id="38ae4-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="38ae4-103">Aby wyświetlić zdarzenia reguły skrzynki odbiorczej (tworzenie, modyfikowanie i usuwanie reguł skrzynek odbiorczych), można użyć funkcji wyszukiwania dziennika inspekcji w centrum zgodności usługi Microsoft 365 Security &.</span><span class="sxs-lookup"><span data-stu-id="38ae4-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="38ae4-104">Zaloguj się do [Centrum zabezpieczeń & programu Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="38ae4-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="38ae4-105">Przejdź do strony **Search**  >  **wyszukiwania dziennika inspekcji** wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="38ae4-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="38ae4-106">Wybierz zakres dat w polach **Data rozpoczęcia** i **Data zakończenia** .</span><span class="sxs-lookup"><span data-stu-id="38ae4-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="38ae4-107">W obszarze **działania dotyczące skrzynek pocztowych programu Exchange**Sprawdź, czy w polu **działania** jest ustawiona wartość **Nowy — InboxRule tworzenie/modyfikowanie/Włączanie/wyłączanie reguły skrzynki odbiorczej**.</span><span class="sxs-lookup"><span data-stu-id="38ae4-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="38ae4-108">Kliknij przycisk **Wyszukaj**.</span><span class="sxs-lookup"><span data-stu-id="38ae4-108">Click **Search**.</span></span>

<span data-ttu-id="38ae4-109">W wynikach wybierz rekord inspekcji.</span><span class="sxs-lookup"><span data-stu-id="38ae4-109">In the results, select an audit record.</span></span> <span data-ttu-id="38ae4-110">W menu wysuwanym Szczegóły kliknij pozycję **więcej informacji**.</span><span class="sxs-lookup"><span data-stu-id="38ae4-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="38ae4-111">Informacje na temat ustawień reguły skrzynki odbiorczej są wyświetlane w polu **Parametry** .</span><span class="sxs-lookup"><span data-stu-id="38ae4-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="38ae4-112">Aby uzyskać więcej informacji, zobacz [Określanie, czy użytkownik utworzył regułę skrzynki odbiorczej](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="38ae4-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
