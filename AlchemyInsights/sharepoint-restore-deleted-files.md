---
title: Przywracanie usuniętego pliku lub folderu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: fc560686ec5c6a3d42a97687fda80ae5001b5c60
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797558"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="f1414-102">Przywracanie usuniętego pliku lub folderu</span><span class="sxs-lookup"><span data-stu-id="f1414-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="f1414-103">W usłudze SharePoint Online kopie zapasowe wszystkich treści są przechowywane przez 14 dni po ich usunięciu.</span><span class="sxs-lookup"><span data-stu-id="f1414-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="f1414-104">Jeśli nie można przywrócić zawartości za pomocą funkcji Kosz lub Przywróć pliki, administrator może skontaktować się z działem pomocy technicznej firmy Microsoft w celu zażądania przywrócenia w dowolnym momencie w 14-dniowym oknie.</span><span class="sxs-lookup"><span data-stu-id="f1414-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="f1414-105">Przywrócenie z kopii zapasowych można wykonać tylko w przypadku zbiorów witryn lub podwitryn, a nie w przypadku konkretnych plików, list i bibliotek.</span><span class="sxs-lookup"><span data-stu-id="f1414-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="f1414-106">Po usunięciu elementu lub witryny z programu SharePoint nie jest ona natychmiast usuwana.</span><span class="sxs-lookup"><span data-stu-id="f1414-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="f1414-107">Usunięte elementy znajdują się przez pewien czas w koszu.</span><span class="sxs-lookup"><span data-stu-id="f1414-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="f1414-108">Podczas tego okresu można przywrócić usunięte elementy do ich pierwotnych lokalizacji.</span><span class="sxs-lookup"><span data-stu-id="f1414-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="f1414-109">Aby uzyskać więcej informacji, skorzystaj z poniższych linków.</span><span class="sxs-lookup"><span data-stu-id="f1414-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="f1414-110">[Przywracanie elementów w koszu witryny programu SharePoint](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span><span class="sxs-lookup"><span data-stu-id="f1414-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span></span>

[<span data-ttu-id="f1414-111">Przywracanie usuniętych plików lub folderów w usłudze OneDrive</span><span class="sxs-lookup"><span data-stu-id="f1414-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="f1414-112">Przywracanie usuniętego zbioru witryn (w tym grupy, komunikacji i innych witryn)</span><span class="sxs-lookup"><span data-stu-id="f1414-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="f1414-113">Przywracanie usuniętej witryny usługi OneDrive</span><span class="sxs-lookup"><span data-stu-id="f1414-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="f1414-114">W przypadku akcji funkcji Kosz zbiorczy Administratorzy mogą rozważyć użycie usługi [SharePoint Online PnP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="f1414-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="f1414-115">**Funkcja przywracania plików**</span><span class="sxs-lookup"><span data-stu-id="f1414-115">**Files Restore feature**</span></span>

<span data-ttu-id="f1414-116">Jeśli wiele plików usługi OneDrive lub programu SharePoint zostanie usuniętych, zastąpionych, uszkodzonych lub zainfekowanych przez złośliwe oprogramowanie, można przywrócić całą całą bibliotekę usługi OneDrive lub programu SharePoint, korzystając z funkcji przywracania plików.</span><span class="sxs-lookup"><span data-stu-id="f1414-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="f1414-117">Przywracanie biblioteki usługi OneDrive</span><span class="sxs-lookup"><span data-stu-id="f1414-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="f1414-118">Przywracanie biblioteki dokumentów</span><span class="sxs-lookup"><span data-stu-id="f1414-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

