---
title: Zasady przechowywania w Centrum administracyjnym programu Exchange nie działają
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952238"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="99ef7-102">Zasady przechowywania w Centrum administracyjnym programu Exchange</span><span class="sxs-lookup"><span data-stu-id="99ef7-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="99ef7-103">Jeśli chcesz, abyśmy uruchamiali automatyczne testy ustawień wymienionych poniżej, wybierz przycisk wstecz < — u góry tej strony, a następnie wprowadź adres e-mail użytkownika, który ma problemy z zasadami przechowywania.</span><span class="sxs-lookup"><span data-stu-id="99ef7-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="99ef7-104">Jeśli masz problemy z zasadami przechowywania w Centrum administracyjnym programu Exchange, które nie mają zastosowania do skrzynek pocztowych lub elementów, które nie są przenoszące do archiwaowej skrzynki pocztowej, sprawdź następujące kwestie:</span><span class="sxs-lookup"><span data-stu-id="99ef7-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="99ef7-105">**Główne przyczyny:**</span><span class="sxs-lookup"><span data-stu-id="99ef7-105">**Root Causes:**</span></span>

- <span data-ttu-id="99ef7-106">**Asystent folderów zarządzanych** nie przetworzył skrzynki pocztowej użytkownika.</span><span class="sxs-lookup"><span data-stu-id="99ef7-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="99ef7-107">Asystent folderów zarządzanych co siedem dni podejmuje próbę przetwarzania każdej skrzynki pocztowej w organizacji opartej na chmurze.</span><span class="sxs-lookup"><span data-stu-id="99ef7-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="99ef7-108">**Rozwiązanie:** Uruchom asystenta folderów zarządzanych.</span><span class="sxs-lookup"><span data-stu-id="99ef7-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="99ef7-109">**W skrzynce pocztowej** **włączono funkcję RetentionHold.**</span><span class="sxs-lookup"><span data-stu-id="99ef7-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="99ef7-110">Jeśli skrzynka pocztowa została umieszczona na wartości retentionhold, zasady przechowywania w skrzynce pocztowej nie będą przetwarzane w tym czasie.</span><span class="sxs-lookup"><span data-stu-id="99ef7-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="99ef7-111">**Rozwiązanie:** Sprawdź stan ustawienia Hold (Przechowywanie) i zaktualizuj je zgodnie z potrzebami.</span><span class="sxs-lookup"><span data-stu-id="99ef7-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="99ef7-112">Aby uzyskać szczegółowe informacje, zobacz [Przechowywanie skrzynki pocztowej.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="99ef7-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="99ef7-113">**Uwaga:** Jeśli skrzynka pocztowa jest mniejsza niż 10 MB, Asystent folderów zarządzanych nie będzie automatycznie przetwarzał tej skrzynki.</span><span class="sxs-lookup"><span data-stu-id="99ef7-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="99ef7-114">Aby uzyskać więcej informacji na temat zasad przechowywania w Centrum administracyjnym programu Exchange, zobacz:</span><span class="sxs-lookup"><span data-stu-id="99ef7-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="99ef7-115">Tagi przechowywania i zasady przechowywania</span><span class="sxs-lookup"><span data-stu-id="99ef7-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="99ef7-116">[Stosowanie zasad przechowywania do skrzynek pocztowych lub](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [Dodawanie lub usuwanie tagów przechowywania](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="99ef7-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="99ef7-117">Jak określić typ hold'a umieszczonego w skrzynce pocztowej</span><span class="sxs-lookup"><span data-stu-id="99ef7-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
