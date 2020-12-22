---
title: Komentarze dotyczące elementów listy
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724164"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="ad086-102">Komentarze dotyczące elementów listy</span><span class="sxs-lookup"><span data-stu-id="ad086-102">Comments on List items</span></span>

<span data-ttu-id="ad086-103">Użytkownicy mogą wyświetlać wszystkie komentarze w elemencie listy i filtrować między widokami pokazującymi komentarze lub działania związane z elementem.</span><span class="sxs-lookup"><span data-stu-id="ad086-103">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="ad086-104">Aby można było dodawać i usuwać komentarze, użytkownicy muszą zwrócić uwagę na następujące kwestie:</span><span class="sxs-lookup"><span data-stu-id="ad086-104">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="ad086-105">Komentarze są zgodne z ustawieniami uprawnień w programie SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ad086-105">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="ad086-106">Listy klasyczne, które nie są jeszcze zbudowane do wyświetlania w nowoczesnych interfejsach użytkowników, na przykład listy zadań, nie będą miały tej funkcji komentowania.</span><span class="sxs-lookup"><span data-stu-id="ad086-106">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="ad086-107">Komentowanie list w aplikacji Teams nie jest dostępne w tej wersji.</span><span class="sxs-lookup"><span data-stu-id="ad086-107">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="ad086-108">Komentarze nie są indeksowane przez wyszukiwanie.</span><span class="sxs-lookup"><span data-stu-id="ad086-108">Comments are not indexed by Search.</span></span>

<span data-ttu-id="ad086-109">Administratorzy mogą wyłączyć tę funkcję na poziomie organizacji, zmieniając parametr **CommentsOnListItemsDisabled** w poleceniu cmdlet **Set-SPOTenant** programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ad086-109">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="ad086-110">Obecnie nie można wyłączyć komentowania na poziomie witryny lub listy.</span><span class="sxs-lookup"><span data-stu-id="ad086-110">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="ad086-111">Mamy nadzieję, że te kontrolki będą znajdować się w nowszej aktualizacji, prawdopodobnie w pierwszym kwartale 2021.</span><span class="sxs-lookup"><span data-stu-id="ad086-111">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
