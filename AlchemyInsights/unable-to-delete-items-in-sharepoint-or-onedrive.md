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
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511986"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="fadbb-102">Nie można usunąć elementów</span><span class="sxs-lookup"><span data-stu-id="fadbb-102">Unable to delete items</span></span>

<span data-ttu-id="fadbb-103">Zasady przechowywania może to spowodować, należy wyłączyć lub wykluczyć odpowiednie wstrzymanie, które jest przyczyną tego problemu.</span><span class="sxs-lookup"><span data-stu-id="fadbb-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="fadbb-104">Po usunięciu zasad przechowywania lub wstrzymania zmiana może potrwać do 24 godzin, aby zmiana mogła zostać wniesiena.</span><span class="sxs-lookup"><span data-stu-id="fadbb-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="fadbb-105">Upewnij się, że nie ma konfiguracji [zasad przechowywania](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) dla elementu.</span><span class="sxs-lookup"><span data-stu-id="fadbb-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="fadbb-106">Witryna mogła przekroczyć limit magazynowania, zwiększyć [przydział lokacji](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) i usunąć element.</span><span class="sxs-lookup"><span data-stu-id="fadbb-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="fadbb-107">Upewnij się, że element nie jest [wyewidencjonowany](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) dla innego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="fadbb-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="fadbb-108">Na koniec administratorzy mogą używać [wzorców i praktyk programu SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), która zawiera bibliotekę poleceń programu PowerShell, które umożliwiają wykonywanie złożonych akcji zarządzania, takich jak wymuszanie usuwania uporczywych elementów.</span><span class="sxs-lookup"><span data-stu-id="fadbb-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="fadbb-109">Usuń plik PNP</span><span class="sxs-lookup"><span data-stu-id="fadbb-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="fadbb-110">Usuń folder PNP</span><span class="sxs-lookup"><span data-stu-id="fadbb-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="fadbb-111">Usuń element listy PNP</span><span class="sxs-lookup"><span data-stu-id="fadbb-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="fadbb-112">Usuń listę PNP</span><span class="sxs-lookup"><span data-stu-id="fadbb-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="fadbb-113">Usuń pole PNP (kolumna)</span><span class="sxs-lookup"><span data-stu-id="fadbb-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)