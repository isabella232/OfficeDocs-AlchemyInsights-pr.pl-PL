---
title: Dołączanie do usługi Azure Active Directory
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
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405053"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="a616f-102">Dołączanie do usługi Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="a616f-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="a616f-103">Jeśli używasz rejestracji urządzeń po raz pierwszy, sprawdź wprowadzenie do zarządzania urządzeniami w usłudze [Azure Active Directory,](/azure/active-directory/devices/overview) które zawiera wskazówki dotyczące sposobu kontrolowania przez urządzenia usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a616f-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="a616f-104">Jeśli rejestrujesz urządzenia bezpośrednio w usłudze Azure AD i zapisujesz je w usłudze Intune, musisz najpierw upewnić się, że skonfigurowano usługę [Intune](/mem/intune/enrollment/device-enrollment) i że w pierwszej kolejności są [one](/mem/intune/fundamentals/licenses-assign) stosowane.</span><span class="sxs-lookup"><span data-stu-id="a616f-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="a616f-105">Upewnij się, że masz uprawnienia do wykonywania operacji w usłudze Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a616f-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="a616f-106">Tylko administrator globalny w usłudze Azure AD może zarządzać ustawieniami rejestracji urządzeń.</span><span class="sxs-lookup"><span data-stu-id="a616f-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="a616f-107">Aby wykonać implementację dołączania do usługi Azure AD, zobacz [Planowanie dołączenia do usługi Azure AD.](/azure/active-directory/devices/azureadjoin-plan)</span><span class="sxs-lookup"><span data-stu-id="a616f-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="a616f-108">Aby uzyskać więcej szczegółowych informacji na temat rozwiązywania typowych problemów dotyczących dołączania do usługi Azure AD, zobacz Często zadawane pytania dotyczące dołączania do usługi [Azure Ad,](/azure/active-directory/devices/faq) a w przypadku urządzeń z systemem Windows 10 Pro zobacz Nie można dołączyć komputera z systemem [Windows 10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)do usługi Azure AD — musisz uaktualnić do — Społeczność firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a616f-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>
