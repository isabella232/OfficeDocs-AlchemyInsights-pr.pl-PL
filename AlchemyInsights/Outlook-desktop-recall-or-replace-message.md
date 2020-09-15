---
title: Program Outlook Desktop odwoływanie lub zamienianie wiadomości e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664000"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="8fb00-102">Odwoływanie lub zamienianie wiadomości e-mail programu Outlook</span><span class="sxs-lookup"><span data-stu-id="8fb00-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="8fb00-103">Jako administrator możesz **odwołać wiadomości w imieniu użytkowników przy użyciu programu PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="8fb00-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="8fb00-104">Nie można odwołać wiadomości z centrum administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="8fb00-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="8fb00-105">Możesz **odwołać tylko wiadomości wysłane do osób w organizacji**.</span><span class="sxs-lookup"><span data-stu-id="8fb00-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="8fb00-106">Jeśli wiadomość została wysłana na adres Gmail, na przykład nie można jej odwołać.</span><span class="sxs-lookup"><span data-stu-id="8fb00-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="8fb00-107">**Wiadomości wysłane z programu Outlook 2016 można odwołać tylko na komputerze PC**.</span><span class="sxs-lookup"><span data-stu-id="8fb00-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="8fb00-108">Jeśli użytkownik wyśle wiadomość za pomocą programu Outlook dla komputerów Mac lub aplikacji Outlook w sieci Web, nie można jej odwołać.</span><span class="sxs-lookup"><span data-stu-id="8fb00-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="8fb00-109">Aby odwołać lub zamienić wiadomość e-mail:</span><span class="sxs-lookup"><span data-stu-id="8fb00-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="8fb00-110">W okienku folderów po lewej stronie okna programu Outlook wybierz folder Elementy wysłane.</span><span class="sxs-lookup"><span data-stu-id="8fb00-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="8fb00-111">Kliknij dwukrotnie wiadomość, którą chcesz odwołać, aby ją otworzyć.</span><span class="sxs-lookup"><span data-stu-id="8fb00-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="8fb00-112">Wybierz kartę **wiadomość** , a następnie wybierz pozycję **Akcje**  >  **odwołaj tę wiadomość**.</span><span class="sxs-lookup"><span data-stu-id="8fb00-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="8fb00-113">Wybierz pozycję **Usuń nieprzeczytane kopie tej wiadomości** lub **Usuń nieprzeczytane kopie i zastąp je nową wiadomością**, a następnie wybierz przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="8fb00-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="8fb00-114">Jeśli wysyłasz wiadomość zastępującą, Zredaguj wiadomość, a następnie wybierz pozycję **Wyślij**.</span><span class="sxs-lookup"><span data-stu-id="8fb00-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="8fb00-115">Sukces lub niepowodzenie odwołania wiadomości zależy od ustawień adresata w programie Outlook.</span><span class="sxs-lookup"><span data-stu-id="8fb00-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="8fb00-116">Procedurę sprawdzania odwołania można znaleźć w [artykule](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="8fb00-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="8fb00-117">Wyszukiwanie i usuwanie wiadomości e-mail w organizacji</span><span class="sxs-lookup"><span data-stu-id="8fb00-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="8fb00-118">Jeśli nie jesteś administratorem globalnym, konto musi zostać dodane do roli menedżera zbierania elektronicznych materiałów dowodowych lub roli zarządzania wyszukiwaniem zgodności w celu wyszukania wiadomości.</span><span class="sxs-lookup"><span data-stu-id="8fb00-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="8fb00-119">Aby usunąć wiadomości, musisz przyłączyć się do grupy ról zarządzania organizacją lub wyszukiwania i usuwania.</span><span class="sxs-lookup"><span data-stu-id="8fb00-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="8fb00-120">Uprawnienia do tych ról są przypisywane w [Centrum zabezpieczeń i zgodności](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="8fb00-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="8fb00-121">[Utwórz Wyszukiwanie zawartości](https://docs.microsoft.com/microsoft-365/compliance/content-search) , aby znaleźć wiadomość, którą chcesz usunąć.</span><span class="sxs-lookup"><span data-stu-id="8fb00-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="8fb00-122">[Nawiązywanie połączenia z programem PowerShell w centrum zabezpieczeń i zgodności](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="8fb00-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="8fb00-123">Jeśli korzystasz z uwierzytelniania wieloskładnikowego, zobacz [nawiązywanie połączenia z programem Microsoft 365 Security and zgodna Center za pomocą uwierzytelniania wieloskładnikowego](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="8fb00-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>