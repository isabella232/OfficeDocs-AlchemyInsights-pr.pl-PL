---
title: Odwołanie w programie Outlook pulpitu lub zamienianie wiadomości e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496121"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="1c1ff-102">Odwoływanie lub zamienianie wiadomości e-mail programu Outlook</span><span class="sxs-lookup"><span data-stu-id="1c1ff-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="1c1ff-103">Jako administrator możesz **odwoływania wiadomości w imieniu użytkowników przy użyciu programu PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="1c1ff-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="1c1ff-104">Nie można odwołać wiadomości z Centrum administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="1c1ff-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="1c1ff-105">Możesz **tylko odwoływania wiadomości, które są wysyłane do osoby w organizacji**.</span><span class="sxs-lookup"><span data-stu-id="1c1ff-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="1c1ff-106">Jeśli wiadomość została wysłana na adres Gmail, na przykład, nie można wywołać ją.</span><span class="sxs-lookup"><span data-stu-id="1c1ff-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="1c1ff-107">Możesz **tylko odwoływania wiadomości wysłane z Outlook 2016 na komputerze PC**.</span><span class="sxs-lookup"><span data-stu-id="1c1ff-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="1c1ff-108">Jeśli użytkownik wysyła wiadomości za pomocą programu Outlook w sieci web lub programu Outlook dla komputerów Macintosh, nie może je wycofać.</span><span class="sxs-lookup"><span data-stu-id="1c1ff-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="1c1ff-109">Aby odwołać lub zastąpić wiadomość e-mail:</span><span class="sxs-lookup"><span data-stu-id="1c1ff-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="1c1ff-110">W okienku folderów po lewej stronie okna programu Outlook zaznacz folder Elementy wysłane.</span><span class="sxs-lookup"><span data-stu-id="1c1ff-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="1c1ff-111">Kliknij dwukrotnie wiadomość, którą chcesz odwołać go otworzyć.</span><span class="sxs-lookup"><span data-stu-id="1c1ff-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="1c1ff-112">Wybierz kartę **wiadomość** , a następnie wybierz **Akcje** > **Odwołaj tę wiadomość**.</span><span class="sxs-lookup"><span data-stu-id="1c1ff-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="1c1ff-113">Wybierz **usunąć nieprzeczytane kopie tej wiadomości** lub **usunąć nieprzeczytane kopie i zastąpić je nową wiadomością**, a następnie wybierz przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="1c1ff-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="1c1ff-114">Jeśli wysyłasz wiadomość wymiany redagowania wiadomości, a następnie zaznacz pole wyboru **Wyślij**.</span><span class="sxs-lookup"><span data-stu-id="1c1ff-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="1c1ff-115">Powodzenie lub niepowodzenie odwołania wiadomości zależy od ustawień odbiorcy w programie Outlook.</span><span class="sxs-lookup"><span data-stu-id="1c1ff-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="1c1ff-116">Aby sprawdzić na przypomnienie, w [tym](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)artykule czynności.</span><span class="sxs-lookup"><span data-stu-id="1c1ff-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="1c1ff-117">Wyszukiwanie i usuwanie wiadomości e-mail w organizacji</span><span class="sxs-lookup"><span data-stu-id="1c1ff-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="1c1ff-118">Jeśli nie jesteś administratorem globalnym, Twoje konto musi dodane do roli Menedżer zbierania elektronicznych materiałów dowodowych lub Rola zarządzania zgodności wyszukiwania do wyszukiwania wiadomości.</span><span class="sxs-lookup"><span data-stu-id="1c1ff-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="1c1ff-119">Aby usunąć wiadomości, będziesz musiał przyłączyć się do grupy ról Zarządzanie organizacją lub Rola zarządzania wyszukiwania i czyszczenie.</span><span class="sxs-lookup"><span data-stu-id="1c1ff-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="1c1ff-120">W [Centrum zabezpieczeń i zgodności](https://go.microsoft.com/fwlink/?linkid=2083731)są przypisane uprawnienia dla tych ról.</span><span class="sxs-lookup"><span data-stu-id="1c1ff-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="1c1ff-121">[Tworzenie zawartości wyszukiwania](https://docs.microsoft.com/office365/securitycompliance/content-search) , aby odnaleźć wiadomości do usunięcia.</span><span class="sxs-lookup"><span data-stu-id="1c1ff-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="1c1ff-122">[Podłącz do bezpieczeństwa i środowiska PowerShell Centrum zgodności](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="1c1ff-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="1c1ff-123">Jeśli używasz wieloczynnikowe uwierzytelnianie Zobacz [Łączenie z zabezpieczeń usługi Office 365 oraz środowiska PowerShell Centrum zgodności za pomocą wieloczynnikowe uwierzytelnianie](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="1c1ff-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>