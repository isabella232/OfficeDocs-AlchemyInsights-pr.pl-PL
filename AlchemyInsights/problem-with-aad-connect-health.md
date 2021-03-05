---
title: Problem z kondycją połączenia AAD
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482073"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="35517-102">Problem z kondycją połączenia AAD</span><span class="sxs-lookup"><span data-stu-id="35517-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="35517-103">Upewnij się, że masz upoważnienie do wykonywania operacji.</span><span class="sxs-lookup"><span data-stu-id="35517-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="35517-104">Administratorzy globalni mają domyślnie dostęp.</span><span class="sxs-lookup"><span data-stu-id="35517-104">Global Admins have access by default.</span></span> <span data-ttu-id="35517-105">Ponadto możesz użyć kontroli dostępu opartej na rolach, [aby](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) delegować uprawnienia rejestracji do współautora.</span><span class="sxs-lookup"><span data-stu-id="35517-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="35517-106">Upewnij się, że wymagane punkty końcowe są włączone i nie są blokowane z powodu zapory.</span><span class="sxs-lookup"><span data-stu-id="35517-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="35517-107">Aby uzyskać szczegółowe informacje, zobacz [wymagania.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="35517-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="35517-108">Rejestracja może zakończyć się niepowodzeniem ze względu na to, że komunikacja wychodząca podlega inspekcji SSL przez warstwę sieciową.</span><span class="sxs-lookup"><span data-stu-id="35517-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="35517-109">Upewnij się, że ustawienia powiadomień dotyczące usługi Azure AD Connect Health zostały zweryfikowane.</span><span class="sxs-lookup"><span data-stu-id="35517-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="35517-110">Sprawdź swoje ustawienia.</span><span class="sxs-lookup"><span data-stu-id="35517-110">Please review your setting.</span></span> <span data-ttu-id="35517-111">Ten [przewodnik](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) może ułatwić ci skonfigurowanie ustawień powiadomień dotyczących powiadomień dotyczących kondycji usługi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="35517-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="35517-112">Aby dowiedzieć się więcej na temat raportu synchronizacji usługi AAD Connect Health i sposobu jego pobierania, zobacz raport synchronizacji [na poziomie obiektu.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="35517-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="35517-113">Aby rozwiązać problemy z alertami kondycji usługi AAD Connect, skorzystaj z przewodnika po rozwiązywaniu problemów dla alertów o odświeżaniu danych [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) oraz w przypadku często zadawanego pytania, zobacz typowe pytania dotyczące instalacji [usługi AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="35517-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
