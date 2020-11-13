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
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019593"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="e86af-102">Nie można usunąć elementów</span><span class="sxs-lookup"><span data-stu-id="e86af-102">Unable to delete items</span></span>

- <span data-ttu-id="e86af-103">Zasady przechowywania mogą być przyczyną tego problemu, należy wyłączyć lub wykluczyć odpowiednie zawieszenie, które powoduje ten problem.</span><span class="sxs-lookup"><span data-stu-id="e86af-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="e86af-104">Gdy zasady przechowywania lub wstrzymanie zostaną usunięte, może upłynąć do 24 godzin, aby zmiana została uwzględniona.</span><span class="sxs-lookup"><span data-stu-id="e86af-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="e86af-105">Upewnij się, że nie ma konfiguracji [zasad przechowywania](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) dla elementu.</span><span class="sxs-lookup"><span data-stu-id="e86af-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="e86af-106">Witryna mogła Przekroczono limit miejsca, zwiększyć [przydział witryny](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) i usunąć element.</span><span class="sxs-lookup"><span data-stu-id="e86af-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

- <span data-ttu-id="e86af-107">Upewnij się, że element nie został [wyewidencjonowany](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) przez innego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="e86af-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="e86af-108">Na koniec Administratorzy mogą używać [wzorów i procedur programu SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP), które zawierają bibliotekę poleceń programu PowerShell, które umożliwiają wykonywanie złożonych akcji zarządzania, takich jak Wymuś usuwanie stubborn elementów.</span><span class="sxs-lookup"><span data-stu-id="e86af-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="e86af-109">Usuwanie pliku PNP</span><span class="sxs-lookup"><span data-stu-id="e86af-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="e86af-110">Usuwanie folderu PNP</span><span class="sxs-lookup"><span data-stu-id="e86af-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="e86af-111">Usuwanie elementu listy PNP</span><span class="sxs-lookup"><span data-stu-id="e86af-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="e86af-112">Usuwanie listy PNP</span><span class="sxs-lookup"><span data-stu-id="e86af-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="e86af-113">Usuwanie pola PNP (kolumny)</span><span class="sxs-lookup"><span data-stu-id="e86af-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)