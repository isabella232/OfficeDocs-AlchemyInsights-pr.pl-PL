---
title: Nie można uzyskać dostępu do tej witryny — błąd podczas próby uzyskania dostępu do witryny programu SharePoint z przeglądarki lub aplikacji Teams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005378"
- "9266"
ms.openlocfilehash: 451544fb85522e0eececc9274825805699685ee9
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747043"
---
# <a name="this-site-cant-be-reached-error-when-trying-to-access-sharepoint-site-from-browser-or-teams"></a><span data-ttu-id="82aa7-102">Błąd "Nie można uzyskać dostępu do tej witryny" podczas próby uzyskania dostępu do witryny programu SharePoint z przeglądarki lub aplikacji Teams</span><span class="sxs-lookup"><span data-stu-id="82aa7-102">“This site can’t be reached” error when trying to access SharePoint site from browser or Teams</span></span>

<span data-ttu-id="82aa7-103">Podczas próby uzyskania dostępu do witryny programu SharePoint z przeglądarki lub aplikacji Teams może zostać wyświetlony komunikat o błędzie "Nie można uzyskać dostępu do tej witryny".</span><span class="sxs-lookup"><span data-stu-id="82aa7-103">Users might receive "This site can't be reached" error when trying to access SharePoint site from browser or Teams.</span></span> 

<span data-ttu-id="82aa7-104">Aby rozwiązać ten problem:</span><span class="sxs-lookup"><span data-stu-id="82aa7-104">To resolve this issue:</span></span> 

1. <span data-ttu-id="82aa7-105">Sprawdź, czy strona główna znajduje się w Koszu, czy w Koszu drugiego poziomu, i przywróć stronę.</span><span class="sxs-lookup"><span data-stu-id="82aa7-105">Check if the home page is in Recycle bin or second-stage recycle bin and restore the page.</span></span>

<span data-ttu-id="82aa7-106">**Przykład bezpośredniego adresu URL do Kosza:**https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span><span class="sxs-lookup"><span data-stu-id="82aa7-106">**Sample direct URL to recycle bin**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span></span>

1. <span data-ttu-id="82aa7-107">Jeśli strona główna zostanie trwale usunięta z Kosza, utwórz nową stronę witryny z biblioteki Strony witryny i nadaj jej stronę główną.</span><span class="sxs-lookup"><span data-stu-id="82aa7-107">If the home page is permanently removed from the recycle bin, create a new site page from the Site Pages library and make it a homepage.</span></span> 

<span data-ttu-id="82aa7-108">**Przykładowy bezpośredni adres URL:**https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span><span class="sxs-lookup"><span data-stu-id="82aa7-108">**Sample direct URL**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span></span>