---
title: 646 Jak skonfigurować AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722573"
---
# <a name="configure-sync-features"></a><span data-ttu-id="abfe6-102">Konfigurowanie funkcji synchronizacji</span><span class="sxs-lookup"><span data-stu-id="abfe6-102">Configure sync features</span></span>

<span data-ttu-id="abfe6-103">Usługa Azure AD Connect zawiera kilka funkcji, które są domyślnie włączone lub które można włączyć później.</span><span class="sxs-lookup"><span data-stu-id="abfe6-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="abfe6-104">Niektóre funkcje wymagają dodatkowej konfiguracji w określonych środowiskach.</span><span class="sxs-lookup"><span data-stu-id="abfe6-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="abfe6-105">[Filtrowanie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) ogranicza obiekty są synchronizowane z usługą Azure AD.</span><span class="sxs-lookup"><span data-stu-id="abfe6-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="abfe6-106">Domyślnie wszyscy użytkownicy, kontakty, grupy i konta komputerów z systemem Windows 10 są synchronizowane.</span><span class="sxs-lookup"><span data-stu-id="abfe6-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="abfe6-107">Obiekty można dołączać lub wykluczać na podstawie domen, obiektów organizacyjnych lub innych atrybutów.</span><span class="sxs-lookup"><span data-stu-id="abfe6-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="abfe6-108">[Synchronizacja skrótu hasła](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizuje skrót hasła z lokalnej usługi Active Directory do usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="abfe6-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="abfe6-109">Umożliwia to zarządzanie hasłami w jednej lokalizacji, ale używanie tego samego hasła zarówno w środowisku lokalnym, jak i w chmurze.</span><span class="sxs-lookup"><span data-stu-id="abfe6-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="abfe6-110">Ponieważ usługa Active Directory jest źródłem autorytatywnym, można użyć własnych zasad haseł.</span><span class="sxs-lookup"><span data-stu-id="abfe6-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="abfe6-111">[Samoobsługowe resetowanie haseł (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) umożliwia użytkownikom resetowanie własnych haseł w chmurze przy jednoczesnym stosowaniu lokalnych zasad haseł.</span><span class="sxs-lookup"><span data-stu-id="abfe6-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="abfe6-112">[Zapis wsteczny urządzenia](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) umożliwia zarejestrowanym urządzeniom w usłudze Azure AD zapisywanie z powrotem w lokalnej usłudze Active Directory, dzięki czemu mogą być używane do dostępu warunkowego.</span><span class="sxs-lookup"><span data-stu-id="abfe6-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="abfe6-113">[Zapobieganie przypadkowym usuwaniom](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) jest domyślnie włączone, aby zapobiec zbyt wielu równoczesnym usuwaniom obiektów (ponad 500 obiektów na synchronizację).</span><span class="sxs-lookup"><span data-stu-id="abfe6-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="abfe6-114">To ustawienie można zmienić w celu zaspokojenia potrzeb organizacji.</span><span class="sxs-lookup"><span data-stu-id="abfe6-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="abfe6-115">[Automatyczne uaktualnianie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) jest domyślnie włączone dla instalacji ekspresowych i pomaga upewnić się, że twoja wersja usługi Azure AD Connect jest zawsze aktualna.</span><span class="sxs-lookup"><span data-stu-id="abfe6-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
