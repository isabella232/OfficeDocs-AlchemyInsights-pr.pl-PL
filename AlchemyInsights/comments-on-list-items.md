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
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982486"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="efde8-102">Komentarze dotyczące elementów listy</span><span class="sxs-lookup"><span data-stu-id="efde8-102">Comments on List items</span></span>

<span data-ttu-id="efde8-103">Użytkownicy wkrótce będą mogli dodawać i usuwać komentarze do elementów listy.</span><span class="sxs-lookup"><span data-stu-id="efde8-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="efde8-104">Użytkownicy mogą wyświetlać wszystkie komentarze w elemencie listy i filtrować między widokami pokazującymi komentarze lub działania związane z elementem.</span><span class="sxs-lookup"><span data-stu-id="efde8-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="efde8-105">**Chronometraż** :</span><span class="sxs-lookup"><span data-stu-id="efde8-105">**Timing** :</span></span>

<span data-ttu-id="efde8-106">**Wersja ukierunkowana** : stopniowe przewinięcie w połowie października i oczekiwanie na zakończenie w połowie listopada</span><span class="sxs-lookup"><span data-stu-id="efde8-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="efde8-107">**Wersja Standard** : stopniowe przewinięcie w połowie listopada i oczekiwanie na zakończenie przed dniem grudnia</span><span class="sxs-lookup"><span data-stu-id="efde8-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="efde8-108">**Wprowadzanie** : wersja ukierunkowana dla całej organizacji</span><span class="sxs-lookup"><span data-stu-id="efde8-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="efde8-109">Aby można było dodawać i usuwać komentarze, użytkownicy muszą zwrócić uwagę na następujące kwestie:</span><span class="sxs-lookup"><span data-stu-id="efde8-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="efde8-110">Komentarze są zgodne z ustawieniami uprawnień w programie SharePoint.</span><span class="sxs-lookup"><span data-stu-id="efde8-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="efde8-111">Listy klasyczne, które nie są jeszcze zbudowane do wyświetlania w nowoczesnych interfejsach użytkowników, na przykład listy zadań, nie będą miały tej funkcji komentowania.</span><span class="sxs-lookup"><span data-stu-id="efde8-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="efde8-112">Komentowanie list w aplikacji Teams nie jest dostępne w tej wersji.</span><span class="sxs-lookup"><span data-stu-id="efde8-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="efde8-113">Komentarze nie są indeksowane przez wyszukiwanie.</span><span class="sxs-lookup"><span data-stu-id="efde8-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="efde8-114">Administratorzy mogą wyłączyć tę funkcję na poziomie organizacji, zmieniając parametr **CommentsOnListItemsDisabled** w poleceniu cmdlet **Set-SPOTenant** programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="efde8-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="efde8-115">Obecnie nie można wyłączyć komentowania na poziomie witryny lub listy.</span><span class="sxs-lookup"><span data-stu-id="efde8-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="efde8-116">Mamy nadzieję, że te kontrolki będą znajdować się w nowszej aktualizacji, prawdopodobnie w pierwszym kwartale 2021.</span><span class="sxs-lookup"><span data-stu-id="efde8-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
