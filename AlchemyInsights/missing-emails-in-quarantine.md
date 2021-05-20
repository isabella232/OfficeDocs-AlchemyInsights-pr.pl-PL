---
title: Brakujące wiadomości e-mail w kwarantannie
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539834"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="1f094-102">Brakujące wiadomości e-mail w kwarantannie"</span><span class="sxs-lookup"><span data-stu-id="1f094-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="1f094-103">Administratorzy [mogą wyświetlać, zwalniać lub usuwać te wiadomości.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span><span class="sxs-lookup"><span data-stu-id="1f094-103">Administrators can [view, release, or delete these messages.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span></span>

<span data-ttu-id="1f094-104">Aby otworzyć Centrum zgodności & zabezpieczeń, przejdź do [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="1f094-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="1f094-105">Aby otworzyć stronę kwarantanny bezpośrednio, przejdź do [https://protection.office.com/quarantine](https://protection.office.com/quarantine) strony .</span><span class="sxs-lookup"><span data-stu-id="1f094-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="1f094-106">Możesz wyszukiwać według następujących wartości:</span><span class="sxs-lookup"><span data-stu-id="1f094-106">You can search by the following values:</span></span>  

- <span data-ttu-id="1f094-107">**Identyfikator wiadomości:** unikatowy identyfikator globalny wiadomości.</span><span class="sxs-lookup"><span data-stu-id="1f094-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="1f094-108">Jeśli wybierzesz wiadomość na liście, wartość Identyfikator wiadomości zostanie wyświetlona w  **wyświetlonym okienku wysuwu** Szczegóły.</span><span class="sxs-lookup"><span data-stu-id="1f094-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="1f094-109">Administratorzy mogą za [pomocą funkcji śledzenia wiadomości](/microsoft-365/security/office-365-security/message-trace-scc) znaleźć wiadomości i odpowiadające im wartości identyfikatora wiadomości.</span><span class="sxs-lookup"><span data-stu-id="1f094-109">Admins can use [message trace](/microsoft-365/security/office-365-security/message-trace-scc) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="1f094-110">**Adres e-mail nadawcy:** adres e-mail jednego nadawcy.</span><span class="sxs-lookup"><span data-stu-id="1f094-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="1f094-111">**Adres e-mail adresata:** adres e-mail pojedynczego adresata.</span><span class="sxs-lookup"><span data-stu-id="1f094-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="1f094-112">**Temat:** użyj całego tematu wiadomości.</span><span class="sxs-lookup"><span data-stu-id="1f094-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="1f094-113">W wyszukiwaniu nie jest wróżniana wielkość liter.</span><span class="sxs-lookup"><span data-stu-id="1f094-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="1f094-114">Po wprowadzeniu kryteriów wyszukiwania kliknij przycisk Odśwież, aby ![ ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  przefiltrować wyniki.</span><span class="sxs-lookup"><span data-stu-id="1f094-114">After you've entered the search criteria, click ![Refresh button](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** to filter the results.</span></span>

<span data-ttu-id="1f094-115">Polecenia cmdlet, których używasz do wyświetlania wiadomości i plików w kwarantannie oraz zarządzania nimi w kwarantannie, to:</span><span class="sxs-lookup"><span data-stu-id="1f094-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="1f094-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="1f094-116">Delete-QuarantineMessage</span></span>](/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="1f094-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="1f094-117">Export-QuarantineMessage</span></span>](/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="1f094-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="1f094-118">Get-QuarantineMessage</span></span>](/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="1f094-119">[Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)To polecenie cmdlet jest tylko dla wiadomości, a nie plików złośliwego oprogramowania z programu Microsoft Defender dla usługi Office 365 dla usługi SharePoint Online, OneDrive dla Firm lub Teams.</span><span class="sxs-lookup"><span data-stu-id="1f094-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from Microsoft Defender for Office 365 for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="1f094-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="1f094-120">Release-QuarantineMessage</span></span>](/powershell/module/exchange/release-quarantinemessage)