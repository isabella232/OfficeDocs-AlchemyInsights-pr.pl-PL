---
title: Outlook Desktop przywoływanie lub zastępowanie wiadomości e-mail
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36496121"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="eab0f-102">Odwoływanie lub zastępowanie wiadomości e-mail programu Outlook</span><span class="sxs-lookup"><span data-stu-id="eab0f-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="eab0f-103">Jako administrator można **przywołać wiadomości w imieniu użytkowników przy użyciu programu PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="eab0f-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="eab0f-104">Nie można przywoływać wiadomości z centrum administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="eab0f-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="eab0f-105">Można **przywoływać tylko te wiadomości, które są wysyłane do osób w organizacji**.</span><span class="sxs-lookup"><span data-stu-id="eab0f-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="eab0f-106">Jeśli wiadomość została wysłana na adres Gmail, na przykład nie możesz jej przypomnieć.</span><span class="sxs-lookup"><span data-stu-id="eab0f-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="eab0f-107">**Wiadomości wysłane z programu Outlook 2016 można przywoływać tylko na komputerze**.</span><span class="sxs-lookup"><span data-stu-id="eab0f-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="eab0f-108">Jeśli użytkownik wyśle wiadomość za pomocą programu Outlook dla komputerów Macintosh lub Outlook w sieci Web, nie można go przypomnieć.</span><span class="sxs-lookup"><span data-stu-id="eab0f-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="eab0f-109">Aby przywołać lub zamienić wiadomość e-mail:</span><span class="sxs-lookup"><span data-stu-id="eab0f-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="eab0f-110">W okienku folderów po lewej stronie okna programu Outlook wybierz folder Elementy wysłane.</span><span class="sxs-lookup"><span data-stu-id="eab0f-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="eab0f-111">Kliknij dwukrotnie wiadomość, którą chcesz przypomnieć, aby ją otworzyć.</span><span class="sxs-lookup"><span data-stu-id="eab0f-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="eab0f-112">Wybierz kartę **wiadomość** , a następnie wybierz **Akcje** > **Przywołaj tę wiadomość**.</span><span class="sxs-lookup"><span data-stu-id="eab0f-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="eab0f-113">Wybierz opcję **Usuń nieprzeczytane kopie tej wiadomości** lub **Usuń nieprzeczytane kopie i Zastąp ją nową wiadomością**, a następnie wybierz **przycisk OK**.</span><span class="sxs-lookup"><span data-stu-id="eab0f-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="eab0f-114">Jeśli wysyłasz wiadomość zastępczą, Skomponuj wiadomość, a następnie wybierz **Wyślij**.</span><span class="sxs-lookup"><span data-stu-id="eab0f-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="eab0f-115">Powodzenie lub niepowodzenie odwołania wiadomości zależy od ustawień adresata w programie Outlook.</span><span class="sxs-lookup"><span data-stu-id="eab0f-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="eab0f-116">Aby uzyskać instrukcje dotyczące sprawdzania wycofywania, zobacz [ten artykuł](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="eab0f-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="eab0f-117">Wyszukiwanie i usuwanie wiadomości e-mail w organizacji</span><span class="sxs-lookup"><span data-stu-id="eab0f-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="eab0f-118">Jeśli nie jesteś administratorem globalnym, Twoje konto musi zostać dodane do roli menedżera zbierania elektronicznych materiałów dowodowych lub roli zarządzania wyszukiwania zgodności w celu wyszukania wiadomości.</span><span class="sxs-lookup"><span data-stu-id="eab0f-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="eab0f-119">Aby usunąć wiadomości, należy przyłączyć się do grupy ról Zarządzanie organizacją lub wyszukiwanie i czyszczenie roli zarządzania.</span><span class="sxs-lookup"><span data-stu-id="eab0f-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="eab0f-120">Uprawnienia dla tych ról są przypisywane w [Centrum zabezpieczeń i zgodności](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="eab0f-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="eab0f-121">[Utwórz Wyszukiwanie zawartości](https://docs.microsoft.com/office365/securitycompliance/content-search) , aby znaleźć wiadomość do usunięcia.</span><span class="sxs-lookup"><span data-stu-id="eab0f-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="eab0f-122">[Połącz się z zabezpieczeniami i centrum zgodności środowiska PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="eab0f-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="eab0f-123">Jeśli korzystasz z uwierzytelniania wieloskładnikowego, zobacz [nawiązywanie połączenia z pakietem Office 365 Security i centrum zgodności środowiska PowerShell przy użyciu uwierzytelniania wieloskładnikowego](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="eab0f-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>