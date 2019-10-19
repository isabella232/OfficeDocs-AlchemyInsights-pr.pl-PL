---
title: Ograniczanie dostępu w programie SharePoint lub OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551461"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="d66c6-102">Ograniczanie dostępu w programie SharePoint lub OneDrive</span><span class="sxs-lookup"><span data-stu-id="d66c6-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="d66c6-103">W programie SharePoint i usłudze OneDrive można ograniczyć dostęp do elementów, takich jak pliki, foldery i listy, udzielając dostępu tylko grupom lub osobom, które mają mieć dostęp.</span><span class="sxs-lookup"><span data-stu-id="d66c6-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="d66c6-104">Domyślnie uprawnienia w programie SharePoint są dziedziczone z wyższych w hierarchii.</span><span class="sxs-lookup"><span data-stu-id="d66c6-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="d66c6-105">Więc plik dziedziczy uprawnienia z folderu, który dziedziczy jego uprawnienia z biblioteki, która dziedziczy jej uprawnienia z witryny.</span><span class="sxs-lookup"><span data-stu-id="d66c6-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="d66c6-106">Można udostępnić na wyższym poziomie (na przykład przez udostępnianie całej witryny), a następnie przerwać dziedziczenie, jeśli nie chcesz udostępniać wszystkie elementy w witrynie.</span><span class="sxs-lookup"><span data-stu-id="d66c6-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="d66c6-107">Jednak nie zaleca się tego, ponieważ sprawia, że utrzymanie uprawnień bardziej skomplikowane i mylące w przyszłości.</span><span class="sxs-lookup"><span data-stu-id="d66c6-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="d66c6-108">Oto, co można zrobić zamiast:</span><span class="sxs-lookup"><span data-stu-id="d66c6-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="d66c6-109">Jeśli na przykład chcesz udostępnić całą zawartość folderu z wyjątkiem jednego pliku, Przenieś ten plik do nowej lokalizacji, która nie jest udostępniana.</span><span class="sxs-lookup"><span data-stu-id="d66c6-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="d66c6-110">Jeśli masz dwa podfoldery w folderze i chcesz udostępnić jeden podfolder grupom A i B i zezwolić tylko na dostęp do drugiego podfolderu, Udostępnij folder nadrzędny grupie A i Dodaj grupę B do pierwszego podfolderu.</span><span class="sxs-lookup"><span data-stu-id="d66c6-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="d66c6-111">Zatrzymywanie udostępniania pliku lub folderu</span><span class="sxs-lookup"><span data-stu-id="d66c6-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

