---
title: Problemy z zgodą administratora
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901507"
---
# <a name="admin-consent-issues"></a>Problemy z zgodą administratora

1. Włącz [przepływ pracy](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) zatwierdzanie przez administratora, aby zezwolić użytkownikom na żądanie zatwierdzenia administratora bezpośrednio z ekranu zgody.

1. Jeśli w trakcie procesu wyrażania zgody użytkownik lub Użytkownicy aplikacji widzą nieoczekiwane błędy, zobacz ten artykuł, aby uzyskać informacje dotyczące rozwiązywania problemów: [nieoczekiwany błąd podczas wykonywania zgody na aplikację](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Dowiedz się więcej [na temat zgody administratora na platformie Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), sposobu działania [monitu o zgodę](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) i sposobu [oceny prośby o zgodę na administratora dzierżawy](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).

1. Aplikacje, które są integrowane z platformą tożsamości firmy Microsoft, korzystają z modelu autoryzacji, który umożliwia użytkownikom i administratorom kontrolę nad sposobem uzyskiwania dostępu do danych. Implementacja modelu autoryzacji została zaktualizowana w punkcie końcowym Microsoft Identity platform i zmienia sposób interakcji aplikacji z platformą Microsoft Identity platform. Zobacz [uprawnienia i wyrażanie zgody w punkcie końcowym Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) , aby zapoznać się z omówieniem tego modelu autoryzacji, w tym z zakresami, uprawnieniami i zgodą.