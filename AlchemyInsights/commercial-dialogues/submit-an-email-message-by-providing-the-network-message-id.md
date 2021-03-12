---
title: Przesyłanie wiadomości e-mail przez podanie identyfikatora wiadomości sieciowej
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748213"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="ab67b-102">Przesyłanie wiadomości e-mail przez podanie identyfikatora wiadomości sieciowej</span><span class="sxs-lookup"><span data-stu-id="ab67b-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="ab67b-103">W **wysuwanych informacjach** Nowe przesyłanie wybierz pozycję Adres **e-mail** **i identyfikator wiadomości sieciowej**.</span><span class="sxs-lookup"><span data-stu-id="ab67b-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="ab67b-104">Aby znaleźć identyfikator wiadomości e-mail w programie Outlook, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="ab67b-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="ab67b-105">Kliknij dwukrotnie wiadomość e-mail, aby ją otworzyć.</span><span class="sxs-lookup"><span data-stu-id="ab67b-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="ab67b-106">Wybierz **pozycję Właściwości**  >  **pliku.**</span><span class="sxs-lookup"><span data-stu-id="ab67b-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="ab67b-107">Otwórz Notatnik lub pusty dokument programu Word, a następnie  skopiuj i wklej zawartość, która znajduje się w polu nagłówków internetowych, do otwartego dokumentu, aby poprawić widoczność.</span><span class="sxs-lookup"><span data-stu-id="ab67b-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="ab67b-108">Zlokalizuj pole **X-MS-Exchange-Organization-Network-Message-Id.**</span><span class="sxs-lookup"><span data-stu-id="ab67b-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="ab67b-109">Wartość po **:** to identyfikator potrzebny do przesłania.</span><span class="sxs-lookup"><span data-stu-id="ab67b-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="ab67b-110">W **obszarze Adresaci**, jeśli wiadomość e-mail trafiła do folderu wiadomości-śmieci dla wszystkich adresatów tej wiadomości, wybierz **pozycję Zaznacz wszystko.**</span><span class="sxs-lookup"><span data-stu-id="ab67b-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="ab67b-111">Jeśli nie, wybierz tylko tego użytkownika, który zgłosił problem.</span><span class="sxs-lookup"><span data-stu-id="ab67b-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="ab67b-112">W obszarze Przyczyna przesłania , jeśli została wybrane polecenie Powinna zostać zablokowana **,** określ, czy wiadomość powinna zostać zablokowana jako **spam,** **wyłudzanie** informacji **lub** złośliwe **oprogramowanie,** a następnie wybierz **pozycję Prześlij.**</span><span class="sxs-lookup"><span data-stu-id="ab67b-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="ab67b-113">Aby dowiedzieć się więcej, zobacz Jak przesłać podejrzaną [wiadomość-chło-śmieci,](https://go.microsoft.com/fwlink/?linkid=2101479)wyłudzy, adresy URL i pliki do firmy Microsoft w celu skanowania.</span><span class="sxs-lookup"><span data-stu-id="ab67b-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
