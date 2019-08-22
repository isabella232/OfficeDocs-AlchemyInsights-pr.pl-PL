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
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530894"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="d0342-102">E-mail przepływu pracy nie jest wysyłany do listy programu SharePoint lub biblioteki</span><span class="sxs-lookup"><span data-stu-id="d0342-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="d0342-103">Wiadomości e-mail z przepływów pracy nie są wysyłane do wszystkich użytkowników lub tylko określonych użytkowników lub widać, że błąd **wiadomość e-mail nie może zostać wysłana. Upewnić się, czy wiadomość e-mail ma prawidłowego adresata**.</span><span class="sxs-lookup"><span data-stu-id="d0342-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="d0342-104">Sprawdź, czy użytkownik istnieje w grupie uprawnienia **Wszystkich osób** (Lista informacji o użytkownikach) dla tego zbioru witryn.</span><span class="sxs-lookup"><span data-stu-id="d0342-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="d0342-105">Przykładowe bezpośredni adres URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="d0342-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="d0342-106">Jeśli użytkownik nie istnieje, upewnij się, że użytkownik jest zalogowany w stronę.</span><span class="sxs-lookup"><span data-stu-id="d0342-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="d0342-107">Jeśli jest to użytkownik zewnętrzny, upewnij się, że ich zaproszenie zostało zaakceptowane.</span><span class="sxs-lookup"><span data-stu-id="d0342-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="d0342-108">Jeśli użytkownik istnieje w grupie uprawnień, upewnij się, że adres e-mail jest poprawny.</span><span class="sxs-lookup"><span data-stu-id="d0342-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="d0342-109">Jeśli adres e-mail użytkownika nie jest ustawiona w tym polu, następnie utworzyć przykładowy alert dla tego użytkownika, co zmusza synchronizacji tego konta użytkownika z profilów użytkownika programu SharePoint do tego zbioru witryn.</span><span class="sxs-lookup"><span data-stu-id="d0342-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="d0342-110">Wiadomości e-mail z przepływów pracy są wysyłane do administratorów zbioru witryn, ale nie do innych użytkowników i wyświetlany jest błąd **HTTP zabrania się <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="d0342-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="d0342-111">Zobacz, [Odmowa dostępu podczas wysyłania wiadomości e-mail do grupy programu SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="d0342-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="d0342-112">Sprawdź także, że funkcji zbioru witryn **Tryb blokowania uprawnień ograniczony dostęp użytkownika** nie jest aktywne.</span><span class="sxs-lookup"><span data-stu-id="d0342-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="d0342-113">Tematy pokrewne</span><span class="sxs-lookup"><span data-stu-id="d0342-113">Related topics</span></span>
<span data-ttu-id="d0342-114">Czy chcesz spróbować Flow Microsoft w dokumentacji Online programu SharePoint?</span><span class="sxs-lookup"><span data-stu-id="d0342-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="d0342-115">Utworzyć przepływ</span><span class="sxs-lookup"><span data-stu-id="d0342-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="d0342-116">SharePoint i przepływu</span><span class="sxs-lookup"><span data-stu-id="d0342-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


