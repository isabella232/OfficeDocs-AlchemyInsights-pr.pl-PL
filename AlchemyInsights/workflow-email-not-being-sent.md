---
title: Nie jest wysyłany e-mail przepływu pracy
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270682"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="66866-102">Nie jest wysyłany e-mail przepływu pracy</span><span class="sxs-lookup"><span data-stu-id="66866-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="66866-103">Wiadomości e-mail z przepływów pracy nie są wysyłane do wszystkich użytkowników lub tylko określonych użytkowników lub widać, że błąd **wiadomość e-mail nie może zostać wysłana. Upewnić się, czy wiadomość e-mail ma prawidłowego adresata**.</span><span class="sxs-lookup"><span data-stu-id="66866-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="66866-104">Sprawdź, czy użytkownik istnieje w grupie uprawnienia **Wszystkich osób** (Lista informacji o użytkownikach) dla tego zbioru witryn.</span><span class="sxs-lookup"><span data-stu-id="66866-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="66866-105">Przykładowe bezpośredni adres URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="66866-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="66866-106">Jeśli użytkownik nie istnieje, upewnij się, że użytkownik jest zalogowany w stronę.</span><span class="sxs-lookup"><span data-stu-id="66866-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="66866-107">Jeśli jest to użytkownik zewnętrzny, upewnij się, że ich zaproszenie zostało zaakceptowane.</span><span class="sxs-lookup"><span data-stu-id="66866-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="66866-108">Jeśli użytkownik istnieje w grupie uprawnień, upewnij się, że adres e-mail jest poprawny.</span><span class="sxs-lookup"><span data-stu-id="66866-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="66866-109">Jeśli adres e-mail użytkownika nie jest ustawiona w tym polu, następnie utworzyć przykładowy alert dla tego użytkownika, co zmusza synchronizacji tego konta użytkownika z profilów użytkownika programu SharePoint do tego zbioru witryn.</span><span class="sxs-lookup"><span data-stu-id="66866-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="66866-110">Wiadomości e-mail z przepływów pracy są wysyłane do administratorów zbioru witryn, ale nie do innych użytkowników i wyświetlany jest błąd \*\*HTTP zabrania się <spam> <spam> \*\* <spam> <spam>.</span><span class="sxs-lookup"><span data-stu-id="66866-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

    <span data-ttu-id="66866-111">Zobacz, [Odmowa dostępu, gdy wiadomości e-mail do grupy](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="66866-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="66866-112">Sprawdź także, że funkcji zbioru witryn **Tryb blokowania uprawnień ograniczony dostęp użytkownika** nie jest aktywne.</span><span class="sxs-lookup"><span data-stu-id="66866-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="66866-113">Tematy pokrewne</span><span class="sxs-lookup"><span data-stu-id="66866-113">Related topics</span></span>
<span data-ttu-id="66866-114">Czy chcesz spróbować Flow Microsoft w dokumentacji Online programu SharePoint?</span><span class="sxs-lookup"><span data-stu-id="66866-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="66866-115">Utworzyć przepływ</span><span class="sxs-lookup"><span data-stu-id="66866-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="66866-116">SharePoint i przepływu</span><span class="sxs-lookup"><span data-stu-id="66866-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


