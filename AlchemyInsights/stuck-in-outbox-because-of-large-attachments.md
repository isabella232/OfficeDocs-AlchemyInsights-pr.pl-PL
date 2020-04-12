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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232640"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="c32c8-102">Naprawianie wiadomości, które utknęły w skrzynce nadawczej</span><span class="sxs-lookup"><span data-stu-id="c32c8-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="c32c8-103">Zaleca się, aby rozpocząć od uruchomienia [scenariusza "Mam problemy z wysyłaniem, odbieraniem lub znajdowaniem wiadomości e-mail"](https://aka.ms/SaRA-OutlookSendReceive) z narzędzia [Pomocy technicznej i odzyskiwania firmy Microsoft](https://diagnostics.office.com/#/) na komputerze, którego dotyczy problem.</span><span class="sxs-lookup"><span data-stu-id="c32c8-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="c32c8-104">Gdy wiadomość utknie w skrzynce nadawczej, najbardziej prawdopodobną przyczyną jest duży załącznik lub opcja "Wyślij natychmiast po podłączeniu" nie jest włączona.</span><span class="sxs-lookup"><span data-stu-id="c32c8-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="c32c8-105">**Usuń duży załącznik**</span><span class="sxs-lookup"><span data-stu-id="c32c8-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="c32c8-106">Kliknij **pozycję Wyślij / Odbierz** > pracę w**trybie offline**.</span><span class="sxs-lookup"><span data-stu-id="c32c8-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="c32c8-107">W okienku nawigacji kliknij pozycję **Skrzynka nadawcza**.</span><span class="sxs-lookup"><span data-stu-id="c32c8-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="c32c8-108">W tym miejscu możesz:</span><span class="sxs-lookup"><span data-stu-id="c32c8-108">From here, you can:</span></span> 
    - <span data-ttu-id="c32c8-109">Usuń wiadomość.</span><span class="sxs-lookup"><span data-stu-id="c32c8-109">Delete the message.</span></span> <span data-ttu-id="c32c8-110">Wystarczy go **zaznaczyć**i kliknąć usuń .</span><span class="sxs-lookup"><span data-stu-id="c32c8-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="c32c8-111">Przeciągnij wiadomość do **folderu wersji roboczych,** kliknij dwukrotnie, aby otworzyć wiadomość, i usuń załącznik (kliknij go i kliknij przycisk **Usuń**).</span><span class="sxs-lookup"><span data-stu-id="c32c8-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="c32c8-112">Jeśli błąd informuje, że program Outlook próbuje przesłać wiadomość, zamknij program Outlook.</span><span class="sxs-lookup"><span data-stu-id="c32c8-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="c32c8-113">Może upłynąć kilka chwil, aby wyjść.</span><span class="sxs-lookup"><span data-stu-id="c32c8-113">It may take a few moments to exit.</span></span> <span data-ttu-id="c32c8-114">Jeśli program Outlook nie zostanie zamknięty, naciśnij **klawisze Ctrl+Alt+Delete** i kliknij pozycję **Rozpocznij Menedżera zadań**.</span><span class="sxs-lookup"><span data-stu-id="c32c8-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="c32c8-115">W Menedżerze zadań wybierz kartę **Procesy,** przewiń w dół do programu outlook.exe i kliknij pozycję **Zakończ proces**.</span><span class="sxs-lookup"><span data-stu-id="c32c8-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="c32c8-116">Po zamknięciu programu Outlook uruchom ponownie program Outlook i powtórz kroki 2-3.</span><span class="sxs-lookup"><span data-stu-id="c32c8-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="c32c8-117">Po usunięciu załącznika kliknij przycisk **Wyślij / Odbierz** > **pracę w trybie offline,** aby usunąć zaznaczenie przycisku i wznowić pracę w trybie online.</span><span class="sxs-lookup"><span data-stu-id="c32c8-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="c32c8-118">Wiadomości utkną również w skrzynce nadawczej po **kliknięciu przycisku Wyślij**, ale nie masz połączenia.</span><span class="sxs-lookup"><span data-stu-id="c32c8-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="c32c8-119">Kliknij **przycisk Wyślij / Odbierz** i spójrz na przycisk Praca w **trybie offline.**</span><span class="sxs-lookup"><span data-stu-id="c32c8-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="c32c8-120">Jeśli jest niebieski, jesteś rozłączony.</span><span class="sxs-lookup"><span data-stu-id="c32c8-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="c32c8-121">Kliknij go, aby się połączyć (przycisk zmieni kolor na biały) i kliknij przycisk **Wyślij wszystko**.</span><span class="sxs-lookup"><span data-stu-id="c32c8-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="c32c8-122">**Włącz wysyłanie natychmiast po podłączeniu**</span><span class="sxs-lookup"><span data-stu-id="c32c8-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="c32c8-123">Na karcie Plik kliknij pozycję **Opcje**.</span><span class="sxs-lookup"><span data-stu-id="c32c8-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="c32c8-124">W oknie dialogowym Opcje programu Outlook kliknij pozycję **Zaawansowane**.</span><span class="sxs-lookup"><span data-stu-id="c32c8-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="c32c8-125">W sekcji Wyślij i odbierz kliknij, aby natychmiast włączyć **opcję Wyślij po podłączeniu**.</span><span class="sxs-lookup"><span data-stu-id="c32c8-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="c32c8-126">Kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="c32c8-126">Click **OK**.</span></span>
 
<span data-ttu-id="c32c8-127">Aby uzyskać szczegółowe informacje, zobacz:</span><span class="sxs-lookup"><span data-stu-id="c32c8-127">For full details, see:</span></span>
- [<span data-ttu-id="c32c8-128">Klip wideo: wysyłanie lub usuwanie zablokowanej wiadomości e-mail</span><span class="sxs-lookup"><span data-stu-id="c32c8-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="c32c8-129">Poczta e-mail pozostaje w folderze Skrzynka nadawcza do czasu ręcznego zainicjowania operacji wysyłania/odbierania w programie Outlook</span><span class="sxs-lookup"><span data-stu-id="c32c8-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
