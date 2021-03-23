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
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Rozwiązywanie problemów z kodami błędów uwierzytelniania i autoryzacji usługi Azure AD (AADSTS)

Aby rozwiązać problemy z kodami błędów uwierzytelniania i autoryzacji usługi AAD (AADSTS), wykonaj następujące zalecane czynności:

1. **Obsługa kodów błędów w aplikacji**

- Specyfikacja **OAuth2.0**, zawiera wskazówki dotyczące obsługi błędów podczas uwierzytelniania przy użyciu części odpowiedzi na https://tools.ietf.org/html/rfc6749#section-5.2 błąd.

    - **błąd:** Ciąg kodu błędu, który może być używany do klasyfikowania typów błędów, które występują, i który należy stosować w celu reagowania na błędy.
    - Pole **błędu** zawiera kilka możliwych wartości — zapoznaj się z linkami do dokumentacji protokołu i specyfikacjami protokołu OAuth 2.0, aby uzyskać więcej informacji na temat konkretnych błędów i sposobu reakcji na nie.

- Oto przykładowa odpowiedź o błędzie:
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
2. **Odnośnik bieżących informacji o kodzie błędu**

- Kody błędów i komunikaty mogą ulec zmianie. Aby uzyskać najnowsze informacje, zobacz stronę, aby znaleźć opisy błędów AADSTS, poprawki i niektóre https://login.microsoftonline.com/error sugerowane obejścia.
- Możesz również wyszukiwać i rozwiązywać problemy z kodami błędów [AADSTS wymienionymi](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) w artykule Kody błędów uwierzytelniania i autoryzacji [usługi Azure AD.](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)

3. **Uzyskiwanie pomocy**

- [Opcje pomocy technicznej](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) i pomocy dla deweloperów — jeśli potrzebujesz odpowiedzi na pytanie lub pomocy w rozwiązaniu problemu, który nie został przez nas zasypany w naszej dokumentacji, może być na czas, aby zasięgnąć pomocy ekspertów. W tym artykule przedstawiono kilka sugestii dotyczących uzyskiwania odpowiedzi na pytania podczas opracowywania aplikacji integrych z platformą tożsamości firmy Microsoft.








