---
title: Stuck in Skrzynka nadawcza z powodu dużych załączników
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441315"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="9d4b9-102">Naprawianie wiadomości, które są zablokowane w skrzynce nadawcza</span><span class="sxs-lookup"><span data-stu-id="9d4b9-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="9d4b9-103">Zaleca się rozpoczęcie od uruchomienia scenariusza ["Mam problemy z wysyłaniem, odbieraniem lub znajdowaniu wiadomości e-mail"](https://aka.ms/SaRA-OutlookSendReceive) w narzędziu [Pomoc techniczna i Asystent odzyskiwania firmy Microsoft](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="9d4b9-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="9d4b9-104">Gdy wiadomość zostaje zablokowana w skrzynce nadawcza, najbardziej prawdopodobną przyczyną są:</span><span class="sxs-lookup"><span data-stu-id="9d4b9-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="9d4b9-105">Duże załączniki.</span><span class="sxs-lookup"><span data-stu-id="9d4b9-105">Large attachments.</span></span>
- <span data-ttu-id="9d4b9-106">Opcja **Wyślij natychmiast po podłączeniu** nie jest włączona.</span><span class="sxs-lookup"><span data-stu-id="9d4b9-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="9d4b9-107">Aby usunąć duże załączniki:</span><span class="sxs-lookup"><span data-stu-id="9d4b9-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="9d4b9-108">W programie Outlook wybierz opcję **Wyślij/Odbierz** > **pracę w trybie offline**.</span><span class="sxs-lookup"><span data-stu-id="9d4b9-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="9d4b9-109">W okienku nawigacji wybierz opcję **Skrzynka nadawcza**.</span><span class="sxs-lookup"><span data-stu-id="9d4b9-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="9d4b9-110">Tutaj możesz:</span><span class="sxs-lookup"><span data-stu-id="9d4b9-110">From here, you can:</span></span> 
    - <span data-ttu-id="9d4b9-111">Usuń wiadomość (zaznacz ją, a następnie wybierz **Usuń**).</span><span class="sxs-lookup"><span data-stu-id="9d4b9-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="9d4b9-112">Przeciągnij wiadomość do folderu wersje robocze, kliknij dwukrotnie, aby ją otworzyć, a następnie Usuń załącznik i wybierz go, a następnie wybierz pozycję **Usuń**).</span><span class="sxs-lookup"><span data-stu-id="9d4b9-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="9d4b9-113">Jeśli zostanie wyświetlony komunikat o błędzie informujący, że program Outlook próbuje przesłać wiadomość, Zamknij program Outlook.</span><span class="sxs-lookup"><span data-stu-id="9d4b9-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="9d4b9-114">Wyjście może zająć kilka chwil.</span><span class="sxs-lookup"><span data-stu-id="9d4b9-114">It may take a few moments to exit.</span></span> <span data-ttu-id="9d4b9-115">Jeśli program Outlook nie zostanie zamknięty, naciśnij kombinację Ctrl + Alt + Delete i wybierz pozycję **Uruchom Menedżera zadań**.</span><span class="sxs-lookup"><span data-stu-id="9d4b9-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="9d4b9-116">W Menedżerze zadań wybierz kartę **procesy** , przewiń w dół do Outlook. exe i wybierz **Zakończ proces**.</span><span class="sxs-lookup"><span data-stu-id="9d4b9-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="9d4b9-117">Po zamknięciu programu Outlook, uruchom go ponownie i powtórz kroki 2 i 3.</span><span class="sxs-lookup"><span data-stu-id="9d4b9-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="9d4b9-118">Po usunięciu załącznika kliknij przycisk **Wyślij/Odbierz** > **pracę w trybie offline** , aby wznowić pracę w trybie online.</span><span class="sxs-lookup"><span data-stu-id="9d4b9-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="9d4b9-119">Wiadomości również utknąć w skrzynce nadawcza po kliknięciu przycisku **Wyślij**, ale nie są podłączone.</span><span class="sxs-lookup"><span data-stu-id="9d4b9-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="9d4b9-120">Kliknij przycisk **Wyślij/Odbierz** i spójrz na przycisk **Pracuj w trybie offline** .</span><span class="sxs-lookup"><span data-stu-id="9d4b9-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="9d4b9-121">Jeśli jest niebieska, zostanie rozłączona.</span><span class="sxs-lookup"><span data-stu-id="9d4b9-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="9d4b9-122">Wybierz go, aby nawiązać połączenie (przycisk zmieni kolor na biały) i kliknij przycisk **Wyślij wszystko**.</span><span class="sxs-lookup"><span data-stu-id="9d4b9-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="9d4b9-123">Aby włączyć funkcję **Wyślij natychmiast po podłączeniu**:</span><span class="sxs-lookup"><span data-stu-id="9d4b9-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="9d4b9-124">Wybierz \*\*\*\* > \*\*\*\* opcje >  pliku**Zaawansowane**.</span><span class="sxs-lookup"><span data-stu-id="9d4b9-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="9d4b9-125">W **wysyłania i odbierania** sekcji, wybierz opcję **Wyślij natychmiast po podłączeniu**, a następnie wybierz **OK**.</span><span class="sxs-lookup"><span data-stu-id="9d4b9-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="9d4b9-126">Aby uzyskać szczegółowe informacje, zobacz:</span><span class="sxs-lookup"><span data-stu-id="9d4b9-126">For full details see:</span></span>
- [<span data-ttu-id="9d4b9-127">Wideo: wysyłanie lub usuwanie zablokowej wiadomości e-mail</span><span class="sxs-lookup"><span data-stu-id="9d4b9-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="9d4b9-128">Wiadomość e-mail pozostaje w folderze Skrzynka nadawcza do momentu ręcznego zainicjowania operacji wysyłania/odbierania w programie Outlook</span><span class="sxs-lookup"><span data-stu-id="9d4b9-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
