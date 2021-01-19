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
# <a name="admin-consent-issues"></a><span data-ttu-id="ed129-102">Problemy z zgodą administratora</span><span class="sxs-lookup"><span data-stu-id="ed129-102">Admin consent issues</span></span>

1. <span data-ttu-id="ed129-103">Włącz [przepływ pracy](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) zatwierdzanie przez administratora, aby zezwolić użytkownikom na żądanie zatwierdzenia administratora bezpośrednio z ekranu zgody.</span><span class="sxs-lookup"><span data-stu-id="ed129-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="ed129-104">Jeśli w trakcie procesu wyrażania zgody użytkownik lub Użytkownicy aplikacji widzą nieoczekiwane błędy, zobacz ten artykuł, aby uzyskać informacje dotyczące rozwiązywania problemów: [nieoczekiwany błąd podczas wykonywania zgody na aplikację](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="ed129-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="ed129-105">Dowiedz się więcej [na temat zgody administratora na platformie Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), sposobu działania [monitu o zgodę](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) i sposobu [oceny prośby o zgodę na administratora dzierżawy](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="ed129-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="ed129-106">Aplikacje, które są integrowane z platformą tożsamości firmy Microsoft, korzystają z modelu autoryzacji, który umożliwia użytkownikom i administratorom kontrolę nad sposobem uzyskiwania dostępu do danych.</span><span class="sxs-lookup"><span data-stu-id="ed129-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="ed129-107">Implementacja modelu autoryzacji została zaktualizowana w punkcie końcowym Microsoft Identity platform i zmienia sposób interakcji aplikacji z platformą Microsoft Identity platform.</span><span class="sxs-lookup"><span data-stu-id="ed129-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="ed129-108">Zobacz [uprawnienia i wyrażanie zgody w punkcie końcowym Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) , aby zapoznać się z omówieniem tego modelu autoryzacji, w tym z zakresami, uprawnieniami i zgodą.</span><span class="sxs-lookup"><span data-stu-id="ed129-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>