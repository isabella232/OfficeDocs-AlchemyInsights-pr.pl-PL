---
title: Rozwiązywanie problemów z błędem 404, nie znaleziono pliku
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 1b15444c-367b-4523-8e08-1c77bbea7524
ms.openlocfilehash: e76864949bde7230e63f509823ab1e3edf631388
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750101"
---
# <a name="troubleshoot-error-404-file-not-found"></a><span data-ttu-id="83375-102">Rozwiązywanie problemów z błędem 404, nie znaleziono pliku</span><span class="sxs-lookup"><span data-stu-id="83375-102">Troubleshoot Error 404, File not found</span></span>

<span data-ttu-id="83375-103">Gdy użytkownicy próbują uzyskać dostęp do witryny lub pliku w programie SharePoint lub usłudze OneDrive, zostanie odebrany błąd 404.</span><span class="sxs-lookup"><span data-stu-id="83375-103">An Error 404 is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="83375-104">Jest to często spowodowane tym, że witryna lub plik lub grupa są w nich dodawane, przenoszone lub usuwane.</span><span class="sxs-lookup"><span data-stu-id="83375-104">This is often caused by a site or file or group getting renamed, moved or deleted.</span></span> <span data-ttu-id="83375-105">Na przykład: użytkownicy będą mieli błąd 404 podczas próby uzyskania dostępu do głównego zbioru witryn i został on usunięty.</span><span class="sxs-lookup"><span data-stu-id="83375-105">For example: Users will experience a 404 Error attempting to access the Root Site Collection and it has been deleted.</span></span>

<span data-ttu-id="83375-106">Aby wyeliminować błąd 404 dla witryny, której nazwa została zmieniona, została przeniesiona lub usunięta:</span><span class="sxs-lookup"><span data-stu-id="83375-106">To resolve Error 404 for a Site that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="83375-107">W przypadku klasycznych witryn, które znajdują się w klasycznym centrum administracyjnym, zobacz [Przywracanie usuniętego zbioru witryn](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span><span class="sxs-lookup"><span data-stu-id="83375-107">For classic sites that exist in the Classic Admin Center, see [Restore a deleted site collection](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="83375-108">W przypadku witryn nowoczesnych (komunikacji, grupowych i innych witryn) istniejących w nowym centrum administracyjnym programu SharePoint zobacz [Wyświetlanie i przywracanie usuniętych witryn w nowym centrum administracyjnym programu SharePoint](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span><span class="sxs-lookup"><span data-stu-id="83375-108">For modern sites (communication, group-connected, or other sites) that exist in the new SharePoint admin center, see [View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="83375-109">Aby wyeliminować błąd 404 dotyczący pliku (lub innego elementu), którego nazwa została zmieniona, przeniesiony lub usunięty:</span><span class="sxs-lookup"><span data-stu-id="83375-109">To resolve Error 404 for a File (or other item) that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="83375-110">Przejdź do witryny programu SharePoint lub usługi OneDrive i Wyświetl kosz z zawartości witryny.</span><span class="sxs-lookup"><span data-stu-id="83375-110">Go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span> <span data-ttu-id="83375-111">Zobacz [przywracanie elementów w koszu witryny programu SharePoint](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span><span class="sxs-lookup"><span data-stu-id="83375-111">See, [Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span></span>

<span data-ttu-id="83375-112">Jeśli nadal nie możesz znaleźć elementu, który można przeszukać w dzienniku inspekcji, jeśli rejestrowanie jest włączone Zobacz, [Przeszukaj dziennik inspekcji w centrum zabezpieczeń programu Microsoft 365 Security &](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="83375-112">If you are still unable to find the item you can search the audit log if logging is enabled see, [Search the audit log in the Microsoft 365 Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>
