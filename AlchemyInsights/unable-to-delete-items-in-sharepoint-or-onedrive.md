---
title: Nie można usunąć elementów w programie SharePoint lub OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571281"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="d591c-102">Nie można usunąć elementów</span><span class="sxs-lookup"><span data-stu-id="d591c-102">Unable to delete items</span></span>

<span data-ttu-id="d591c-103">Zasady przechowywania może to spowodować, należy wyłączyć lub wykluczyć odpowiednie wstrzymanie, które jest przyczyną tego problemu.</span><span class="sxs-lookup"><span data-stu-id="d591c-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="d591c-104">Po usunięciu zasad przechowywania lub blokady zmiana może potrwać do 24 godzin.</span><span class="sxs-lookup"><span data-stu-id="d591c-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="d591c-105">Upewnij się, że nie ma konfiguracji [zasad przechowywania](https://docs.microsoft.com/office365/securitycompliance/retention-policies) w elemencie.</span><span class="sxs-lookup"><span data-stu-id="d591c-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="d591c-106">Lokacja mogła przekroczyć limit magazynowania, zwiększyć [przydział lokacji](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) i usunąć element.</span><span class="sxs-lookup"><span data-stu-id="d591c-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="d591c-107">Upewnij się, że element nie jest [wyewidencjonowany](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) do innego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="d591c-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="d591c-108">Na koniec administratorzy mogą używać [wzorców i praktyk programu SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), który zawiera bibliotekę poleceń programu PowerShell, które umożliwiają wykonywanie złożonych akcji zarządzania, takich jak wymuszanie usuwania upartych elementów.</span><span class="sxs-lookup"><span data-stu-id="d591c-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="d591c-109">Usuwanie pliku PNP</span><span class="sxs-lookup"><span data-stu-id="d591c-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="d591c-110">Usuwanie folderu PNP</span><span class="sxs-lookup"><span data-stu-id="d591c-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="d591c-111">Usuń element listy PNP</span><span class="sxs-lookup"><span data-stu-id="d591c-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="d591c-112">Usuń listę PNP</span><span class="sxs-lookup"><span data-stu-id="d591c-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="d591c-113">Usuwanie pola PNP (kolumna)</span><span class="sxs-lookup"><span data-stu-id="d591c-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)