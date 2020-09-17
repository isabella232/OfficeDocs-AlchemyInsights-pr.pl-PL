---
title: Nie można usunąć elementów w programie SharePoint ani w usłudze OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806121"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="5b6a8-102">Nie można usunąć elementów</span><span class="sxs-lookup"><span data-stu-id="5b6a8-102">Unable to delete items</span></span>

<span data-ttu-id="5b6a8-103">Zasady przechowywania mogą być przyczyną tego problemu, należy wyłączyć lub wykluczyć odpowiednie zawieszenie, które powoduje ten problem.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="5b6a8-104">Gdy zasady przechowywania lub wstrzymanie zostaną usunięte, może upłynąć do 24 godzin, aby zmiana została uwzględniona.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="5b6a8-105">Upewnij się, że nie ma konfiguracji [zasad przechowywania](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) dla elementu.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="5b6a8-106">Witryna mogła Przekroczono limit miejsca, zwiększyć [przydział witryny](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) i usunąć element.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="5b6a8-107">Upewnij się, że element nie został [wyewidencjonowany](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) przez innego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="5b6a8-108">Na koniec Administratorzy mogą używać [wzorów i procedur programu SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP), które zawierają bibliotekę poleceń programu PowerShell, które umożliwiają wykonywanie złożonych akcji zarządzania, takich jak Wymuś usuwanie stubborn elementów.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="5b6a8-109">Usuwanie pliku PNP</span><span class="sxs-lookup"><span data-stu-id="5b6a8-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="5b6a8-110">Usuwanie folderu PNP</span><span class="sxs-lookup"><span data-stu-id="5b6a8-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="5b6a8-111">Usuwanie elementu listy PNP</span><span class="sxs-lookup"><span data-stu-id="5b6a8-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="5b6a8-112">Usuwanie listy PNP</span><span class="sxs-lookup"><span data-stu-id="5b6a8-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="5b6a8-113">Usuwanie pola PNP (kolumny)</span><span class="sxs-lookup"><span data-stu-id="5b6a8-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)