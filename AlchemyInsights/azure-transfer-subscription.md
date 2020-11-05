---
title: Transferowanie własności usługi Azure do rozliczeń
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922165"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="5ebca-102">Transferowanie własności usługi Azure do rozliczeń</span><span class="sxs-lookup"><span data-stu-id="5ebca-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="5ebca-103">Zaloguj się w [witrynie Azure Portal](https://portal.azure.com/) jako administrator konta rozliczeniowego z subskrypcją, którą chcesz przenieść.</span><span class="sxs-lookup"><span data-stu-id="5ebca-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="5ebca-104">Jeśli nie masz pewności, czy jesteś administratorem, lub jeśli potrzebujesz określić, kto jest, zobacz [Określanie administratora rozliczania kont](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="5ebca-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="5ebca-105">Wyszukaj w obszarze **Zarządzanie kosztami + rozliczenia**.</span><span class="sxs-lookup"><span data-stu-id="5ebca-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="5ebca-106">Wybierz pozycję **subskrypcje** z okienka po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="5ebca-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="5ebca-107">W zależności od dostępu może być konieczne wybranie zakresu rozliczeń, a następnie **abonamentów** lub **subskrypcji platformy Azure**.</span><span class="sxs-lookup"><span data-stu-id="5ebca-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="5ebca-108">Wybieranie **prawa własności do rozliczeń** dla subskrypcji, którą chcesz przenieść</span><span class="sxs-lookup"><span data-stu-id="5ebca-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="5ebca-109">Wprowadź adres e-mail użytkownika, który jest administratorem rozliczeń konta, który będzie nowym właścicielem subskrypcji, a następnie wybierz pozycję **Wyślij żądanie przeniesienia**</span><span class="sxs-lookup"><span data-stu-id="5ebca-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="5ebca-110">Użytkownik otrzyma wiadomość e-mail z instrukcjami w celu przejrzenia żądania przeniesienia.</span><span class="sxs-lookup"><span data-stu-id="5ebca-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="5ebca-111">Aby zatwierdzić żądanie przeniesienia, użytkownik wybiera link w wiadomości e-mail i postępuje zgodnie z instrukcjami.</span><span class="sxs-lookup"><span data-stu-id="5ebca-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="5ebca-112">**Uwaga** : Jeśli przekierujesz własność rozliczeniową abonamentu na konto użytkownika w innej dzierżawie usługi Azure AD, wszystkie przydziały [kontroli dostępu oparte na rolach (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)do zarządzania zasobami w ramach subskrypcji zostaną trwale usunięte.</span><span class="sxs-lookup"><span data-stu-id="5ebca-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="5ebca-113">Tylko nowy właściciel będzie miał dostęp do zarządzania zasobami w ramach subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="5ebca-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="5ebca-114">Aby uzyskać więcej informacji, zobacz [przenoszenie subskrypcji do użytkownika w innej dzierżawie usługi Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="5ebca-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="5ebca-115">**Polecane dokumenty**</span><span class="sxs-lookup"><span data-stu-id="5ebca-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="5ebca-116">Prawo do przenoszenia prawa własności do konta usługi Azure na innym koncie</span><span class="sxs-lookup"><span data-stu-id="5ebca-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="5ebca-117">Informacje o transferowaniu własności do rozliczeń dla subskrypcji platformy Azure</span><span class="sxs-lookup"><span data-stu-id="5ebca-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="5ebca-118">Przenoszenie programu Visual Studio, sieci partnera firmy Microsoft (MPN) i regulowanie abonamentów na dev/testowe</span><span class="sxs-lookup"><span data-stu-id="5ebca-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="5ebca-119">Przekazywanie praw własności — często zadawane pytania</span><span class="sxs-lookup"><span data-stu-id="5ebca-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="5ebca-120">Rozwiązywanie problemów dotyczących przekazywania własności</span><span class="sxs-lookup"><span data-stu-id="5ebca-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
