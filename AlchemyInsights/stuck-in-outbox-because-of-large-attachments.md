---
title: Utknął w skrzynce nadawczej z powodu dużych załączników
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
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241262"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="6ed2f-102">Naprawianie wiadomości, które utknęły w skrzynce nadawczej</span><span class="sxs-lookup"><span data-stu-id="6ed2f-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="6ed2f-103">Zaleca się rozpoczęcie od uruchomienia scenariusza ["Mam problemy z wysyłaniem, odbieraniem lub znajdowaniem wiadomości e-mail"](https://aka.ms/SaRA-OutlookSendReceive) z narzędzia [Microsoft Support and Recovery Assistant.](https://diagnostics.office.com/#/)</span><span class="sxs-lookup"><span data-stu-id="6ed2f-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="6ed2f-104">Gdy wiadomość utknie w skrzynce nadawczej, najbardziej prawdopodobną przyczyną jest duży załącznik lub opcja "Wyślij natychmiast po podłączeniu" nie jest włączona.</span><span class="sxs-lookup"><span data-stu-id="6ed2f-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="6ed2f-105">**Usuń duży załącznik**</span><span class="sxs-lookup"><span data-stu-id="6ed2f-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="6ed2f-106">W programie Outlook wybierz pozycję **Wyślij / Odbierz** > **pracę w trybie offline**.</span><span class="sxs-lookup"><span data-stu-id="6ed2f-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="6ed2f-107">W okienku nawigacji wybierz pozycję **Skrzynka nadawcza**.</span><span class="sxs-lookup"><span data-stu-id="6ed2f-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="6ed2f-108">W tym miejscu możesz:</span><span class="sxs-lookup"><span data-stu-id="6ed2f-108">From here, you can:</span></span> 
    - <span data-ttu-id="6ed2f-109">Usuń wiadomość (zaznacz ją, a następnie wybierz pozycję **Usuń**).</span><span class="sxs-lookup"><span data-stu-id="6ed2f-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="6ed2f-110">Przeciągnij wiadomość do folderu Wersje robocze, kliknij dwukrotnie, aby ją otworzyć, a następnie usuń zaznacz załącznik, a następnie wybierz pozycję **Usuń**).</span><span class="sxs-lookup"><span data-stu-id="6ed2f-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="6ed2f-111">Jeśli pojawi się błąd informujący, że program Outlook próbuje przesłać wiadomość, zamknij program Outlook.</span><span class="sxs-lookup"><span data-stu-id="6ed2f-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="6ed2f-112">Może upłynąć kilka chwil, aby wyjść.</span><span class="sxs-lookup"><span data-stu-id="6ed2f-112">It may take a few moments to exit.</span></span> <span data-ttu-id="6ed2f-113">Jeśli program Outlook nie zostanie zamknięty, naciśnij klawisze Ctrl+Alt+Delete i wybierz pozycję **Rozpocznij Menedżera zadań**.</span><span class="sxs-lookup"><span data-stu-id="6ed2f-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="6ed2f-114">W Menedżerze zadań wybierz kartę **Procesy,** przewiń w dół do programu outlook.exe i wybierz pozycję **Zakończ proces**.</span><span class="sxs-lookup"><span data-stu-id="6ed2f-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="6ed2f-115">Po zamknięciu programu Outlook uruchom go ponownie i powtórz kroki 2 i 3.</span><span class="sxs-lookup"><span data-stu-id="6ed2f-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="6ed2f-116">Po usunięciu załącznika kliknij przycisk **Wyślij / Odbierz** > **pracę w trybie offline,** aby wznowić pracę w trybie online.</span><span class="sxs-lookup"><span data-stu-id="6ed2f-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="6ed2f-117">Wiadomości utkną również w skrzynce nadawczej po **kliknięciu przycisku Wyślij**, ale nie masz połączenia.</span><span class="sxs-lookup"><span data-stu-id="6ed2f-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="6ed2f-118">Kliknij **przycisk Wyślij / Odbierz** i spójrz na przycisk Praca w **trybie offline.**</span><span class="sxs-lookup"><span data-stu-id="6ed2f-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="6ed2f-119">Jeśli jest niebieski, jesteś rozłączony.</span><span class="sxs-lookup"><span data-stu-id="6ed2f-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="6ed2f-120">Kliknij go, aby się połączyć (przycisk zmieni kolor na biały) i kliknij przycisk **Wyślij wszystko**.</span><span class="sxs-lookup"><span data-stu-id="6ed2f-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="6ed2f-121">**Włącz wysyłanie natychmiast po podłączeniu**</span><span class="sxs-lookup"><span data-stu-id="6ed2f-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="6ed2f-122">Na karcie Plik kliknij pozycję **Opcje**.</span><span class="sxs-lookup"><span data-stu-id="6ed2f-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="6ed2f-123">W oknie dialogowym Opcje programu Outlook kliknij pozycję **Zaawansowane**.</span><span class="sxs-lookup"><span data-stu-id="6ed2f-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="6ed2f-124">W sekcji Wyślij i odbierz kliknij, aby natychmiast włączyć **opcję Wyślij po podłączeniu**.</span><span class="sxs-lookup"><span data-stu-id="6ed2f-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="6ed2f-125">Kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="6ed2f-125">Click **OK**.</span></span>
 
<span data-ttu-id="6ed2f-126">Aby uzyskać szczegółowe informacje, zobacz:</span><span class="sxs-lookup"><span data-stu-id="6ed2f-126">For full details, see:</span></span>
- [<span data-ttu-id="6ed2f-127">Klip wideo: wysyłanie lub usuwanie zablokowanej wiadomości e-mail</span><span class="sxs-lookup"><span data-stu-id="6ed2f-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="6ed2f-128">Poczta e-mail pozostaje w folderze Skrzynka nadawcza do czasu ręcznego zainicjowania operacji wysyłania/odbierania w programie Outlook</span><span class="sxs-lookup"><span data-stu-id="6ed2f-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
