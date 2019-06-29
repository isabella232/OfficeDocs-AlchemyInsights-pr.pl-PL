---
title: 646 jak skonfigurować AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 0569cb10c1d1dd422709de5d2569e43ee9d75386
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35385368"
---
# <a name="configure-sync-features"></a><span data-ttu-id="36286-102">Konfigurowanie funkcji synchronizacji</span><span class="sxs-lookup"><span data-stu-id="36286-102">Configure sync features</span></span>

<span data-ttu-id="36286-103">Azure AD Connect zawiera kilka funkcji, które są domyślnie włączone, lub można włączyć później.</span><span class="sxs-lookup"><span data-stu-id="36286-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="36286-104">Niektóre funkcje wymagają dodatkowej konfiguracji w konkretnych środowiskach.</span><span class="sxs-lookup"><span data-stu-id="36286-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="36286-105">Limitów [Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) obiekty są synchronizowane Azure AD.</span><span class="sxs-lookup"><span data-stu-id="36286-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="36286-106">Domyślnie wszystkie użytkownicy, kontakty, grupy, i Windows 10 kont komputerów są synchronizowane.</span><span class="sxs-lookup"><span data-stu-id="36286-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="36286-107">Można uwzględnić lub wykluczyć na podstawie domen, jednostek organizacyjnych lub innych atrybutów obiektów.</span><span class="sxs-lookup"><span data-stu-id="36286-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="36286-108">[Synchronizacja haseł mieszania](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizuje wartość skrótu hasła w usłudze Active Directory lokalnie usługą Azure AD.</span><span class="sxs-lookup"><span data-stu-id="36286-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="36286-109">Dzięki temu zarządzanie hasłami w jednym miejscu, ale korzystanie z tego samego hasła w obu lokalnych i środowiskach w chmurze.</span><span class="sxs-lookup"><span data-stu-id="36286-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="36286-110">Ponieważ usługa Active Directory jest autorytatywnym źródłem informacji, można użyć własnych zasad haseł.</span><span class="sxs-lookup"><span data-stu-id="36286-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="36286-111">[Resetowania hasła Sklep internetowy (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) umożliwia użytkownikom resetowania haseł w chmurze podczas nadal stosowania zasad haseł użytkownika lokalnego.</span><span class="sxs-lookup"><span data-stu-id="36286-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="36286-112">[Urządzenie stornowania](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) pozwala zarejestrowanych urządzeń w Azure AD być zapisywane z powrotem na lokalnej usługi Active Directory, mogą być używane dla dostępu warunkowego.</span><span class="sxs-lookup"><span data-stu-id="36286-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="36286-113">[Zapobiegaj przypadkowym usunięciom](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) jest domyślnie włączona w celu zapobiegania usuwanie zbyt wiele równoczesnych obiektu (ponad 500 obiektów na synchronizacji).</span><span class="sxs-lookup"><span data-stu-id="36286-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="36286-114">Można zmienić to ustawienie, aby zaspokoić potrzeby organizacji.</span><span class="sxs-lookup"><span data-stu-id="36286-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="36286-115">[Automatyczne uaktualnienie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) jest włączona domyślnie dla instalacji express i pomaga zapewnić, że używanej wersji Azure Połącz AD jest zawsze aktualna.</span><span class="sxs-lookup"><span data-stu-id="36286-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
