---
title: Odwoływanie lub zamienianie wiadomości e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353516"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="166c7-102">Odwoływanie lub zamienianie wiadomości e-mail w programie Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="166c7-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="166c7-103">Możesz **odwołać tylko wiadomości wysłane do osób w organizacji**.</span><span class="sxs-lookup"><span data-stu-id="166c7-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="166c7-104">Jeśli na przykład wiadomość została wysłana na adres Gmail, nie można jej odwołać.</span><span class="sxs-lookup"><span data-stu-id="166c7-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="166c7-105">Możesz **odwołać tylko wiadomości wysyłane z programu Outlook dla komputerów PC**.</span><span class="sxs-lookup"><span data-stu-id="166c7-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="166c7-106">Jeśli użytkownik wyśle wiadomość za pomocą programu Outlook dla komputerów Mac lub aplikacji Outlook w sieci Web, nie można jej odwołać.</span><span class="sxs-lookup"><span data-stu-id="166c7-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="166c7-107">Jako Administrator dzierżawy możesz **odwołać wiadomości w imieniu użytkowników za pomocą programu PowerShell** (Aby uzyskać więcej informacji, zobacz: [Wyszukiwanie i usuwanie wiadomości e-mail](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="166c7-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="166c7-108">Nie można odwołać wiadomości z centrum administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="166c7-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="166c7-109">Aby uzyskać więcej informacji, przewiń w dół do listy "wyszukiwanie i usuwanie wiadomości e-mail w organizacji".</span><span class="sxs-lookup"><span data-stu-id="166c7-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="166c7-110">**Odwoływanie lub zamienianie wysłanej wiadomości e-mail**</span><span class="sxs-lookup"><span data-stu-id="166c7-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="166c7-111">W okienku folderów po lewej stronie okna programu Outlook wybierz folder Elementy wysłane.</span><span class="sxs-lookup"><span data-stu-id="166c7-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="166c7-112">Otwórz wiadomość, którą chcesz odwołać.</span><span class="sxs-lookup"><span data-stu-id="166c7-112">Open the message that you want to recall.</span></span> <span data-ttu-id="166c7-113">Musisz kliknąć dwukrotnie, aby otworzyć wiadomość.</span><span class="sxs-lookup"><span data-stu-id="166c7-113">You must double-click to open the message.</span></span> <span data-ttu-id="166c7-114">Wybranie wiadomości w celu wyświetlenia jej w okienku odczytu nie pozwala na odwołanie wiadomości.</span><span class="sxs-lookup"><span data-stu-id="166c7-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="166c7-115">Na karcie wiadomość wybierz pozycję **Akcje**  >  **odwołaj tę wiadomość**.</span><span class="sxs-lookup"><span data-stu-id="166c7-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="166c7-116">Wybierz pozycję **Usuń nieprzeczytane kopie tej wiadomości** lub **Usuń nieprzeczytane kopie i zastąp je nową wiadomością**, a następnie wybierz **przycisk OK**.</span><span class="sxs-lookup"><span data-stu-id="166c7-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="166c7-117">Jeśli wysyłasz wiadomość zastępującą, Zredaguj wiadomość, a następnie wybierz pozycję **Wyślij**.</span><span class="sxs-lookup"><span data-stu-id="166c7-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="166c7-118">Sukces lub niepowodzenie odwołania wiadomości zależy od ustawień adresatów w programie Outlook.</span><span class="sxs-lookup"><span data-stu-id="166c7-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="166c7-119">Aby uzyskać więcej informacji, w tym sposób sprawdzania odwołania, zobacz [odwoływanie lub zamienianie wysłanej wiadomości e-mail](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="166c7-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="166c7-120">**_Wyszukiwanie i usuwanie wiadomości e-mail w organizacji_** jest najłatwiej, jeśli jesteś administratorem globalnym. Jeśli nie jesteś administratorem globalnym, konto należy dodać do grupy ról Menedżer zbierania elektronicznych materiałów dowodowych lub do roli zarządzania wyszukiwaniem zgodności.</span><span class="sxs-lookup"><span data-stu-id="166c7-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="166c7-121">Aby usunąć wiadomości, musisz przyłączyć się do grupy ról zarządzania organizacją lub wyszukiwania i usuwania.</span><span class="sxs-lookup"><span data-stu-id="166c7-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="166c7-122">Uprawnienia do tych ról są przypisywane w [Centrum zabezpieczeń & zgodności](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="166c7-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="166c7-123">[Utwórz Wyszukiwanie zawartości](https://docs.microsoft.com/microsoft-365/compliance/content-search) , aby znaleźć wiadomość, którą chcesz usunąć.</span><span class="sxs-lookup"><span data-stu-id="166c7-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="166c7-124">[Nawiązywanie połączenia z programem PowerShell w centrum zgodności & zabezpieczeniami](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="166c7-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="166c7-125">Jeśli korzystasz z uwierzytelniania wieloskładnikowe (Multi-Factor Authentication), zobacz [nawiązywanie połączenia z programem Microsoft 365 Security & Centrum zgodności programu PowerShell przy użyciu uwierzytelniania wieloskładnikowego](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="166c7-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
