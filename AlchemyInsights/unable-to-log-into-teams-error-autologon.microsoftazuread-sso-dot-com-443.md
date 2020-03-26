---
title: Nie można zalogować się do usługi Teams z powodu błędu autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932036"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="91305-102">Nie można zalogować się do usługi Teams z powodu błędu autologon.microsoftazuread-sso kropka com:443</span><span class="sxs-lookup"><span data-stu-id="91305-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="91305-103">Jeśli w uwierzytelnianiu usługi Office 365 jest włączone bezproblemowe logowanie jednokrotne, może być konieczne dodanie adresu URL „autologon.microsoftazuread-sso.com” do witryn intranetowych.</span><span class="sxs-lookup"><span data-stu-id="91305-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="91305-104">Jeśli został on wcześniej dodany do zaufanych witryn i jest używane bezproblemowe logowanie jednokrotne, należy usunąć go z witryn zaufanych.</span><span class="sxs-lookup"><span data-stu-id="91305-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="91305-105">Zapoznaj się z [listą kontrolną rozwiązywania problemów bezproblemowego logowania jednokrotnego](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="91305-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="91305-106">Wykonaj poniższe czynności, aby dodać adres URL do listy witryn intranetowych:</span><span class="sxs-lookup"><span data-stu-id="91305-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="91305-107">Otwórz program Internet Explorer, klikając przycisk **Start**.</span><span class="sxs-lookup"><span data-stu-id="91305-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="91305-108">W polu wyszukiwania wpisz ciąg Internet Explorer, a następnie na liście wyników kliknij pozycję **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="91305-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="91305-109">Kliknij pozycję **Narzędzia**, a następnie kliknij pozycję **Opcje internetowe**.</span><span class="sxs-lookup"><span data-stu-id="91305-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="91305-110">Kliknij kartę **Zabezpieczenia**.</span><span class="sxs-lookup"><span data-stu-id="91305-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="91305-111">Kliknij teraz pozycję **Lokalne witryny intranetowe**, po czym kliknij przycisk **witryny**, a następnie przycisk **Zaawansowane**.</span><span class="sxs-lookup"><span data-stu-id="91305-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="91305-112">Wprowadź adres URL witryny internetowej, a następnie kliknij pozycję **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="91305-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="91305-113">Po zakończeniu kliknij przycisk **Zamknij**.</span><span class="sxs-lookup"><span data-stu-id="91305-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="91305-114">Aby uzyskać więcej informacji, zobacz [Dokumentację wdrażania bezproblemowego logowania jednokrotnego w usłudze Office 365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (obejmuje oparty na zasadach proces dodawania adresu URL do witryn intranetowych w kroku 3).</span><span class="sxs-lookup"><span data-stu-id="91305-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
