---
title: Aktualizowanie adresów sprzedanych i rozliczeniowych skojarzonych z procedurami zalecanymi przez MCA
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004166"
- "7325"
ms.openlocfilehash: 8cdd2c64a95e88eb2fb4624c6e2696f77b75e198
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679986"
---
# <a name="update-sold-to-and-bill-to-address-associated-to-your-mca---recommended-steps"></a><span data-ttu-id="28d46-102">Aktualizowanie adresów sprzedanych i rozliczeniowych skojarzonych z procedurami zalecanymi przez MCA</span><span class="sxs-lookup"><span data-stu-id="28d46-102">Update sold-to and bill-to address associated to your MCA - recommended steps</span></span>

<span data-ttu-id="28d46-103">Możesz zaktualizować adres "sprzedany" i "płatnika" skojarzony z umową dotyczącą klientów firmy Microsoft (MCA).</span><span class="sxs-lookup"><span data-stu-id="28d46-103">You can update the sold-to and bill-to address associated to your Microsoft Customer Agreement (MCA).</span></span> 

> [!NOTE]
> <span data-ttu-id="28d46-104">Zmiany w profilu użytkownika usługi Azure Active Directory mogą wprowadzać tylko administrator użytkowników.</span><span class="sxs-lookup"><span data-stu-id="28d46-104">Only a user administrator can make changes to the Azure Active Directory user profile information.</span></span> <span data-ttu-id="28d46-105">Jeśli nie masz przypisanej roli administratora użytkowników, skontaktuj się z administratorem.</span><span class="sxs-lookup"><span data-stu-id="28d46-105">If you're not assigned the user administrator role, contact your user administrator.</span></span> <span data-ttu-id="28d46-106">Aby uzyskać więcej informacji na temat zmieniania profilu użytkownika, zobacz [Dodawanie lub aktualizowanie informacji o profilu użytkownika przy użyciu usługi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="28d46-106">For more information about changing a user's profile, see [Add or update a user's profile information using Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal).</span></span>

<span data-ttu-id="28d46-107">**Adres sprzedaży** — adres sprzedany to adres, a także informacje kontaktowe organizacji lub osoby, która jest odpowiedzialna za konto rozliczeniowe.</span><span class="sxs-lookup"><span data-stu-id="28d46-107">**Sold-to address** - The sold-to address is the address and the contact information of the organization or the individual, who is responsible for a billing account.</span></span> <span data-ttu-id="28d46-108">Zostanie ona wyświetlona we wszystkich fakturach wygenerowanych dla konta rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="28d46-108">It's displayed in all the invoices generated for the billing account.</span></span>

<span data-ttu-id="28d46-109">**Adres płatnika** — adres płatnika to adres i informacje kontaktowe organizacji lub osoby, która jest odpowiedzialna za faktury wygenerowane dla konta rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="28d46-109">**Bill-to address** - The bill-to address is the address and the contact information of the organization or the individual, who is responsible for the invoices generated for a billing account.</span></span> <span data-ttu-id="28d46-110">W przypadku konta rozliczeniowego składnika MCA jest to adres płatnika dla każdego profilu rozliczeń i jest on wyświetlany na fakturze wygenerowanej dla profilu rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="28d46-110">For a billing account for an MCA, there's a bill-to address for each billing profile and it's displayed in the invoice generated for the billing profile.</span></span>

<span data-ttu-id="28d46-111">**Aby zaktualizować konto rozliczeniowe MCA adres sprzedany**:</span><span class="sxs-lookup"><span data-stu-id="28d46-111">**To update an MCA billing account sold-to address**:</span></span>

1. <span data-ttu-id="28d46-112">Zaloguj się w witrynie Azure Portal przy użyciu adresu e-mail, który ma właściciela lub rolę współautora na koncie rozliczeniowym MCA.</span><span class="sxs-lookup"><span data-stu-id="28d46-112">Sign in to the Azure portal using the email address, which has an owner or a contributor role on the billing account for an MCA.</span></span>
1. <span data-ttu-id="28d46-113">Wyszukaj rozliczenia **kosztów zarządzania kosztami**  +  .</span><span class="sxs-lookup"><span data-stu-id="28d46-113">Search for **Cost Management** + **Billing**.</span></span>
1. <span data-ttu-id="28d46-114">Kliknij pozycję **Właściwości**  >  **Aktualizuj sprzedaż**.</span><span class="sxs-lookup"><span data-stu-id="28d46-114">Click **Properties** > **Update sold-to**.</span></span>
1. <span data-ttu-id="28d46-115">Wprowadź nowy adres i kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="28d46-115">Enter the new address and click **Save**.</span></span>

<span data-ttu-id="28d46-116">Niektóre konta wymagają dodatkowej weryfikacji, aby można było zaktualizować jej adres do sprzedaży.</span><span class="sxs-lookup"><span data-stu-id="28d46-116">Some accounts require additional verification before their sold-to address can be updated.</span></span> <span data-ttu-id="28d46-117">Jeśli Twoje konto wymaga ręcznego zatwierdzania, zostanie wyświetlony monit o skontaktowanie się z pomocą techniczną platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="28d46-117">If your account requires manual approval, you'll be asked to contact Azure support.</span></span>

<span data-ttu-id="28d46-118">**Aby zaktualizować adres konta rozliczeniowego MCA**:</span><span class="sxs-lookup"><span data-stu-id="28d46-118">**To update an MCA billing account address**:</span></span> 

1. <span data-ttu-id="28d46-119">Zaloguj się w witrynie Azure Portal przy użyciu adresu e-mail, który ma właściciela lub rolę współautora na koncie rozliczeniowym lub profilu rozliczeniowym dla MCA.</span><span class="sxs-lookup"><span data-stu-id="28d46-119">Sign in to the Azure portal using the email address, which has an owner or a contributor role on a billing account or a billing profile for an MCA.</span></span>
1. <span data-ttu-id="28d46-120">Wyszukaj rozliczenia **kosztów zarządzania kosztami**  +  .</span><span class="sxs-lookup"><span data-stu-id="28d46-120">Search for **Cost Management** + **Billing**.</span></span>
1. <span data-ttu-id="28d46-121">Kliknij kolejno pozycje **Profile rozliczeń** i wybierz profil rozliczeniowy, aby zaktualizować adres rozliczeniowy.</span><span class="sxs-lookup"><span data-stu-id="28d46-121">Click **Billing profiles** and select a select a billing profile to update the billing address.</span></span>
1. <span data-ttu-id="28d46-122">Kliknij pozycję **Właściwości**  >  **Aktualizuj adres**.</span><span class="sxs-lookup"><span data-stu-id="28d46-122">Click **Properties** > **Update address**.</span></span>
1. <span data-ttu-id="28d46-123">Wprowadź nowy adres, a następnie kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="28d46-123">Enter the new address and then click **Save**.</span></span>

<span data-ttu-id="28d46-124">**Polecane dokumenty**</span><span class="sxs-lookup"><span data-stu-id="28d46-124">**Recommended documents**</span></span>

<span data-ttu-id="28d46-125">[Zmienianie informacji o kontakcie z kontem rozliczeniowym na platformie Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile) </span><span class="sxs-lookup"><span data-stu-id="28d46-125">[Change contact information for an Azure billing account](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile) </span></span>  
[<span data-ttu-id="28d46-126">Aktualizowanie ustawień konta rozliczeniowego</span><span class="sxs-lookup"><span data-stu-id="28d46-126">Update billing account settings</span></span>](https://docs.microsoft.com/microsoft-store/update-microsoft-store-for-business-account-settings)  
[<span data-ttu-id="28d46-127">Opis ról administracyjnych umowy klienta firmy Microsoft na platformie Azure</span><span class="sxs-lookup"><span data-stu-id="28d46-127">Understand Microsoft Customer Agreement administrative roles in Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)