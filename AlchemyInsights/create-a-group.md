---
title: Tworzenie grupy
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088910"
---
# <a name="create-a-group"></a><span data-ttu-id="98f91-102">Tworzenie grupy</span><span class="sxs-lookup"><span data-stu-id="98f91-102">Create a group</span></span>

<span data-ttu-id="98f91-103">W tym temacie opisano tworzenie grup.</span><span class="sxs-lookup"><span data-stu-id="98f91-103">This topic describes group creation.</span></span>

<span data-ttu-id="98f91-104">**Uprawnienie do tworzenia grupy**</span><span class="sxs-lookup"><span data-stu-id="98f91-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="98f91-105">Upewnij się, że masz autoryzację do tworzenia nowej grupy.</span><span class="sxs-lookup"><span data-stu-id="98f91-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="98f91-106">Administratorzy globalni mogą wyłączyć tworzenie grup w witrynie Azure Portal lub panelu programu Access.</span><span class="sxs-lookup"><span data-stu-id="98f91-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="98f91-107">Aby utworzyć nową grupę lub uzyskać odpowiednie uprawnienia, może być konieczne posiadanie administratora.</span><span class="sxs-lookup"><span data-stu-id="98f91-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="98f91-108">**Zarządzanie uprawnieniami do tworzenia grup**</span><span class="sxs-lookup"><span data-stu-id="98f91-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="98f91-109">Administratorzy globalni mogą zarządzać uprawnieniami do tworzenia grup (z powodów związanych z zabezpieczeniami) lub grup usługi Office 365 utworzonych w witrynie Azure Portal lub panelu dostępu, wybierając pozycję "użytkownicy mogą tworzyć grupy zabezpieczeń w portalu Azure" lub "użytkownicy mogą tworzyć grupy usługi Office 365 w obszarze portale Azure" — Opcje we **wszystkich grupach**—  >  **Ogólne (Ustawienia)**.</span><span class="sxs-lookup"><span data-stu-id="98f91-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="98f91-110">Możesz również ograniczyć możliwość tworzenia grup, aby wybrać grupę użytkowników, jeśli masz licencję usługi Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="98f91-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="98f91-111">**Wyłączanie powiadomienia powitalnego dla nowych członków grupy pakietu Office 365**</span><span class="sxs-lookup"><span data-stu-id="98f91-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="98f91-112">Powiadomienie powitalne wysyłane do użytkowników, którzy są dodawani do grup usługi Office 365, można wyłączyć, ustawiając **UnifiedGroupWelcomeMessageEnabled** na false (FAŁSZ) w programie PowerShell.</span><span class="sxs-lookup"><span data-stu-id="98f91-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="98f91-113">Dowiedz się więcej o [tym ustawieniu.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="98f91-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

