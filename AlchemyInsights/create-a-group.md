---
title: Tworzenie grupy
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816367"
---
# <a name="create-a-group"></a><span data-ttu-id="6c34b-102">Tworzenie grupy</span><span class="sxs-lookup"><span data-stu-id="6c34b-102">Create a group</span></span>

<span data-ttu-id="6c34b-103">W tym temacie opisano tworzenie grup.</span><span class="sxs-lookup"><span data-stu-id="6c34b-103">This topic describes group creation.</span></span>

<span data-ttu-id="6c34b-104">**Uprawnienie do tworzenia grupy**</span><span class="sxs-lookup"><span data-stu-id="6c34b-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="6c34b-105">Upewnij się, że masz upoważnienie do tworzenia nowej grupy.</span><span class="sxs-lookup"><span data-stu-id="6c34b-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="6c34b-106">Administratorzy globalni mogą wyłączyć tworzenie grup w Portalu Azure lub panelu dostępu.</span><span class="sxs-lookup"><span data-stu-id="6c34b-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="6c34b-107">Administrator może utworzyć nową grupę lub nadać Ci odpowiednie uprawnienia.</span><span class="sxs-lookup"><span data-stu-id="6c34b-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="6c34b-108">**Zarządzanie uprawnieniami do tworzenia grup**</span><span class="sxs-lookup"><span data-stu-id="6c34b-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="6c34b-109">Administratorzy globalni mogą zarządzać uprawnieniami do tworzenia grup (ze względów bezpieczeństwa) lub grupami usługi Office 365 utworzonymi w Portalu Azure lub w Panelu dostępu, wybierając pozycję "Użytkownicy mogą tworzyć grupy zabezpieczeń w portalach Azure" lub "Użytkownicy mogą tworzyć grupy usługi Office 365 w portalach Azure" w grupie Wszystkie grupy ogólne  >  **(ustawienia).**</span><span class="sxs-lookup"><span data-stu-id="6c34b-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="6c34b-110">Jeśli masz licencję Usługi Azure Active Directory P1 Premium, możesz też ograniczyć tworzenie grup w celu wybrania grupy użytkowników.</span><span class="sxs-lookup"><span data-stu-id="6c34b-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="6c34b-111">**Wyłączanie powiadomień powitalnych dla nowych członków grupy usługi Office 365**</span><span class="sxs-lookup"><span data-stu-id="6c34b-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="6c34b-112">Powiadomienie powitalne wysyłane do użytkowników dodanych do grup usługi Office 365 można wyłączyć, ustawiając dla opcji **UnifiedGroupWelcomeMessageEnabled wartość False** w programie PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6c34b-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="6c34b-113">Tutaj dowiesz się o tym [ustawieniu.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="6c34b-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

