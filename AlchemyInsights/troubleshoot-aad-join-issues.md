---
title: Rozwiązywanie problemów z dołączaniem do usługi Azure AD
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405132"
---
# <a name="troubleshoot-azure-ad-join-issues"></a><span data-ttu-id="a020a-102">Rozwiązywanie problemów z dołączaniem do usługi Azure AD</span><span class="sxs-lookup"><span data-stu-id="a020a-102">Troubleshoot Azure AD join issues</span></span>

1. <span data-ttu-id="a020a-103">Jeśli używasz rejestracji urządzeń po raz pierwszy, sprawdź wprowadzenie do zarządzania urządzeniami w usłudze [Azure Active Directory,](https://docs.microsoft.com/azure/active-directory/devices/overview) które zawiera wskazówki dotyczące sposobu kontrolowania przez urządzenia usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a020a-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="a020a-104">Jeśli rejestrujesz urządzenia bezpośrednio w usłudze Azure AD i zapisujesz je w usłudze Intune, musisz najpierw upewnić się, że skonfigurowano usługę [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) i że w pierwszej kolejności są [one](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) stosowane.</span><span class="sxs-lookup"><span data-stu-id="a020a-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="a020a-105">Upewnij się, że masz uprawnienia do wykonywania operacji w usłudze Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a020a-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="a020a-106">Tylko administrator globalny w usłudze Azure AD może zarządzać ustawieniami rejestracji urządzeń.</span><span class="sxs-lookup"><span data-stu-id="a020a-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="a020a-107">Aby wykonać implementację dołączania do usługi Azure AD, zobacz [Planowanie dołączenia do usługi Azure AD.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)</span><span class="sxs-lookup"><span data-stu-id="a020a-107">To do Azure AD join implementation, see [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="a020a-108">Aby uzyskać więcej szczegółowych informacji na temat rozwiązywania typowych problemów dotyczących dołączania do usługi Azure AD, zobacz Często zadawane pytania dotyczące dołączania do usługi [Azure Ad,](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) a w przypadku urządzeń z systemem Windows 10 Pro zobacz Nie można dołączyć komputera z systemem [Windows 10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) do usługi Azure AD — konieczność uaktualnienia do — Microsoft Community</span><span class="sxs-lookup"><span data-stu-id="a020a-108">For more details on resolving  common issues with Azure AD join see [Azure Ad Join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span></span>
