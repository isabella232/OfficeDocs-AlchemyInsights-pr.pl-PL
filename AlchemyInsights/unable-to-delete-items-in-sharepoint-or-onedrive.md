---
title: Nie można usunąć elementów w programie SharePoint lub OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: b25e6d144dcefcfed4258e78ad5cfd4089ba7d1e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558663"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="12f2c-102">Nie można usunąć elementów</span><span class="sxs-lookup"><span data-stu-id="12f2c-102">Unable to delete items</span></span>

<span data-ttu-id="12f2c-103">Masz problemy z usunięciem elementów programu SharePoint?</span><span class="sxs-lookup"><span data-stu-id="12f2c-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="12f2c-104">Zawsze upewnij się, że masz [odpowiednie uprawnienia](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) , aby usunąć element lub mają próba [administrator zbioru witryn](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) , Usuń element.</span><span class="sxs-lookup"><span data-stu-id="12f2c-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="12f2c-105">Upewnij się, że nie ma ustawienia [zasad przechowywania](https://docs.microsoft.com/office365/securitycompliance/retention-policies) dla towaru.</span><span class="sxs-lookup"><span data-stu-id="12f2c-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="12f2c-106">Upewnij się, że element nie jest [wyewidencjonowany przez](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) innego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="12f2c-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="12f2c-107">Wreszcie Administratorzy mogą używać [programu SharePoint wzorce i praktyki](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) który zawiera biblioteki programu PowerShell polecenia, które pozwalają na przeprowadzenie kompleksowego zarządzania akcje takie jak wymusić usunięcie elementów uporczywe.</span><span class="sxs-lookup"><span data-stu-id="12f2c-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="12f2c-108">Usuń plik PNP</span><span class="sxs-lookup"><span data-stu-id="12f2c-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="12f2c-109">Usuwanie folderu PNP</span><span class="sxs-lookup"><span data-stu-id="12f2c-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="12f2c-110">Usuwanie elementu listy PNP</span><span class="sxs-lookup"><span data-stu-id="12f2c-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="12f2c-111">Usuwanie listy PNP</span><span class="sxs-lookup"><span data-stu-id="12f2c-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="12f2c-112">Usuwanie PNP pola (kolumny)</span><span class="sxs-lookup"><span data-stu-id="12f2c-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)