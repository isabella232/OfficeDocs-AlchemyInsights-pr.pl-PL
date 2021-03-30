---
title: Single-Sign na urządzeniach przyłączony do usługi Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405052"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="4a51b-102">Logowanie pojedyncze dla urządzeń przyłącznych do usługi Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="4a51b-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="4a51b-103">Jeśli masz lokalne środowisko usługi Active Directory (AD) i chcesz dołączyć komputery przyłączone do domeny usługi AD do usługi Azure AD, możesz to zrobić, wykonując hybrydowe dołączanie do usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4a51b-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="4a51b-104">[Jak to zrobić: Planowanie hybrydowej implementacji](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) dołączania do usługi Azure Active Directory zawiera powiązane kroki implementacji hybrydowego sprzężenia usługi Azure AD w środowisku.</span><span class="sxs-lookup"><span data-stu-id="4a51b-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="4a51b-105">Konfigurowanie urządzeń przyłącznych do usługi Azure AD dla aplikacji lokalnych Single-Sign przy użyciu funkcji Windows Hello dla firm</span><span class="sxs-lookup"><span data-stu-id="4a51b-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="4a51b-106">**Problemy z tokenem odświeżania podstawowego (PRT)** Token odświeżania podstawowego (PRT) to kluczowy artefakt uwierzytelniania usługi Azure AD na urządzeniach z systemem Windows 10, Windows Server 2016 i nowszych wersjach oraz urządzeniach z systemami iOS i Android.</span><span class="sxs-lookup"><span data-stu-id="4a51b-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="4a51b-107">Jest to token sieci Web JSON (JWT) specjalnie wydany dla pierwszego tokenu tokenu zabezpieczającego firmy Microsoft w celu umożliwienia logowania jednokrotnego (SSO) w aplikacjach używanych na tych urządzeniach.</span><span class="sxs-lookup"><span data-stu-id="4a51b-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="4a51b-108">[W tece Co to jest token odświeżania podstawowego?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)zostaną ci szczegółowe informacje o tym, jak jest wydany, używany i chroniony prt na urządzeniach z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="4a51b-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="4a51b-109">**WamDefaultSet: YES i AzureADPrt: YES** Te pola wskazują, czy użytkownik pomyślnie uwierzytelnił się w usłudze Azure AD podczas logowania się na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="4a51b-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="4a51b-110">Jeśli wartości to **NIE,** może to być spowodowane:</span><span class="sxs-lookup"><span data-stu-id="4a51b-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="4a51b-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span><span class="sxs-lookup"><span data-stu-id="4a51b-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="4a51b-112">Alternatywny identyfikator logowania</span><span class="sxs-lookup"><span data-stu-id="4a51b-112">Alternate Login ID</span></span>
- <span data-ttu-id="4a51b-113">Nie znaleziono serwera proxy HTTP</span><span class="sxs-lookup"><span data-stu-id="4a51b-113">HTTP Proxy not found</span></span>

<span data-ttu-id="4a51b-114">Rozwiązywanie problemów z urządzeniami przy użyciu polecenia dsregcmd — [stan logowania jednokrotnego](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="4a51b-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
