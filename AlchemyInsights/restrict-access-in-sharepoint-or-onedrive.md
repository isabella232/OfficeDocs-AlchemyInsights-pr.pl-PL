---
title: Ograniczanie dostępu w programie SharePoint lub OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b6be074ed5f7e83f8196ca3fe90252673896569f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29482823"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="72164-102">Ograniczanie dostępu w programie SharePoint lub OneDrive</span><span class="sxs-lookup"><span data-stu-id="72164-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="72164-p101">W programie SharePoint i OneDrive możesz ograniczyć dostęp do elementów, takich jak pliki, foldery i list poprzez przyznanie dostępu tylko do grup lub osób, które chcesz mieć dostęp. Domyślnie uprawnienia w programie SharePoint są dziedziczone z wyżej w hierarchii. Tak więc plik dziedziczą uprawnienia z folderu, który dziedziczy uprawnienia z biblioteki, która dziedziczy uprawnienia z witryny.</span><span class="sxs-lookup"><span data-stu-id="72164-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="72164-p102">Można udostępniać na wyższym poziomie (takich jak Udostępnianie całej witryny) i następnie przerwać dziedziczenie, jeśli nie chcesz udostępniać wszystkie elementy na stronie. Jednak nie jest to zalecane, ponieważ to sprawia, że utrzymywanie uprawnienia bardziej skomplikowana i myląca w przyszłości. Oto, co można zrobić w zamian:</span><span class="sxs-lookup"><span data-stu-id="72164-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="72164-109">Jeśli na przykład chcesz udostępnić całą zawartość folderu z wyjątkiem jednego pliku w nim, należy przenieść ten plik do nowej lokalizacji, która nie jest udostępniony.</span><span class="sxs-lookup"><span data-stu-id="72164-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="72164-110">Jeśli masz dwa podfoldery w folderze, a chcesz udostępnić jeden podfolder z grupy A i B oraz dostęp do tylko grupa A drugi podfolderu, udostępnić folder nadrzędny z grupy A i dodać grupy B do pierwszego podfolderu.</span><span class="sxs-lookup"><span data-stu-id="72164-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="72164-111">Zatrzymaj udostępnianie pliku lub folderu</span><span class="sxs-lookup"><span data-stu-id="72164-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

