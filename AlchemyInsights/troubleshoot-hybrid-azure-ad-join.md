---
title: Rozwiązywanie problemów z dołączeniem hybrydowym do usługi Microsoft Azure Active Directory
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401917"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="e50d1-102">Rozwiązywanie problemów z dołączeniem hybrydowym do usługi Microsoft Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="e50d1-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="e50d1-103">Zdecydowanie zalecane: upewnij się, że urządzenie może uzyskać dostęp do punktów końcowych usługi Device Registration w ramach konta systemowego przy użyciu [skryptu Testowanie łączności rejestracji urządzeń](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span><span class="sxs-lookup"><span data-stu-id="e50d1-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="e50d1-104">Jeśli po raz pierwszy konfigurujesz rejestracje urządzeń, upewnij się, że przejrzany został artykuł W[prowadzenie do zarządzania urządzeniami w usłudze Microsoft Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/), aby dowiedzieć się, w jaki sposób kontrolować urządzenia w usłudze Microsoft Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e50d1-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="e50d1-105">Jeśli rejestrujesz urządzenia bezpośrednio w usłudze Microsoft Azure Active Directory i zapisujesz je w usłudze Intune, upewnij się najpierw, że [usługa Intune jest skonfigurowana](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) i posiada [licencjonowanie](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="e50d1-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="e50d1-106">Upewnij się, że masz uprawnienia do wykonywania operacji w usłudze Microsoft Azure Active Directory i lokalnej usłudze Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e50d1-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="e50d1-107">Tylko administrator globalny w usłudze Microsoft Azure Active Directory może zarządzać ustawieniami w przypadku rejestracji urządzeń.</span><span class="sxs-lookup"><span data-stu-id="e50d1-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="e50d1-108">Jeśli dodatkowo konfigurujesz automatyczne rejestracje w lokalnej usłudze Active Directory, musisz być administratorem usługi Active Directory i usług federacyjnych Active Directory (o ile mają zastosowanie).</span><span class="sxs-lookup"><span data-stu-id="e50d1-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="e50d1-109">W celu uzyskania więcej informacji szczegółowych na temat rozwiązywania potencjalnych problemów, zobacz artykuł [Rozwiązywanie problemów z dołączeniem hybrydowym](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) w zakresie konfiguracji przyłączonej hybrydowo do usługi Azure AD, a w przypadku Zarządzania urządzeniami przy użyciu portalu usługi Azure AD, zobacz [Konfigurowanie urządzeń przyłączonych hybrydowo do usługi Azure AD (przyłączonych do domeny lokalnej)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) i [Zarządzanie urządzeniami przy użyciu Azure Portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="e50d1-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="e50d1-110">Aby rozwiązać typowe problemy z dołączaniem hybrydowym do usługi Microsoft Azure Active Directory, zobacz [Dołączanie hybrydowe do usługi Azure AD — często zadawane pytania](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="e50d1-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
