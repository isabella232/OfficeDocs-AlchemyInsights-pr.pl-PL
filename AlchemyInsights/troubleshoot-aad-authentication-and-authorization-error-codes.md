---
title: Rozwiązywanie problemów z kodami błędów uwierzytelniania i autoryzacji usługi Azure AD (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037845"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="b73ee-102">Rozwiązywanie problemów z kodami błędów uwierzytelniania i autoryzacji usługi Azure AD (AADSTS)</span><span class="sxs-lookup"><span data-stu-id="b73ee-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="b73ee-103">Aby rozwiązać problemy z kodami błędów uwierzytelniania i autoryzacji usługi AAD (AADSTS), wykonaj następujące zalecane czynności:</span><span class="sxs-lookup"><span data-stu-id="b73ee-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="b73ee-104">**Obsługa kodów błędów w aplikacji**</span><span class="sxs-lookup"><span data-stu-id="b73ee-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="b73ee-105">Specyfikacja **OAuth2.0**, zawiera wskazówki dotyczące obsługi błędów podczas uwierzytelniania przy użyciu części odpowiedzi na https://tools.ietf.org/html/rfc6749#section-5.2 błąd.</span><span class="sxs-lookup"><span data-stu-id="b73ee-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="b73ee-106">**błąd:** Ciąg kodu błędu, który może być używany do klasyfikowania typów błędów, które występują, i który należy stosować w celu reagowania na błędy.</span><span class="sxs-lookup"><span data-stu-id="b73ee-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="b73ee-107">Pole **błędu** zawiera kilka możliwych wartości — zapoznaj się z linkami do dokumentacji protokołu i specyfikacjami protokołu OAuth 2.0, aby uzyskać więcej informacji na temat konkretnych błędów i sposobu reakcji na nie.</span><span class="sxs-lookup"><span data-stu-id="b73ee-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="b73ee-108">Oto przykładowa odpowiedź o błędzie:</span><span class="sxs-lookup"><span data-stu-id="b73ee-108">Here is a sample error response:</span></span>
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. <span data-ttu-id="b73ee-109">**Odnośnik bieżących informacji o kodzie błędu**</span><span class="sxs-lookup"><span data-stu-id="b73ee-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="b73ee-110">Kody błędów i komunikaty mogą ulec zmianie.</span><span class="sxs-lookup"><span data-stu-id="b73ee-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="b73ee-111">Aby uzyskać najnowsze informacje, zobacz stronę, aby znaleźć opisy błędów AADSTS, poprawki i niektóre https://login.microsoftonline.com/error sugerowane obejścia.</span><span class="sxs-lookup"><span data-stu-id="b73ee-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="b73ee-112">Możesz również wyszukiwać i rozwiązywać problemy z kodami błędów [AADSTS wymienionymi](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) w artykule Kody błędów uwierzytelniania i autoryzacji [usługi Azure AD.](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)</span><span class="sxs-lookup"><span data-stu-id="b73ee-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="b73ee-113">**Uzyskiwanie pomocy**</span><span class="sxs-lookup"><span data-stu-id="b73ee-113">**Get Help**</span></span>

- <span data-ttu-id="b73ee-114">[Opcje pomocy technicznej](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) i pomocy dla deweloperów — jeśli potrzebujesz odpowiedzi na pytanie lub pomocy w rozwiązaniu problemu, który nie został przez nas zasypany w naszej dokumentacji, może być na czas, aby zasięgnąć pomocy ekspertów.</span><span class="sxs-lookup"><span data-stu-id="b73ee-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="b73ee-115">W tym artykule przedstawiono kilka sugestii dotyczących uzyskiwania odpowiedzi na pytania podczas opracowywania aplikacji integrych z platformą tożsamości firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b73ee-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








