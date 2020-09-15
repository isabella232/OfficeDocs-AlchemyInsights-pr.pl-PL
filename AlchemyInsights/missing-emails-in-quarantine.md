---
title: Brakujące wiadomości e-mail w kwarantannie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673724"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="d2584-102">Brakujące wiadomości e-mail w kwarantannie</span><span class="sxs-lookup"><span data-stu-id="d2584-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="d2584-103">Administratorzy mogą [wyświetlać, zwalniać lub usuwać te wiadomości.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="d2584-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="d2584-104">Aby otworzyć Centrum zabezpieczeń & zgodności, przejdź do [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="d2584-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="d2584-105">Aby otworzyć stronę kwarantanny bezpośrednio, przejdź do strony [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="d2584-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="d2584-106">Możesz wyszukiwać według następujących wartości:</span><span class="sxs-lookup"><span data-stu-id="d2584-106">You can search by the following values:</span></span>  

- <span data-ttu-id="d2584-107">**Identyfikator wiadomości**: unikatowy identyfikator globalny wiadomości.</span><span class="sxs-lookup"><span data-stu-id="d2584-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="d2584-108">Po zaznaczeniu wiadomości na liście zostanie wyświetlona wartość  **identyfikatora wiadomości**  w wyświetlonym okienku menu wysuwanego  **szczegóły**  .</span><span class="sxs-lookup"><span data-stu-id="d2584-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="d2584-109">Administratorzy mogą używać [funkcji śledzenia wiadomości](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) do znajdowania wiadomości i ich odpowiednich wartości identyfikatorów wiadomości.</span><span class="sxs-lookup"><span data-stu-id="d2584-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="d2584-110">**Adres E-mail nadawcy**: adres e-mail jednego nadawcy.</span><span class="sxs-lookup"><span data-stu-id="d2584-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="d2584-111">**Adres E-mail adresata**: adres e-mail jednego adresata.</span><span class="sxs-lookup"><span data-stu-id="d2584-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="d2584-112">**Temat**: Użyj całego tematu wiadomości.</span><span class="sxs-lookup"><span data-stu-id="d2584-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="d2584-113">W wyszukiwaniu wielkość liter nie jest uwzględniana.</span><span class="sxs-lookup"><span data-stu-id="d2584-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="d2584-114">Po wprowadzeniu kryteriów wyszukiwania kliknij przycisk ![ Odśwież ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Odśwież** , aby przefiltrować wyniki.  </span><span class="sxs-lookup"><span data-stu-id="d2584-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="d2584-115">Polecenia cmdlet służące do wyświetlania i zarządzania wiadomościami oraz plikami w kwarantannie są następujące:</span><span class="sxs-lookup"><span data-stu-id="d2584-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="d2584-116">DELETE-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="d2584-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="d2584-117">Eksportowanie — QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="d2584-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="d2584-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="d2584-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="d2584-119">[Wersja Preview — QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Zauważ, że to polecenie cmdlet jest przeznaczone tylko dla wiadomości, a nie do plików złośliwego oprogramowania w usłudze SharePoint Online, OneDrive dla firm lub w usłudze Teams.</span><span class="sxs-lookup"><span data-stu-id="d2584-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="d2584-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="d2584-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)