---
title: Obsługa fakturowania w ramach nowoczesnych wiadomości e-mail w usłudze Azure
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
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922139"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="92d2d-102">Fakturowanie wiadomości e-mail na platformie Azure</span><span class="sxs-lookup"><span data-stu-id="92d2d-102">Email invoicing in Azure</span></span>

<span data-ttu-id="92d2d-103">Aby zaktualizować preferencję na fakturze e-mail, musisz mieć właściciela lub rolę współautora w profilu rozliczeń lub koncie rozliczeniowym.</span><span class="sxs-lookup"><span data-stu-id="92d2d-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="92d2d-104">Po wybraniu tej funkcji wszyscy użytkownicy z rolami właściciel, współautorzy, czytelnicy i Menedżer faktur będą mogli otrzymać fakturę w wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="92d2d-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="92d2d-105">Zaloguj się w [witrynie Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="92d2d-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="92d2d-106">Wyszukaj **Zarządzanie kosztami + rozliczenia**.</span><span class="sxs-lookup"><span data-stu-id="92d2d-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="92d2d-107">Wybierz pozycję **faktury** z lewej strony, a następnie wybierz pozycję **Faktura w wiadomości e-mail** od początku strony.</span><span class="sxs-lookup"><span data-stu-id="92d2d-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="92d2d-108">Jeśli masz wiele profilów rozliczeń, wybierz profil rozliczeniowy, a następnie wybierz pozycję **Zrezygnuj**.</span><span class="sxs-lookup"><span data-stu-id="92d2d-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="92d2d-109">Wybierz pozycję **Aktualizuj**.</span><span class="sxs-lookup"><span data-stu-id="92d2d-109">Select **Update**.</span></span>
6. <span data-ttu-id="92d2d-110">Jeśli masz wiele profilów rozliczeń, wybierz profil rozliczeniowy, a następnie wybierz pozycję **Zrezygnuj**.</span><span class="sxs-lookup"><span data-stu-id="92d2d-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="92d2d-111">Możesz udostępnić innym osobom dostęp do wyświetlania, pobierania i płacenia faktur, przypisując im rolę Menedżer fakturowania dla profilu rozliczania MCA lub MPA.</span><span class="sxs-lookup"><span data-stu-id="92d2d-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="92d2d-112">Jeśli zaznaczono opcję pobierania faktury w wiadomości e-mail, użytkownicy będą mogli także uzyskać faktury w wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="92d2d-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="92d2d-113">Zaloguj się w [witrynie Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="92d2d-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="92d2d-114">Wyszukaj **Zarządzanie kosztami + rozliczenia**.</span><span class="sxs-lookup"><span data-stu-id="92d2d-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="92d2d-115">Wybierz pozycję **Profile rozliczeń** z lewej strony.</span><span class="sxs-lookup"><span data-stu-id="92d2d-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="92d2d-116">Na liście Profile rozliczeń wybierz profil rozliczeniowy, dla którego chcesz przypisać rolę Menedżera faktur.</span><span class="sxs-lookup"><span data-stu-id="92d2d-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="92d2d-117">Wybierz pozycję **Kontrola dostępu (IAM)** z lewej strony, a następnie wybierz pozycję **Dodaj** od początku strony.</span><span class="sxs-lookup"><span data-stu-id="92d2d-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="92d2d-118">Z listy rozwijanej rola wybierz pozycję **Menedżer faktur**.</span><span class="sxs-lookup"><span data-stu-id="92d2d-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="92d2d-119">Wprowadź adres e-mail użytkownika, który ma udzielić dostępu.</span><span class="sxs-lookup"><span data-stu-id="92d2d-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="92d2d-120">Wybierz pozycję **Zapisz** , aby przypisać rolę.</span><span class="sxs-lookup"><span data-stu-id="92d2d-120">Select **Save** to assign the role.</span></span>
