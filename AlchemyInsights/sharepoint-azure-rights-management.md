---
title: Ograniczanie dostępu w programie SharePoint lub usłudze OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: cc6f93ba8ae3a030f83da5eca2d28dcf38f0f8f7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47800906"
---
# <a name="irm-protection-to-sharepoint-files"></a><span data-ttu-id="e7ff0-102">Ochrona plików programu SharePoint za pomocą usługi IRM</span><span class="sxs-lookup"><span data-stu-id="e7ff0-102">IRM Protection to SharePoint files</span></span>


<span data-ttu-id="e7ff0-103">W usłudze SharePoint Online ochrona za pomocą funkcji IRM jest stosowana do plików na poziomie listy i biblioteki.</span><span class="sxs-lookup"><span data-stu-id="e7ff0-103">Within SharePoint Online, IRM protection is applied to files at the list and library level.</span></span> <span data-ttu-id="e7ff0-104">Zanim Twoja organizacja będzie mogła korzystać z ochrony IRM, musisz najpierw skonfigurować zarządzanie prawami.</span><span class="sxs-lookup"><span data-stu-id="e7ff0-104">Before your organization can use IRM protection, you must first set up Rights Management.</span></span> <span data-ttu-id="e7ff0-105">Usługa IRM korzysta z usługi Azure Rights Management w usłudze Azure Information Protection do szyfrowania i przypisywania ograniczeń użytkowania.</span><span class="sxs-lookup"><span data-stu-id="e7ff0-105">IRM relies on the Azure Rights Management service from Azure Information Protection to encrypt and assign usage restrictions.</span></span> <span data-ttu-id="e7ff0-106">Niektóre subskrypcje usługi Microsoft 365 obejmują usługę Azure Rights Management, ale nie wszystkie.</span><span class="sxs-lookup"><span data-stu-id="e7ff0-106">Some Microsoft 365 subscriptions include Azure Rights Management, but not all.</span></span> 

<span data-ttu-id="e7ff0-107">Aby dowiedzieć się więcej, zobacz:</span><span class="sxs-lookup"><span data-stu-id="e7ff0-107">To learn more, see:</span></span>

- <span data-ttu-id="e7ff0-108">[Jak aplikacje i usługi pakietu Office obsługują usługę Azure Rights Management](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support).</span><span class="sxs-lookup"><span data-stu-id="e7ff0-108">[How Office applications and services support Azure Rights Management](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support).</span></span>

- <span data-ttu-id="e7ff0-109">[Konfigurowanie usługi Zarządzanie prawami do informacji (IRM) w centrum administracyjnym programu SharePoint](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center).</span><span class="sxs-lookup"><span data-stu-id="e7ff0-109">[Set up Information Rights Management (IRM) in SharePoint admin center](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center).</span></span>

- <span data-ttu-id="e7ff0-110">[IRM-umożliwia włączanie bibliotek dokumentów i list programu SharePoint](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists).</span><span class="sxs-lookup"><span data-stu-id="e7ff0-110">[IRM-enable SharePoint document libraries and lists](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists).</span></span>

- <span data-ttu-id="e7ff0-111">[Zarządzanie prawami do informacji w pakiecie Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c).</span><span class="sxs-lookup"><span data-stu-id="e7ff0-111">[Information Rights Management in Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c).</span></span>

- <span data-ttu-id="e7ff0-112">[Zarządzanie prawami do informacji w usłudze Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/information-rights-management-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="e7ff0-112">[Information Rights Management in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/information-rights-management-in-exchange-online).</span></span>


