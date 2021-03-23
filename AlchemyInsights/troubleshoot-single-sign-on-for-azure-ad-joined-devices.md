---
title: Rozwiązywanie problemów z logowaniem pojedynczym dla urządzeń przyłącznych do usługi Azure AD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037339"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="bc1bc-102">Rozwiązywanie problemów z logowaniem pojedynczym dla urządzeń przyłącznych do usługi Azure AD</span><span class="sxs-lookup"><span data-stu-id="bc1bc-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="bc1bc-103">Jeśli masz lokalne środowisko usługi Active Directory (AD) i chcesz dołączyć komputery przyłączone do domeny usługi AD do usługi Azure AD, możesz to zrobić, wykonując hybrydowe dołączanie do usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bc1bc-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="bc1bc-104">[Jak to zrobić: Planowanie hybrydowej implementacji](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) dołączania do usługi Azure Active Directory zawiera powiązane kroki implementacji hybrydowego sprzężenia usługi Azure AD w środowisku.</span><span class="sxs-lookup"><span data-stu-id="bc1bc-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="bc1bc-105">Aby uzyskać więcej informacji, zobacz Konfigurowanie urządzeń przyłącznych do usługi Azure AD dla urządzeń lokalnychSingle-Sign [Wł. przy użyciu funkcji Windows Hello dla firm.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)</span><span class="sxs-lookup"><span data-stu-id="bc1bc-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="bc1bc-106">**Problemy z tokenem odświeżania podstawowego (PRT)**</span><span class="sxs-lookup"><span data-stu-id="bc1bc-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="bc1bc-107">Token odświeżania podstawowego (PRT) to kluczowy artefakt uwierzytelniania usługi Azure AD na urządzeniach z systemem Windows 10, Windows Server 2016 i nowszych wersjach oraz urządzeniach z systemami iOS i Android.</span><span class="sxs-lookup"><span data-stu-id="bc1bc-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="bc1bc-108">Jest to token sieci Web JSON (JWT) specjalnie wydany dla pierwszego tokenu tokenu zabezpieczającego firmy Microsoft w celu umożliwienia logowania jednokrotnego (SSO) w aplikacjach używanych na tych urządzeniach.</span><span class="sxs-lookup"><span data-stu-id="bc1bc-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="bc1bc-109">Aby uzyskać szczegółowe informacje o tym, jak jest wystawiany, używany i chroniony prt na urządzeniach z systemem Windows 10, zobacz Co to jest [token odświeżania podstawowego?.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)</span><span class="sxs-lookup"><span data-stu-id="bc1bc-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="bc1bc-110">**WamDefaultSet: YES i AzureADPrt: YES**</span><span class="sxs-lookup"><span data-stu-id="bc1bc-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="bc1bc-111">Te pola wskazują, czy użytkownik pomyślnie uwierzytelnił się w usłudze Azure AD podczas logowania się na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="bc1bc-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="bc1bc-112">Jeśli wartości to **NIE,** może to być spowodowane:</span><span class="sxs-lookup"><span data-stu-id="bc1bc-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="bc1bc-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span><span class="sxs-lookup"><span data-stu-id="bc1bc-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="bc1bc-114">Alternatywny identyfikator logowania</span><span class="sxs-lookup"><span data-stu-id="bc1bc-114">Alternate Login ID</span></span>
- <span data-ttu-id="bc1bc-115">Nie znaleziono serwera proxy HTTP</span><span class="sxs-lookup"><span data-stu-id="bc1bc-115">HTTP Proxy not found</span></span>

<span data-ttu-id="bc1bc-116">Aby rozwiązać problemy z urządzeniami przy użyciu polecenia dsregcmd, zobacz [Stan logowania jednokrotnego.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="bc1bc-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
