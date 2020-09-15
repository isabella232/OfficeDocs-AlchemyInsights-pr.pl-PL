---
title: Odmowa dostępu podczas mapowania dysku do programu SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 8fc866390d63443c94beef76b6a53a628b85d6d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668753"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="2e1dc-102">Rozwiązywanie problemów z bibliotekami programu SharePoint zamapowanymi na dyski sieciowe</span><span class="sxs-lookup"><span data-stu-id="2e1dc-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="2e1dc-103">Po przejściu do zmapowanego dysku sieciowego może zostać wyświetlony dowolny z następujących komunikatów:</span><span class="sxs-lookup"><span data-stu-id="2e1dc-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="2e1dc-104">**\\Ścieżka jest niedostępna. Być może nie masz uprawnień do korzystania z tego zasobu sieciowego. Skontaktuj się z administratorem tego serwera, aby dowiedzieć się, czy masz uprawnienia dostępu.**</span><span class="sxs-lookup"><span data-stu-id="2e1dc-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="2e1dc-105">**Odmowa dostępu. Przed otwarciem plików w tej lokalizacji musisz najpierw dodać witrynę sieci Web do listy zaufanych witryn, przejść do witryny sieci Web i wybrać opcję logowania automatycznego.**</span><span class="sxs-lookup"><span data-stu-id="2e1dc-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="2e1dc-106">[Uzyskaj pomoc w rozwiązywaniu problemów z zmapowanymi dyskami sieciowymi](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="2e1dc-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="2e1dc-107">Mapowanie biblioteki jako dysku sieciowego jest tymczasowe i obsługiwane tylko w programie Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="2e1dc-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="2e1dc-108">Zamiast tego [Zsynchronizuj pliki programu SharePoint za pomocą nowego klienta synchronizacji usługi OneDrive](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) , który obejmuje [pliki na żądanie](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span><span class="sxs-lookup"><span data-stu-id="2e1dc-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="2e1dc-109">Uzyskiwanie dostępu do wszystkich plików w usłudze OneDrive bez korzystania z lokalnego miejsca do magazynowania.</span><span class="sxs-lookup"><span data-stu-id="2e1dc-109">Access all your files in OneDrive without using local storage space.</span></span>
  