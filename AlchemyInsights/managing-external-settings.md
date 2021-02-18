---
title: Zarządzanie ustawieniami zewnętrznymi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294313"
---
# <a name="managing-external-settings"></a><span data-ttu-id="15563-102">Zarządzanie ustawieniami zewnętrznymi</span><span class="sxs-lookup"><span data-stu-id="15563-102">Managing External Settings</span></span>

<span data-ttu-id="15563-103">**Ogłoszenie**</span><span class="sxs-lookup"><span data-stu-id="15563-103">**Announcement**</span></span>

- <span data-ttu-id="15563-104">[Od 4 stycznia 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support)r. firma Google wyloguje obsługę logowania WebView.</span><span class="sxs-lookup"><span data-stu-id="15563-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="15563-105">Sprawdź, czy na Twoje aplikacje mają wpływ wytyczne firmy Google dotyczące testowania zgodności</span><span class="sxs-lookup"><span data-stu-id="15563-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="15563-106">Korzystanie z funkcji System WebView lub przeglądarki systemowej podczas logowania się do użytkowników za pomocą kont Google dla klientów indywidualnych</span><span class="sxs-lookup"><span data-stu-id="15563-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="15563-107">**Zarządzanie ustawieniami zaproszenia**</span><span class="sxs-lookup"><span data-stu-id="15563-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="15563-108">Upewnij się, że ustawienia współpracy zewnętrznej zostały skonfigurowane [w](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) celu umożliwienia odpowiednim osobom wysyłania zaproszeń.</span><span class="sxs-lookup"><span data-stu-id="15563-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="15563-109">**Zarządzanie uprawnieniami dostępu użytkownika gościa**</span><span class="sxs-lookup"><span data-stu-id="15563-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="15563-110">Administratorzy globalni mogą zarządzać uprawnieniami dostępu gości w katalogu za pośrednictwem portalu Azure Portal, konfigurując uprawnienia dostępu gościa na stronie Ustawienia współpracy zewnętrznej.</span><span class="sxs-lookup"><span data-stu-id="15563-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="15563-111">[Dowiedz się więcej o tym ustawieniu.](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="15563-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="15563-112">Jeśli chcesz, aby goście mieli dostęp do aplikacji, takich jak Teams lub SharePoint, potwierdź, że te aplikacje zostały skonfigurowane tak, aby zezwalały na dostęp gości.</span><span class="sxs-lookup"><span data-stu-id="15563-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="15563-113">Dowiedz się więcej o [ustawieniach aplikacji Teams i](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) [programie SharePoint.](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="15563-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="15563-114">**Konfigurowanie zaproszeń:**</span><span class="sxs-lookup"><span data-stu-id="15563-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="15563-115">Włączanie współpracy zewnętrznej B2B i zarządzanie tym, kto może zapraszać gości</span><span class="sxs-lookup"><span data-stu-id="15563-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="15563-116">Zezwalanie na zaproszenia do użytkowników z określonych organizacji lub blokowanie ich</span><span class="sxs-lookup"><span data-stu-id="15563-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="15563-117">**Konfigurowanie dozwolonych dostawców tożsamości:**</span><span class="sxs-lookup"><span data-stu-id="15563-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="15563-118">Federacja Google</span><span class="sxs-lookup"><span data-stu-id="15563-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="15563-119">Federacja bezpośrednia</span><span class="sxs-lookup"><span data-stu-id="15563-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="15563-120">Uwierzytelnianie za pomocą adresu e-mail z kodem dostępu w wiadomości e-mail</span><span class="sxs-lookup"><span data-stu-id="15563-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
