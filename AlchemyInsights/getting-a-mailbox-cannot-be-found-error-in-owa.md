---
title: 126 Nie można odnaleźć skrzynki pocztowej w programie OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426672"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="523c2-102">Błąd nie można odnaleźć skrzynki pocztowej w aplikacji Outlook w sieci Web?</span><span class="sxs-lookup"><span data-stu-id="523c2-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="523c2-103">Jeśli korzystasz z aplikacji Outlook w  sieci Web i nie można odnaleźć skrzynki pocztowej z powodu błędu, konto użyte do nawiązania połączenia z usługą Outlook w sieci Web nie ma licencji usługi Exchange Online, a zatem z kontem nie jest skojarzona żadna skrzynka pocztowa.</span><span class="sxs-lookup"><span data-stu-id="523c2-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="523c2-104">Administrator może przypisać licencję do Twojego konta, korzystając z następujących kroków:</span><span class="sxs-lookup"><span data-stu-id="523c2-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="523c2-105">Otwórz centrum [administracyjne platformy Microsoft 365](https://portal.office.com/adminportal/home#/homepage) i  przejdź do pozycji Aktywni użytkownicy w sekcji Użytkownicy, a następnie wybierz użytkownika, który widzi błąd. </span><span class="sxs-lookup"><span data-stu-id="523c2-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="523c2-106">Na otwartej stronie użytkownika przejdź  do sekcji Licencje i  aplikacje, wybierz odpowiednią wartość Lokalizacja i przypisz licencję zawierającą usługę Exchange Online (rozwiń licencję, aby wyświetlić jej szczegóły).</span><span class="sxs-lookup"><span data-stu-id="523c2-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="523c2-107">Po zakończeniu kliknij pozycję **Zapisz zmiany**.</span><span class="sxs-lookup"><span data-stu-id="523c2-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="523c2-108">W niektórych przypadkach, jeśli licencja jest już przypisana do konta użytkownika, usunięcie i ponowne przypisanie licencji pomaga rozwiązać ten problem i uzyskać jego poprawnie aprowizowane w systemie:</span><span class="sxs-lookup"><span data-stu-id="523c2-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="523c2-109">Sprawdź, czy Twoja subskrypcja usługi M365 Exchange Online (i inne, jeśli masz subskrypcje) jest aktualna i nie wygasła niedawno.</span><span class="sxs-lookup"><span data-stu-id="523c2-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="523c2-110">Gdy już upewnisz się, że Twoja subskrypcja nie wygasła, a do konta użytkownika przypisano ważną licencję, może upłynąć do 24 godzin, aby uzyskać inicjowanie obsługi administracyjnej, dlatego może być konieczne zaczekanie na rozwiązanie problemu.</span><span class="sxs-lookup"><span data-stu-id="523c2-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="523c2-111">Aby uzyskać więcej informacji, zobacz [Przypisywanie licencji i zarządzanie nimi.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="523c2-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>