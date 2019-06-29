---
title: Identyfikowanie Usuń wiadomość zdarzeń w dziennikach inspekcji
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 89877331d328d798177fab3150d5219c5b484a70
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383143"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="6e594-102">Dzienniki inspekcji dla usunięte wiadomości e-mail</span><span class="sxs-lookup"><span data-stu-id="6e594-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="6e594-103">Począwszy od stycznia 2019, Microsoft jest włączenie rejestrowania domyślnie inspekcji skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="6e594-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="6e594-104">W przeciwnym razie Aby przejrzeć delete komunikat zdarzenia dla określonego użytkownika, należy ręcznie włączyć akcje usuwania w celu prowadzenia inspekcji.</span><span class="sxs-lookup"><span data-stu-id="6e594-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="6e594-105">Jeśli skrzynka pocztowa inspekcji rejestrowanie jest już włączone dla danej organizacji lub dla określonego użytkownika, wykonaj następujące kroki.</span><span class="sxs-lookup"><span data-stu-id="6e594-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="6e594-106">Zaloguj się do [Centrum zgodności Office 365 zabezpieczeń &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="6e594-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="6e594-107">Kliknij przycisk **Wyszukaj i dochodzenia** i wybierz **Przeszukiwania dzienników inspekcji**.</span><span class="sxs-lookup"><span data-stu-id="6e594-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="6e594-108">Wybierz zakres dat w polach **Data początkowa** i **Data końcowa** .</span><span class="sxs-lookup"><span data-stu-id="6e594-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="6e594-109">Umożliwia określenie nazwy użytkownika dla użytkownika, który chcesz zbadać (użytkownik, który elementy usunięte).</span><span class="sxs-lookup"><span data-stu-id="6e594-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="6e594-110">W dziedzinie **działalności** wybierz opcję **usunięte wiadomości z folderu Elementy usunięte** i **wiadomości przenoszonych do folderu Elementy usunięte**.</span><span class="sxs-lookup"><span data-stu-id="6e594-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="6e594-111">Kliknij przycisk **Wyszukaj**.</span><span class="sxs-lookup"><span data-stu-id="6e594-111">Click **Search**.</span></span>

<span data-ttu-id="6e594-112">W wynikach wybierz rekord audytu.</span><span class="sxs-lookup"><span data-stu-id="6e594-112">In the results, select an audit record.</span></span> <span data-ttu-id="6e594-113">W menu wysuwane Szczegóły kliknij przycisk **Więcej informacji**.</span><span class="sxs-lookup"><span data-stu-id="6e594-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="6e594-114">Dodatkowe informacje o usunięty element (na przykład, wiersz tematu i lokalizacji elementu, gdy został usunięty) jest wyświetlana w polu **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="6e594-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="6e594-115">Właściwość **ClientInfoString** pokaże, czy usunięcie pojawił się w programie Outlook, program Outlook w sieci web (dawniej znany jako aplikacji sieci Web programu Outlook) lub inne urządzenie.</span><span class="sxs-lookup"><span data-stu-id="6e594-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="6e594-116">Aby uzyskać więcej informacji zobacz [Określanie, która skonfigurowała przekazywanie dla skrzynki pocztowej wiadomości e-mail](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="6e594-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="6e594-117">**Uwaga**: nie można pobrać elementy usunięte za pomocą funkcji dziennika inspekcji.</span><span class="sxs-lookup"><span data-stu-id="6e594-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="6e594-118">Aby odzyskać usunięte wiadomości w programie Outlook w sieci web, zobacz [Odzyskiwanie usuniętych elementów w programie Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="6e594-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
