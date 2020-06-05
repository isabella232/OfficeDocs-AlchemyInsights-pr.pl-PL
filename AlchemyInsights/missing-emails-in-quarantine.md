---
title: Brakujące wiadomości e-mail w kwarantannie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569555"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="4d541-102">Brakujące e-maile w kwarantannie"</span><span class="sxs-lookup"><span data-stu-id="4d541-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="4d541-103">Administratorzy mogą [wyświetlać, zwalniać lub usuwać te wiadomości.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="4d541-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="4d541-104">Aby otworzyć Centrum zgodności & zabezpieczeń, przejdź do pliku [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="4d541-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="4d541-105">Aby otworzyć stronę kwarantanny bezpośrednio, przejdź do [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="4d541-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="4d541-106">Można wyszukiwać według następujących wartości:</span><span class="sxs-lookup"><span data-stu-id="4d541-106">You can search by the following values:</span></span>  

- <span data-ttu-id="4d541-107">**Identyfikator wiadomości:** globalnie unikatowy identyfikator wiadomości.</span><span class="sxs-lookup"><span data-stu-id="4d541-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="4d541-108">Jeśli wybierzesz wiadomość na liście, w wyświetlonym okienku wysuwu **szczegółów** pojawi się wartość **identyfikatora wiadomości.**</span><span class="sxs-lookup"><span data-stu-id="4d541-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="4d541-109">Administratorzy mogą używać [śledzenia wiadomości](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) do znajdowania wiadomości i odpowiadających im wartości identyfikatora wiadomości.</span><span class="sxs-lookup"><span data-stu-id="4d541-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="4d541-110">**Adres e-mail nadawcy:** adres e-mail pojedynczego nadawcy.</span><span class="sxs-lookup"><span data-stu-id="4d541-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="4d541-111">**Adres e-mail odbiorcy:** adres e-mail jednego adresata.</span><span class="sxs-lookup"><span data-stu-id="4d541-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="4d541-112">**Temat**: Użyj całego tematu wiadomości.</span><span class="sxs-lookup"><span data-stu-id="4d541-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="4d541-113">W wyszukiwaniu nie jest rozróżniana wielkość liter.</span><span class="sxs-lookup"><span data-stu-id="4d541-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="4d541-114">Po wprowadzeniu kryteriów wyszukiwania kliknij przycisk Odśwież przycisk ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Odśwież,** aby filtrować wyniki.  </span><span class="sxs-lookup"><span data-stu-id="4d541-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="4d541-115">Polecenia cmdlet używane do wyświetlania wiadomości i plików w kwarantannie oraz zarządzanie nimi to:</span><span class="sxs-lookup"><span data-stu-id="4d541-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="4d541-116">Usuń-KwarantannaMessage</span><span class="sxs-lookup"><span data-stu-id="4d541-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="4d541-117">Eksport-KwarantannaNajedzaj</span><span class="sxs-lookup"><span data-stu-id="4d541-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="4d541-118">Pobierz kwarantannęSeułka</span><span class="sxs-lookup"><span data-stu-id="4d541-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="4d541-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Należy pamiętać, że to polecenie cmdlet jest przeznaczone tylko dla wiadomości, a nie plików złośliwego oprogramowania z usługi ATP dla usługi SharePoint Online, OneDrive dla Firm lub Zespołów.</span><span class="sxs-lookup"><span data-stu-id="4d541-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="4d541-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="4d541-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)