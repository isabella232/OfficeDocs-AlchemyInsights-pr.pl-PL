---
title: Identyfikowanie zdarzeń usuwania wiadomości w dziennikach inspekcji
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508998"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="741a7-102">Dzienniki inspekcji usuniętych wiadomości e-mail</span><span class="sxs-lookup"><span data-stu-id="741a7-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="741a7-103">Począwszy od stycznia 2019 r., firma Microsoft domyślnie włącza rejestrowanie inspekcji skrzynek pocztowych.</span><span class="sxs-lookup"><span data-stu-id="741a7-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="741a7-104">W przeciwnym razie, aby przejrzeć zdarzenia usuwania wiadomości dla określonego użytkownika, należy ręcznie włączyć akcje usuwania do inspekcji.</span><span class="sxs-lookup"><span data-stu-id="741a7-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="741a7-105">Jeśli rejestrowanie inspekcji skrzynki pocztowej jest już włączone dla twojej organizacji lub dla określonego użytkownika, wykonaj poniższe czynności.</span><span class="sxs-lookup"><span data-stu-id="741a7-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="741a7-106">Zaloguj się do [Centrum zgodności & zabezpieczeń usługi Microsoft 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="741a7-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="741a7-107">Kliknij **pozycję Wyszukaj i przeszukuj** i wybierz pozycję **Wyszukiwanie dziennika inspekcji**.</span><span class="sxs-lookup"><span data-stu-id="741a7-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="741a7-108">Wybierz zakres dat w polach **Data rozpoczęcia** i **Data zakończenia.**</span><span class="sxs-lookup"><span data-stu-id="741a7-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="741a7-109">Określ nazwę użytkownika, który chcesz zbadać (użytkownik, który usunął elementy).</span><span class="sxs-lookup"><span data-stu-id="741a7-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="741a7-110">W polu **Działania** wybierz folder **Usunięte wiadomości z folderu Elementy usunięte** i folder **Przeniesiono wiadomości do folderu Elementy usunięte**.</span><span class="sxs-lookup"><span data-stu-id="741a7-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="741a7-111">Kliknij **pozycję Wyszukaj**.</span><span class="sxs-lookup"><span data-stu-id="741a7-111">Click **Search**.</span></span>

<span data-ttu-id="741a7-112">W wynikach wybierz rekord inspekcji.</span><span class="sxs-lookup"><span data-stu-id="741a7-112">In the results, select an audit record.</span></span> <span data-ttu-id="741a7-113">W wysu wysu wysu wysunął szczegóły kliknij pozycję **Więcej informacji**.</span><span class="sxs-lookup"><span data-stu-id="741a7-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="741a7-114">Dodatkowe informacje o usuniętym elemencie (na przykład wiersz tematu i lokalizacja elementu, gdy został usunięty) są wyświetlane w polu **AffectedItems.**</span><span class="sxs-lookup"><span data-stu-id="741a7-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="741a7-115">**Właściwość ClientInfoString** zostanie wyświetlena, jeśli usunięcie nastąpiło w programie Outlook, w programie Outlook w sieci Web (wcześniej znanej jako outlook web app) lub na jakimkolwiek innym urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="741a7-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="741a7-116">Aby uzyskać więcej informacji, zobacz [Określanie, kto skonfigurował przekazywanie poczty e-mail dla skrzynki pocztowej](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="741a7-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="741a7-117">**Uwaga:** Nie można pobrać usuniętych elementów przy użyciu funkcji dziennika inspekcji.</span><span class="sxs-lookup"><span data-stu-id="741a7-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="741a7-118">Aby pobrać usunięte wiadomości w aplikacji Outlook w sieci Web, zobacz [Odzyskiwanie usuniętych elementów w aplikacji Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="741a7-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
