---
title: Notification AAD Connect
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037230"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="a2621-102">Notification AAD Connect</span><span class="sxs-lookup"><span data-stu-id="a2621-102">Notification AAD Connect</span></span>

- <span data-ttu-id="a2621-103">Upewnij się, że masz upoważnienie do wykonania operacji.</span><span class="sxs-lookup"><span data-stu-id="a2621-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="a2621-104">Administratorzy globalni mają domyślnie dostęp.</span><span class="sxs-lookup"><span data-stu-id="a2621-104">Global Admins have access by default.</span></span> <span data-ttu-id="a2621-105">Ponadto możesz użyć kontroli dostępu opartej na rolach, [aby](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) delegować uprawnienia rejestracji do współautora.</span><span class="sxs-lookup"><span data-stu-id="a2621-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="a2621-106">Upewnij się, że wymagane punkty końcowe są włączone i nie są blokowane z powodu zapory.</span><span class="sxs-lookup"><span data-stu-id="a2621-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="a2621-107">Aby uzyskać szczegółowe informacje, zobacz [wymagania.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="a2621-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="a2621-108">Rejestracja może zakończyć się niepowodzeniem, ponieważ komunikacja wychodząca jest poddawana inspekcji SSL przez warstwę sieciową.</span><span class="sxs-lookup"><span data-stu-id="a2621-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="a2621-109">Upewnij się, że zostały zweryfikowane ustawienia powiadomień dotyczące usługi Azure AD Connect Health, i sprawdź ustawienia.</span><span class="sxs-lookup"><span data-stu-id="a2621-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="a2621-110">Aby dowiedzieć się, jak skonfigurować ustawienia powiadomień dla powiadomień usługi Azure AD Connect Health, zobacz ten [przewodnik.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)</span><span class="sxs-lookup"><span data-stu-id="a2621-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="a2621-111">Aby dowiedzieć się więcej na temat raportu synchronizacji usługi AAD Connect Health i sposobu jego pobierania, zobacz Raport [synchronizacji na poziomie obiektów.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="a2621-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="a2621-112">Aby rozwiązać problemy z alertami kondycji usługi AAD Connect, postępuj zgodnie z instrukcje rozwiązywania problemów dotyczące alertów o odświeżeń danych [aAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) oraz w przypadku często zadawanego pytania, zobacz Typowe pytania dotyczące instalacji usługi [AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="a2621-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
