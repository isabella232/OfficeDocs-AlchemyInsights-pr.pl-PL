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
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831744"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="39f8b-102">Brakujące wiadomości e-mail w kwarantannie"</span><span class="sxs-lookup"><span data-stu-id="39f8b-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="39f8b-103">Administratorzy [mogą wyświetlać, zwalniać lub usuwać te wiadomości.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="39f8b-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="39f8b-104">Aby otworzyć Centrum zgodności & zabezpieczeń, przejdź do [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="39f8b-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="39f8b-105">Aby otworzyć stronę kwarantanny bezpośrednio, przejdź do [https://protection.office.com/quarantine](https://protection.office.com/quarantine) strony .</span><span class="sxs-lookup"><span data-stu-id="39f8b-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="39f8b-106">Możesz wyszukiwać według następujących wartości:</span><span class="sxs-lookup"><span data-stu-id="39f8b-106">You can search by the following values:</span></span>  

- <span data-ttu-id="39f8b-107">**Identyfikator wiadomości:** unikatowy identyfikator globalny wiadomości.</span><span class="sxs-lookup"><span data-stu-id="39f8b-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="39f8b-108">Jeśli wybierzesz wiadomość na liście, wartość Identyfikator wiadomości zostanie wyświetlona w  **wyświetlonym okienku wysuwu** Szczegóły.</span><span class="sxs-lookup"><span data-stu-id="39f8b-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="39f8b-109">Administratorzy mogą za [pomocą funkcji śledzenia wiadomości](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) znaleźć wiadomości i odpowiadające im wartości identyfikatora wiadomości.</span><span class="sxs-lookup"><span data-stu-id="39f8b-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="39f8b-110">**Adres e-mail nadawcy:** adres e-mail jednego nadawcy.</span><span class="sxs-lookup"><span data-stu-id="39f8b-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="39f8b-111">**Adres e-mail adresata:** adres e-mail pojedynczego adresata.</span><span class="sxs-lookup"><span data-stu-id="39f8b-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="39f8b-112">**Temat:** użyj całego tematu wiadomości.</span><span class="sxs-lookup"><span data-stu-id="39f8b-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="39f8b-113">W wyszukiwaniu nie jest wróżniana wielkość liter.</span><span class="sxs-lookup"><span data-stu-id="39f8b-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="39f8b-114">Po wprowadzeniu kryteriów wyszukiwania kliknij przycisk Odśwież, aby ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  przefiltrować wyniki.  </span><span class="sxs-lookup"><span data-stu-id="39f8b-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="39f8b-115">Polecenia cmdlet, których używasz do wyświetlania wiadomości i plików w kwarantannie oraz zarządzania nimi w kwarantannie, to:</span><span class="sxs-lookup"><span data-stu-id="39f8b-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="39f8b-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="39f8b-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="39f8b-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="39f8b-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="39f8b-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="39f8b-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="39f8b-119">[Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Pamiętaj, że to polecenie cmdlet jest tylko dla wiadomości, a nie plików złośliwego oprogramowania z atp dla usługi SharePoint Online, OneDrive dla Firm lub Teams.</span><span class="sxs-lookup"><span data-stu-id="39f8b-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="39f8b-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="39f8b-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)