---
title: Uprawnienia interfejsu API i zgoda
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974989"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="6ad9f-102">Uprawnienia interfejsu API i zgoda</span><span class="sxs-lookup"><span data-stu-id="6ad9f-102">API permissions and consent</span></span>

<span data-ttu-id="6ad9f-103">Aplikacje, które są integrowane z platformą tożsamości firmy Microsoft, korzystają z modelu autoryzacji, który umożliwia użytkownikom i administratorom kontrolę nad sposobem uzyskiwania dostępu do danych.</span><span class="sxs-lookup"><span data-stu-id="6ad9f-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="6ad9f-104">Implementacja modelu autoryzacji została zaktualizowana w punkcie końcowym Microsoft Identity platform.</span><span class="sxs-lookup"><span data-stu-id="6ad9f-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="6ad9f-105">Zmiana sposobu, w jaki aplikacja musi współpracować z platformą Microsoft Identity.</span><span class="sxs-lookup"><span data-stu-id="6ad9f-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="6ad9f-106">[Uprawnienia i zgoda w punkcie końcowym Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) obejmują podstawowe pojęcia tego modelu autoryzacji, w tym zakresy, uprawnienia i sposób wyrażania zgody.</span><span class="sxs-lookup"><span data-stu-id="6ad9f-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="6ad9f-107">[Struktura zgody na usługę Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) ułatwia tworzenie wielodostępnych i natywnych aplikacji klienckich.</span><span class="sxs-lookup"><span data-stu-id="6ad9f-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="6ad9f-108">Te aplikacje umożliwiają logowanie się na kontach użytkowników z dzierżawy usługi Azure AD innej niż ta, w której zarejestrowano aplikację.</span><span class="sxs-lookup"><span data-stu-id="6ad9f-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="6ad9f-109">Mogą także mieć dostęp do interfejsów API sieci Web, takich jak Microsoft Graph API (Aby uzyskać dostęp do usługi Azure AD, usługi Intune i usług w systemie Microsoft 365) oraz innych interfejsów API usług firmy Microsoft, oprócz własnych interfejsów API sieci Web.</span><span class="sxs-lookup"><span data-stu-id="6ad9f-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

