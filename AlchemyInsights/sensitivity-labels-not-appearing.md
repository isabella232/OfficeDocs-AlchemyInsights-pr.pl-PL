---
title: Etykiety czułości nie są wyświetlane
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: df64022f6ad684e2af3eac080068536b7a167b74
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581025"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="fe418-102">Etykiety czułości nie są wyświetlane</span><span class="sxs-lookup"><span data-stu-id="fe418-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="fe418-103">Etykiety czułości umożliwiają klasyfikowanie i ochronę poufnych treści.</span><span class="sxs-lookup"><span data-stu-id="fe418-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="fe418-104">Można je tworzyć w centrum zgodności usługi Microsoft 365, centrum zabezpieczeń usługi Microsoft 365 lub centrum zgodności & zabezpieczeń usługi Microsoft 365 w obszarze Etykiety klasyfikacji > czułości.</span><span class="sxs-lookup"><span data-stu-id="fe418-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="fe418-105">Aby dowiedzieć się więcej o tej funkcji, zobacz [Omówienie etykiet czułości](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="fe418-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="fe418-106">Jeśli etykiety czułości zostały skonfigurowane, ale nie są one wyświetlane w aplikacjach usługi Microsoft 365, sprawdź następujące kwestie:</span><span class="sxs-lookup"><span data-stu-id="fe418-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="fe418-107">Upewnij się, że etykieta czułości została [opublikowana](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) dla użytkowników i grup, które chcesz.</span><span class="sxs-lookup"><span data-stu-id="fe418-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="fe418-108">Upewnij się, że użytkownik korzysta z aplikacji obsługującej etykiety czułości — zobacz [etykiety czułości w dokumencie](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="fe418-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="fe418-109">Jeśli [przeprowadzasz migrację etykiet usługi Azure Information Protection,](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)należy pamiętać o zagadnieniach wymienionych [tutaj](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span><span class="sxs-lookup"><span data-stu-id="fe418-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="fe418-110">Obsługa zapobiegania utracie danych (DLP): obecnie tylko etykiety przechowywania mogą być używane jako warunek w zasadach DLP.</span><span class="sxs-lookup"><span data-stu-id="fe418-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="fe418-111">Obsługa etykiet czułości w zasadach DLP nie jest jeszcze dostępna, ale pracujemy nad tym.</span><span class="sxs-lookup"><span data-stu-id="fe418-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="fe418-112">Gdy szyfrowanie jest włączone na etykiecie czułości, można wybrać:</span><span class="sxs-lookup"><span data-stu-id="fe418-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="fe418-113">Przypisz uprawnienia teraz</span><span class="sxs-lookup"><span data-stu-id="fe418-113">Assign permissions now</span></span>
    - <span data-ttu-id="fe418-114">Zezwalanie użytkownikom na przypisywanie uprawnień</span><span class="sxs-lookup"><span data-stu-id="fe418-114">Let users assign permissions</span></span>


<span data-ttu-id="fe418-115">Aby uzyskać więcej informacji na temat możliwych problemów, zobacz [Znane problemy z etykietami czułości](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="fe418-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>