---
title: Ograniczanie dostępu w programie SharePoint lub usłudze OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720692"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="de012-102">Ograniczanie dostępu w programie SharePoint lub usłudze OneDrive</span><span class="sxs-lookup"><span data-stu-id="de012-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="de012-103">W programie SharePoint i usłudze OneDrive możesz ograniczyć dostęp do elementów, takich jak pliki, foldery i listy, udzielając dostępu tylko grupom lub osobom, do których chcesz mieć dostęp.</span><span class="sxs-lookup"><span data-stu-id="de012-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="de012-104">Domyślnie uprawnienia w programie SharePoint są dziedziczone z wyższego poziomu w hierarchii.</span><span class="sxs-lookup"><span data-stu-id="de012-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="de012-105">Dzięki temu plik dziedziczy uprawnienia z folderu, który dziedziczy uprawnienia z biblioteki, co powoduje dziedziczenie uprawnień do witryny.</span><span class="sxs-lookup"><span data-stu-id="de012-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="de012-106">Możesz udostępnić na wyższym poziomie (na przykład udostępnić całą witrynę), a następnie przerwać dziedziczenie, jeśli nie chcesz udostępniać wszystkich elementów w witrynie.</span><span class="sxs-lookup"><span data-stu-id="de012-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="de012-107">Nie jest to jednak zalecane, ponieważ ułatwia to zachowanie uprawnień bardziej złożonych i mylących w przyszłości.</span><span class="sxs-lookup"><span data-stu-id="de012-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="de012-108">Możesz to zrobić w następujący sposób:</span><span class="sxs-lookup"><span data-stu-id="de012-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="de012-109">Jeśli na przykład chcesz udostępnić całą zawartość folderu z wyjątkiem jednego pliku, Przenieś ten plik do nowej lokalizacji, która nie jest udostępniona.</span><span class="sxs-lookup"><span data-stu-id="de012-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="de012-110">Jeśli w folderze znajdują się dwa podfoldery i chcesz udostępnić pojedynczy podfolder grupom a i B i zezwolić tylko na grupowanie w drugim podfolderze, Udostępnij folder nadrzędny grupie A i Dodaj grupę B do pierwszego podfolderu.</span><span class="sxs-lookup"><span data-stu-id="de012-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="de012-111">Zatrzymywanie udostępniania pliku lub folderu </span><span class="sxs-lookup"><span data-stu-id="de012-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

