---
title: E-mail przepływu pracy nie jest wysyłany
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049383"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="9d775-102">Wiadomości e-mail przepływu pracy nie są wysyłane do listy programu SharePoint lub biblioteki</span><span class="sxs-lookup"><span data-stu-id="9d775-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="9d775-103">Wiadomości e-mail z przepływów pracy nie są wysyłane do wszystkich użytkowników lub tylko określonych użytkowników lub zostanie wyświetlony błąd **nie można wysłać wiadomości e-mail. Upewnij się, że wiadomość e-mail ma prawidłowego adresata**.</span><span class="sxs-lookup"><span data-stu-id="9d775-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="9d775-104">Sprawdź, czy użytkownik istnieje w grupie uprawnienia **wszystkich osób** (lista informacji o użytkowniczek) dla tego zbioru witryn.</span><span class="sxs-lookup"><span data-stu-id="9d775-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="9d775-105">Przykładowy bezpośredni adres URL:<tenant>https://.<sitename>SharePoint.com/sites//_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="9d775-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="9d775-106">Jeśli użytkownik nie istnieje, upewnij się, że użytkownik jest zalogowany na stronie.</span><span class="sxs-lookup"><span data-stu-id="9d775-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="9d775-107">Jeśli jest to użytkownik zewnętrzny, upewnij się, że zaproszenie zostało zaakceptowane.</span><span class="sxs-lookup"><span data-stu-id="9d775-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="9d775-108">Jeśli użytkownik nie istnieje w grupie uprawnień, upewnij się, że adres e-mail jest poprawny.</span><span class="sxs-lookup"><span data-stu-id="9d775-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="9d775-109">Jeśli adres e-mail użytkowników nie jest ustawiony w tym miejscu, Utwórz przykładowy alert dla tego użytkownika, który wymusza synchronizację tego konta użytkownika z profilów użytkowników programu SharePoint do tego zbioru witryn.</span><span class="sxs-lookup"><span data-stu-id="9d775-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="9d775-110">Wiadomości e-mail z przepływów pracy są wysyłane do administratorów zbioru witryn, ale nie do innych użytkowników i Zobacz błąd **http zabronione <span>https:</span>/URL/_vti_bin/Client.XVC.Sp.Utilities.Utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="9d775-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="9d775-111">Zobacz [odmowa dostępu podczas wysyłania wiadomości e-mail do grupy programu SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="9d775-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="9d775-112">Ponadto sprawdź, czy funkcja zbioru witryn **trybu blokowania uprawnień ograniczonego dostępu użytkownika** nie jest aktywna.</span><span class="sxs-lookup"><span data-stu-id="9d775-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="9d775-113">Tematy pokrewne</span><span class="sxs-lookup"><span data-stu-id="9d775-113">Related topics</span></span>
<span data-ttu-id="9d775-114">Chcesz wypróbować usługi Microsoft Flow w usłudze SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="9d775-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="9d775-115">Utwórz przepływ</span><span class="sxs-lookup"><span data-stu-id="9d775-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="9d775-116">SharePoint i przepływu</span><span class="sxs-lookup"><span data-stu-id="9d775-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


