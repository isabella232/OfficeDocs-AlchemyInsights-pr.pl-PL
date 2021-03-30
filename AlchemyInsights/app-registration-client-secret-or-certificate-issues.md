---
title: Problemy z kluczem tajnym klienta rejestracji aplikacji lub certyfikatem
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
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404781"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="42a69-102">Problemy z kluczem tajnym klienta rejestracji aplikacji lub certyfikatem</span><span class="sxs-lookup"><span data-stu-id="42a69-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="42a69-103">Klucz tajny klienta aplikacji wygasa?</span><span class="sxs-lookup"><span data-stu-id="42a69-103">Application client secret expiring?</span></span>

<span data-ttu-id="42a69-104">Niezależnie od sposobu utworzenia zarejestrowanej aplikacji, czy to w ramach standardowego procesu rejestracji w portalu rejestracji aplikacji, czy też podmiot zabezpieczeń usługi został utworzony w dzierżawie przy użyciu zgody aplikacji, przed wygaśnięciem bieżącej aplikacji musi zostać utworzony nowy klucz tajny klienta i zaktualizowany w powiązanym kodzie aplikacji.</span><span class="sxs-lookup"><span data-stu-id="42a69-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="42a69-105">Maksymalny okres ważności to 2 lata.</span><span class="sxs-lookup"><span data-stu-id="42a69-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="42a69-106">Warto pamiętać, że wartość tajna musi być rejestrowana, ponieważ nie będzie już widoczna po opuszczeniu strony rejestracji aplikacji w portalu.</span><span class="sxs-lookup"><span data-stu-id="42a69-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="42a69-107">Aby uzyskać więcej informacji, zobacz [Szybki start: rejestrowanie](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) aplikacji na platformie tożsamości Firmy Microsoft i [Najlepsze rozwiązania dotyczące platformy tożsamości firmy Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="42a69-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="42a69-108">Aby dowiedzieć się więcej, [zobacz Tworzenie aplikacji Usługi Azure AD & podmiotu](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)zabezpieczeń usługi w portalu — platforma tożsamości firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="42a69-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
