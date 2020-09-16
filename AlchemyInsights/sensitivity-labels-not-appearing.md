---
title: Etykiety wrażliwości nie są wyświetlane
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801194"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="badf9-102">Etykiety wrażliwości nie są wyświetlane</span><span class="sxs-lookup"><span data-stu-id="badf9-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="badf9-103">Etykiety wrażliwości pozwalają sklasyfikować i chronić poufną zawartość.</span><span class="sxs-lookup"><span data-stu-id="badf9-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="badf9-104">Można je utworzyć w centrum zgodności z programem Microsoft 365, Centrum zabezpieczeń Microsoft 365 lub Microsoft 365 Security & Center w obszarze Klasyfikacja wrażliwości > etykiet.</span><span class="sxs-lookup"><span data-stu-id="badf9-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="badf9-105">Aby dowiedzieć się więcej o tej funkcji, zobacz [Omówienie etykiet wrażliwości](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="badf9-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="badf9-106">Jeśli etykiety wrażliwości zostały skonfigurowane, ale nie są wyświetlane w aplikacjach Microsoft 365, sprawdź następujące elementy:</span><span class="sxs-lookup"><span data-stu-id="badf9-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="badf9-107">Upewnij się, że etykieta wrażliwości została [opublikowana](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) na potrzeby użytkowników i grup.</span><span class="sxs-lookup"><span data-stu-id="badf9-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="badf9-108">Upewnij się, że użytkownik korzysta z aplikacji obsługującej etykiety wrażliwości — zobacz [etykiety liter w dokumencie](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="badf9-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="badf9-109">Jeśli [przeprowadzasz migrację etykiet ochrony danych platformy Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), zapoznaj się z wymienionymi [tutaj](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)uwagami.</span><span class="sxs-lookup"><span data-stu-id="badf9-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="badf9-110">Obsługa ochrony przed utratą danych (DLP): obecnie w zasadach DLP można użyć tylko etykiet przechowywania jako warunków.</span><span class="sxs-lookup"><span data-stu-id="badf9-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="badf9-111">Obsługa etykiet wrażliwości w zasadach DLP nie jest jeszcze dostępna, ale pracujemy nad nią.</span><span class="sxs-lookup"><span data-stu-id="badf9-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="badf9-112">Po włączeniu szyfrowania na etykiecie czułości możesz wybrać jedną z następujących opcji:</span><span class="sxs-lookup"><span data-stu-id="badf9-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="badf9-113">Przydziel teraz uprawnienia</span><span class="sxs-lookup"><span data-stu-id="badf9-113">Assign permissions now</span></span>
    - <span data-ttu-id="badf9-114">Zezwalanie użytkownikom na przypisywanie uprawnień</span><span class="sxs-lookup"><span data-stu-id="badf9-114">Let users assign permissions</span></span>


<span data-ttu-id="badf9-115">Aby uzyskać więcej informacji na temat możliwych problemów, zobacz [znane problemy z etykietami czułości](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="badf9-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>