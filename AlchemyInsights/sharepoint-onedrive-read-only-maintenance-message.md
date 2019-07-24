---
title: Tylko do odczytu dla utrzymania komunikat podczas próby użycia programu SharePoint lub OneDrive
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: cc232fba6f502e2b6f282a8c1a1e29221e36b70d
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840525"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="4be39-102">Tylko do odczytu dla utrzymania komunikat podczas próby użycia programu SharePoint lub OneDrive</span><span class="sxs-lookup"><span data-stu-id="4be39-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="4be39-103">Użytkownicy może pojawić się **Tylko do odczytu dla utrzymania** komunikat podczas próby użycia programu SharePoint lub OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4be39-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive.</span></span>  <span data-ttu-id="4be39-104">Jeśli tak, należy sprawdzić, czy jest aktywne konserwacji występujące w dzierżawie przechodząc do [Centrum wiadomości](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="4be39-104">If so, check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span> <span data-ttu-id="4be39-105">Ponadto należy koniecznie sprawdź pulpit nawigacyjny [Kondycji usługi](https://portal.office.com/adminportal/home#/servicehealth) , aby sprawdzić, czy wszystkie klasyfikatory/incydentów, które może mieć miejsce.</span><span class="sxs-lookup"><span data-stu-id="4be39-105">Also, make sure to check the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) dashboard to check for any advisories/incidents that may be occurring.</span></span>

<span data-ttu-id="4be39-106">Centrum wiadomości ani kondycji usług pulpitu nawigacyjnego zauważyli nic na temat bieżących napraw dla dzierżawy, może to być przeglądarki buforowanie problemu.</span><span class="sxs-lookup"><span data-stu-id="4be39-106">If neither the Message Center or Service Health dashboard have noted anything about current maintenance for your tenant, this may be a browser caching issue.</span></span>

<span data-ttu-id="4be39-107">Spróbuj wyczyścić pamięć podręczną przeglądarki przed nawigowania do witryny.</span><span class="sxs-lookup"><span data-stu-id="4be39-107">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="4be39-108">W przeglądarce Microsoft Edge wybierz **Ustawienia**, a następnie wybierz **Prywatność i Bezpieczeństwo**.</span><span class="sxs-lookup"><span data-stu-id="4be39-108">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="4be39-109">W obszarze **Przeglądanie wyczyść**wybierz opcję **Wybierz elementy do wyczyszczenia**.</span><span class="sxs-lookup"><span data-stu-id="4be39-109">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="4be39-110">Wybierz **pliki cookie i zapisane dane witryn internetowych**, a następnie wybierz **Wyczyść**.</span><span class="sxs-lookup"><span data-stu-id="4be39-110">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="4be39-111">Te kroki mogą się różnić, jeżeli używasz innej przeglądarki, takich jak Google Chrome lub Mozilla Firefox.</span><span class="sxs-lookup"><span data-stu-id="4be39-111">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="4be39-112">Innym rozwiązaniem byłoby otworzyć witryny programu SharePoint lub OneDrive w nowym oknie InPrivate.</span><span class="sxs-lookup"><span data-stu-id="4be39-112">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>