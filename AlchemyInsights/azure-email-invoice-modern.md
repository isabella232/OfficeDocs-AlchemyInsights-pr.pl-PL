---
title: Nowoczesne fakturowanie poczty e-mail platformy Azure
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820836"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="9b3eb-102">Fakturowanie poczty e-mail na platformie Azure</span><span class="sxs-lookup"><span data-stu-id="9b3eb-102">Email invoicing in Azure</span></span>

<span data-ttu-id="9b3eb-103">Aby zaktualizować preferencje dotyczące faktur e-mail, musisz mieć rolę właściciela lub współautora w profilu rozliczeniowym lub na jego koncie rozliczeniowym.</span><span class="sxs-lookup"><span data-stu-id="9b3eb-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="9b3eb-104">Po wybraniu zgody wszyscy użytkownicy z rolami właściciela, współautora, czytelników i menedżera faktur w profilu rozliczeniowym otrzymają fakturę w wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="9b3eb-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="9b3eb-105">Zaloguj się do [portalu Azure Portal.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="9b3eb-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="9b3eb-106">Szukaj w pozycji **Zarządzanie kosztami + rozliczenia**.</span><span class="sxs-lookup"><span data-stu-id="9b3eb-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="9b3eb-107">Wybierz **pozycję Faktury** z lewej strony, a następnie wybierz pozycję Wyślij fakturę pocztą e-mail u góry strony. </span><span class="sxs-lookup"><span data-stu-id="9b3eb-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="9b3eb-108">Jeśli masz wiele profilów rozliczeniowych, wybierz profil rozliczeniowy, a następnie wybierz pozycję **Wybierz opcję**.</span><span class="sxs-lookup"><span data-stu-id="9b3eb-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="9b3eb-109">Wybierz **pozycję Aktualizuj**.</span><span class="sxs-lookup"><span data-stu-id="9b3eb-109">Select **Update**.</span></span>
6. <span data-ttu-id="9b3eb-110">Jeśli masz wiele profilów rozliczeniowych, wybierz profil rozliczeniowy, a następnie wybierz pozycję **Wybierz opcję**.</span><span class="sxs-lookup"><span data-stu-id="9b3eb-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="9b3eb-111">Możesz dać innym osobom dostęp do wyświetlania, pobierania i opłacania faktur, przypisując im rolę menedżera faktur dla profilu rozliczeniowego MCA lub MPA.</span><span class="sxs-lookup"><span data-stu-id="9b3eb-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="9b3eb-112">Jeśli w wiadomości e-mail wybrałeś(-asz) fakturę, użytkownicy również otrzymają faktury w wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="9b3eb-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="9b3eb-113">Zaloguj się do [portalu Azure Portal.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="9b3eb-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="9b3eb-114">Szukaj w pozycji **Zarządzanie kosztami + rozliczenia**.</span><span class="sxs-lookup"><span data-stu-id="9b3eb-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="9b3eb-115">Wybierz **pozycję Profile rozliczeniowe** z lewej strony.</span><span class="sxs-lookup"><span data-stu-id="9b3eb-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="9b3eb-116">Z listy profile rozliczeniowe wybierz profil rozliczeniowy, do którego chcesz przypisać rolę menedżera faktur.</span><span class="sxs-lookup"><span data-stu-id="9b3eb-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="9b3eb-117">Wybierz **pozycję Kontrola dostępu (IAM)** z lewej strony, a następnie wybierz pozycję **Dodaj** u góry strony.</span><span class="sxs-lookup"><span data-stu-id="9b3eb-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="9b3eb-118">Z listy rozwijanej Rola wybierz pozycję **Menedżer faktur**.</span><span class="sxs-lookup"><span data-stu-id="9b3eb-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="9b3eb-119">Wprowadź adres e-mail użytkownika, który ma udzielić dostępu.</span><span class="sxs-lookup"><span data-stu-id="9b3eb-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="9b3eb-120">Wybierz **pozycję Zapisz,** aby przypisać rolę.</span><span class="sxs-lookup"><span data-stu-id="9b3eb-120">Select **Save** to assign the role.</span></span>
