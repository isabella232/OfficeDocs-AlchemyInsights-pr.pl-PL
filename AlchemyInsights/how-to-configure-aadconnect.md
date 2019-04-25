---
title: 646 jak skonfigurować AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 44b2532c634bf17d87c562f9506cc1e81cc7e84a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399781"
---
# <a name="configure-sync-features"></a><span data-ttu-id="7e7e0-102">Konfigurowanie funkcji synchronizacji</span><span class="sxs-lookup"><span data-stu-id="7e7e0-102">Configure sync features</span></span>

<span data-ttu-id="7e7e0-103">Azure AD Connect zawiera kilka funkcji, które są domyślnie włączone, lub można włączyć później.</span><span class="sxs-lookup"><span data-stu-id="7e7e0-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="7e7e0-104">Niektóre funkcje wymagają dodatkowej konfiguracji w konkretnych środowiskach.</span><span class="sxs-lookup"><span data-stu-id="7e7e0-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="7e7e0-105">Limitów [Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) obiekty są synchronizowane Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7e7e0-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="7e7e0-106">Domyślnie wszystkie użytkownicy, kontakty, grupy, i Windows 10 kont komputerów są synchronizowane.</span><span class="sxs-lookup"><span data-stu-id="7e7e0-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="7e7e0-107">Można uwzględnić lub wykluczyć na podstawie domen, jednostek organizacyjnych lub innych atrybutów obiektów.</span><span class="sxs-lookup"><span data-stu-id="7e7e0-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="7e7e0-108">[Synchronizacja mieszania hasła](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizuje wartość skrótu hasła w usłudze Active Directory lokalnie usługą Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7e7e0-108">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="7e7e0-109">Dzięki temu zarządzanie hasłami w jednym miejscu, ale korzystanie z tego samego hasła w obu lokalnych i środowiskach w chmurze.</span><span class="sxs-lookup"><span data-stu-id="7e7e0-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="7e7e0-110">Ponieważ usługa Active Directory jest autorytatywnym źródłem informacji, można użyć własnych zasad haseł.</span><span class="sxs-lookup"><span data-stu-id="7e7e0-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="7e7e0-111">[Resetowania hasła Sklep internetowy (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) umożliwia użytkownikom resetowania haseł w chmurze podczas nadal stosowania zasad haseł użytkownika lokalnego.</span><span class="sxs-lookup"><span data-stu-id="7e7e0-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="7e7e0-112">[Urządzenie stornowania](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) pozwala zarejestrowanych urządzeń w Azure AD być zapisywane z powrotem na lokalnej usługi Active Directory, mogą być używane dla dostępu warunkowego.</span><span class="sxs-lookup"><span data-stu-id="7e7e0-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="7e7e0-113">[Zapobiegaj przypadkowym usunięciom](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) jest domyślnie włączona w celu zapobiegania usuwanie zbyt wiele równoczesnych obiektu (ponad 500 obiektów na synchronizacji).</span><span class="sxs-lookup"><span data-stu-id="7e7e0-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="7e7e0-114">Można zmienić to ustawienie, aby zaspokoić potrzeby organizacji.</span><span class="sxs-lookup"><span data-stu-id="7e7e0-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="7e7e0-115">[Automatyczne uaktualnienie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) jest włączona domyślnie dla instalacji express i pomaga zapewnić, że używanej wersji Azure Połącz AD jest zawsze aktualna.</span><span class="sxs-lookup"><span data-stu-id="7e7e0-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
