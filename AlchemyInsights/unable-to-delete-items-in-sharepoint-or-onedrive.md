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
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049527"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="b5578-102">Nie można usunąć elementów</span><span class="sxs-lookup"><span data-stu-id="b5578-102">Unable to delete items</span></span>

<span data-ttu-id="b5578-103">Masz problemy z usunięciem elementów programu SharePoint?</span><span class="sxs-lookup"><span data-stu-id="b5578-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="b5578-104">Zawsze upewnij się, że masz [odpowiednie uprawnienia](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) do usunięcia elementu lub próba usunięcia elementu przez [administratora zbioru witryn](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) .</span><span class="sxs-lookup"><span data-stu-id="b5578-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="b5578-105">Upewnij się, że w elemencie nie ma ustawienia [zasad przechowywania](https://docs.microsoft.com/office365/securitycompliance/retention-policies) .</span><span class="sxs-lookup"><span data-stu-id="b5578-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="b5578-106">Upewnij się, że element nie jest [wyewidencjonowany](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) dla innego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="b5578-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="b5578-107">Na koniec Administratorzy mogą używać [wzorców i praktyk programu SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP), który zawiera bibliotekę poleceń programu PowerShell, które umożliwiają wykonywanie złożonych działań zarządzania, takich jak wymuszenie usunięcia uparty elementów.</span><span class="sxs-lookup"><span data-stu-id="b5578-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="b5578-108">Usuń plik PNP</span><span class="sxs-lookup"><span data-stu-id="b5578-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="b5578-109">Usuń folder PNP</span><span class="sxs-lookup"><span data-stu-id="b5578-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="b5578-110">Usuń element listy PNP</span><span class="sxs-lookup"><span data-stu-id="b5578-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="b5578-111">Usuń listę PNP</span><span class="sxs-lookup"><span data-stu-id="b5578-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="b5578-112">Usuń pole PNP (kolumna)</span><span class="sxs-lookup"><span data-stu-id="b5578-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)