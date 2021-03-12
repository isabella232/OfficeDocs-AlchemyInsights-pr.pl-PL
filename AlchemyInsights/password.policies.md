---
title: Zasady dotyczące haseł
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747048"
---
# <a name="password-policies"></a><span data-ttu-id="36fe1-102">Zasady dotyczące haseł</span><span class="sxs-lookup"><span data-stu-id="36fe1-102">Password policies</span></span>

<span data-ttu-id="36fe1-103">**Mam problemy z zasadami haseł użytkownika**</span><span class="sxs-lookup"><span data-stu-id="36fe1-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="36fe1-104">Zasady dotyczące haseł dla użytkownika zależą od tego, czy użytkownik jest tylko w chmurze, czy lokalnie.</span><span class="sxs-lookup"><span data-stu-id="36fe1-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="36fe1-105">Tylko użytkownicy w chmurze muszą wybrać hasło spełniające wymagania z tego artykułu: Zasady dotyczące haseł, które mają zastosowanie tylko [do kont użytkowników w chmurze](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="36fe1-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="36fe1-106">Użytkownicy lokalni muszą wybrać hasło spełniające wymagania lokalne.</span><span class="sxs-lookup"><span data-stu-id="36fe1-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="36fe1-107">Jeśli użytkownik lokalnego nie może ustawić swojego hasła, sprawdź wymagania lokalne.</span><span class="sxs-lookup"><span data-stu-id="36fe1-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="36fe1-108">**Nie wiem, jak ustawić lub sprawdzić zasady wygasania haseł**</span><span class="sxs-lookup"><span data-stu-id="36fe1-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="36fe1-109">Przy użyciu programu PowerShell możesz ustawić i sprawdzić zasady wygasania dla użytkowników chmury w dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="36fe1-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="36fe1-110">Wykonaj instrukcje z tego artykułu: Ustawianie lub sprawdzanie zasad dotyczących haseł [przy użyciu programu PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="36fe1-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="36fe1-111">Zasady wygasania haseł użytkowników lokalnych są ustawiane w lokalnej u użytkownikach AD.</span><span class="sxs-lookup"><span data-stu-id="36fe1-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="36fe1-112">**Inne przydatne linki:**</span><span class="sxs-lookup"><span data-stu-id="36fe1-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="36fe1-113">Wprowadzenie do resetowania hasła</span><span class="sxs-lookup"><span data-stu-id="36fe1-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="36fe1-114">Rozwiązywanie problemów z resetowaniem hasła inicjowanych przez administratora</span><span class="sxs-lookup"><span data-stu-id="36fe1-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
