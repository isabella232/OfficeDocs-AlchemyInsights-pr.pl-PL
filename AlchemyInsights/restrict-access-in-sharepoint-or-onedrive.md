---
title: Ograniczanie dostępu w programie SharePoint lub OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715894"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="6ff57-102">Ograniczanie dostępu w programie SharePoint lub OneDrive</span><span class="sxs-lookup"><span data-stu-id="6ff57-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="6ff57-103">W programie SharePoint i OneDrive ograniczasz dostęp do elementów, takich jak pliki, foldery i listy, przyznając dostęp tylko grupom lub osobom, do których chcesz mieć dostęp.</span><span class="sxs-lookup"><span data-stu-id="6ff57-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="6ff57-104">Domyślnie uprawnienia w programie SharePoint są dziedziczone z wyższej pozycji w hierarchii.</span><span class="sxs-lookup"><span data-stu-id="6ff57-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="6ff57-105">Tak więc plik dziedziczy jego uprawnienia z folderu, który dziedziczy jego uprawnienia z biblioteki, która dziedziczy jego uprawnienia z witryny.</span><span class="sxs-lookup"><span data-stu-id="6ff57-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="6ff57-106">Możesz udostępniać na wyższym poziomie (na przykład udostępniając całą witrynę), a następnie przerywać dziedziczenie, jeśli nie chcesz udostępniać wszystkich elementów w witrynie.</span><span class="sxs-lookup"><span data-stu-id="6ff57-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="6ff57-107">Jednak nie zaleca się tego, ponieważ sprawia, że utrzymanie uprawnień bardziej skomplikowane i mylące w przyszłości.</span><span class="sxs-lookup"><span data-stu-id="6ff57-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="6ff57-108">Oto, co możesz zrobić:</span><span class="sxs-lookup"><span data-stu-id="6ff57-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="6ff57-109">Jeśli na przykład chcesz udostępnić całą zawartość folderu z wyjątkiem jednego pliku, przenieś ten plik do nowej lokalizacji, która nie jest udostępniana.</span><span class="sxs-lookup"><span data-stu-id="6ff57-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="6ff57-110">Jeśli w folderze są dwa podfoldery, a jeden podfolder chcesz udostępnić jeden podfolder grupom A i B oraz zezwolić tylko grupie A na dostęp do drugiego podfolderu, udostępnij folder nadrzędny grupie A i dodaj grupę B do pierwszego podfolderu.</span><span class="sxs-lookup"><span data-stu-id="6ff57-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="6ff57-111">Zatrzymywanie udostępniania pliku lub folderu</span><span class="sxs-lookup"><span data-stu-id="6ff57-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

