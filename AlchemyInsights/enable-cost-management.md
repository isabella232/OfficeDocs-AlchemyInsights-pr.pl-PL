---
title: Włączanie zarządzania kosztami
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678767"
---
# <a name="enable-cost-management"></a><span data-ttu-id="da165-102">Włączanie zarządzania kosztami</span><span class="sxs-lookup"><span data-stu-id="da165-102">Enable cost management</span></span>

<span data-ttu-id="da165-103">**Co oznacza "koszty są wyłączone dla Twojej organizacji"?**</span><span class="sxs-lookup"><span data-stu-id="da165-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="da165-104">Organizacje korzystające z kont Enterprise Agreement (EA) lub Microsoft Customer Agreement (MCA) mogą wyłączyć dostęp do informacji o kosztach i cenach.</span><span class="sxs-lookup"><span data-stu-id="da165-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="da165-105">Po zalogowaniu się do portalu Azure Portal może korzystać z interfejsów API rozliczeń w celu programistycznego pobierania faktur (po włączeniu) i szczegółów użycia.</span><span class="sxs-lookup"><span data-stu-id="da165-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="da165-106">**Jak zezwolić dodatkowym użytkownikom na uzyskiwanie dostępu do faktur**</span><span class="sxs-lookup"><span data-stu-id="da165-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="da165-107">Przejdź do **bloku subskrypcje** w portalu Azure.</span><span class="sxs-lookup"><span data-stu-id="da165-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="da165-108">Wybierz pozycję **faktury** , a następnie pozycję **dostęp do faktur**.</span><span class="sxs-lookup"><span data-stu-id="da165-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="da165-109">Włącz program Access, a następnie Zapisz zmiany, aby umożliwić użytkownikom w rolach objętych zakresem abonamentu Pobieranie faktur.</span><span class="sxs-lookup"><span data-stu-id="da165-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="da165-110">Administrator konta może również skonfigurować możliwość wysyłania faktur pocztą e-mail.</span><span class="sxs-lookup"><span data-stu-id="da165-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="da165-111">Aby dowiedzieć się więcej, zobacz [Uzyskiwanie faktury w wiadomości e-mail](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="da165-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="da165-112">**Jak dodać użytkowników do roli czytnika rozliczeń**</span><span class="sxs-lookup"><span data-stu-id="da165-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="da165-113">Przejdź do **bloku subskrypcje** w portalu Azure.</span><span class="sxs-lookup"><span data-stu-id="da165-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="da165-114">Wybierz pozycję **Kontrola dostępu (IAM)** , a następnie kliknij przycisk **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="da165-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="da165-115">Wybierz pozycję **czytnik rozliczeń** na stronie **Wybieranie roli** .</span><span class="sxs-lookup"><span data-stu-id="da165-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="da165-116">Wpisz adres e-mail użytkownika, którego chcesz zaprosić, a następnie kliknij przycisk **OK** , aby wysłać zaproszenie.</span><span class="sxs-lookup"><span data-stu-id="da165-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="da165-117">Postępuj zgodnie z instrukcjami podanymi w wiadomości e-mail z zaproszeniem, aby zalogować się jako czytnik rozliczeń.</span><span class="sxs-lookup"><span data-stu-id="da165-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="da165-118">Aby uzyskać więcej informacji, zobacz [udzielanie dostępu do rozliczeń](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="da165-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="da165-119">**Polecane dokumenty**</span><span class="sxs-lookup"><span data-stu-id="da165-119">**Recommended documents**</span></span>

- [<span data-ttu-id="da165-120">Włączanie widoków DA i AO za pośrednictwem portalu EA</span><span class="sxs-lookup"><span data-stu-id="da165-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="da165-121">Koszty wliczone w zarządzanie kosztami</span><span class="sxs-lookup"><span data-stu-id="da165-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="da165-122">Obsługiwane oferty platformy Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="da165-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="da165-123">Przegląd kosztów w analizie kosztów</span><span class="sxs-lookup"><span data-stu-id="da165-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="da165-124">Zapewnianie dostępu do informacji o rozliczeniach</span><span class="sxs-lookup"><span data-stu-id="da165-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="da165-125">Sprawdzanie dostępu do umowy z klientem firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="da165-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






