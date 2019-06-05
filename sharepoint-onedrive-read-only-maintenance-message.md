---
title: 127 pojawia się błąd TenantAccessBlockedException podczas uzyskiwania dostępu do poczty e-mail?
ms.author: kirks
author: Techwriter40
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
ms.openlocfilehash: 54ebc269b391e6b0d607e55af8283ebf3d9e2aa7
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/04/2019
ms.locfileid: "34715081"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="8a6a2-102">Tylko do odczytu dla utrzymania komunikat podczas próby użycia programu SharePoint lub OneDrive</span><span class="sxs-lookup"><span data-stu-id="8a6a2-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="8a6a2-103">Podczas próby użycia programu SharePoint lub OneDrive, użytkownicy mogą otrzymywać tylko do odczytu dla obsługi wiadomości.</span><span class="sxs-lookup"><span data-stu-id="8a6a2-103">Users may receive a Read-Only for Maintenance message when attempting to use SharePoint or OneDrive.</span></span>

<span data-ttu-id="8a6a2-104">Sprawdź, czy istnieje aktywnego zarządzania występujące w dzierżawie przechodząc do <a href="https://portal.office.com/adminportal/home#/MessageCenter">Centrum wiadomości</a>.</span><span class="sxs-lookup"><span data-stu-id="8a6a2-104">Check if there is active maintenance occurring on your tenant by navigating to the <a href="https://portal.office.com/adminportal/home#/MessageCenter">Message center</a>.</span></span> <span data-ttu-id="8a6a2-105">Wreszcie upewnij się, że odwiedź stronę <a href="https://portal.office.com/adminportal/home#/servicehealth">Usług zdrowotnych</a> , aby sprawdzić, czy wszystkie klasyfikatory/incydentów, które może mieć miejsce.</span><span class="sxs-lookup"><span data-stu-id="8a6a2-105">Finally, ensure you visit the <a href="https://portal.office.com/adminportal/home#/servicehealth">Service Health</a> page to check for any advisories/incidents that may be occurring.</span></span>

<span data-ttu-id="8a6a2-106">Centrum wiadomości ani służby zdrowia Dashboard zauważyli nic na temat bieżących napraw dla dzierżawy, może to być przeglądarki buforowanie problemu.</span><span class="sxs-lookup"><span data-stu-id="8a6a2-106">If neither the Message Center or Service Health Dashboard have noted anything about current maintenance for your tenant, this may be a browser caching issue.</span></span>

<span data-ttu-id="8a6a2-107">Spróbuj wyczyścić pamięć podręczną przeglądarki przed nawigowania do witryny.</span><span class="sxs-lookup"><span data-stu-id="8a6a2-107">Please attempt to clear the browser cache before navigating to the site.</span></span>

  <li><span data-ttu-id="8a6a2-108">W przeglądarce Microsoft Edge, przejdź do <strong>więcej &hellip; &gt; ustawienia</strong></span><span class="sxs-lookup"><span data-stu-id="8a6a2-108">In the Microsoft Edge browser, go to <strong>More &hellip;&gt; Settings</strong></span></span></li>  <li><span data-ttu-id="8a6a2-109">W obszarze <strong>Przeglądanie wyczyść </strong>wybierz opcję <strong>Wybierz elementy do wyczyszczenia</strong>.</span><span class="sxs-lookup"><span data-stu-id="8a6a2-109">Under <strong>Clear browsing </strong>, select <strong>Choose what to clear</strong>.</span></span></li>  <li><span data-ttu-id="8a6a2-110">Zaznacz pole wyboru dane zapisane strony internetowej i plików cookie i wybierz <strong>Wyczyść</strong>.</span><span class="sxs-lookup"><span data-stu-id="8a6a2-110">Select the Cookies and saved website data check box and select <strong>Clear</strong>.</span></span></li>  </ol>  

<span data-ttu-id="8a6a2-111">**Uwaga**: te kroki mogą się różnić, jeżeli używasz innej przeglądarki, takie jak Firefox lub Chrome.</span><span class="sxs-lookup"><span data-stu-id="8a6a2-111">**Note**: These steps may differ when using other browsers such as Firefox or Chrome.</span></span>

