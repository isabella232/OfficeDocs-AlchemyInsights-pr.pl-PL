---
title: Etykiety czułości nie pojawiają się
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 4bf8e02246c966f22648467386a7862f0521fecf
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207235"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="6af22-102">Etykiety czułości nie pojawiają się</span><span class="sxs-lookup"><span data-stu-id="6af22-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="6af22-103">Etykiety czułości pozwalają klasyfikować i chronić poufne treści.</span><span class="sxs-lookup"><span data-stu-id="6af22-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="6af22-104">Mogą one być tworzone w centrum zgodności Microsoft 365, Centrum zabezpieczeń Microsoft 365 lub Office 365 Security & Compliance Center w obszarze Klasyfikacja etykiet > czułość.</span><span class="sxs-lookup"><span data-stu-id="6af22-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Office 365 Security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="6af22-105">Aby dowiedzieć się więcej na temat tej funkcji, zobacz [Omówienie etykiet czułości](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="6af22-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span></span>

<span data-ttu-id="6af22-106">Jeśli skonfigurowano etykiety czułości, ale nie są wyświetlane w aplikacjach pakietu Office, sprawdź następujące elementy:</span><span class="sxs-lookup"><span data-stu-id="6af22-106">If you configured your sensitivity labels but they aren't appearing in the Office apps, check the following:</span></span>

- <span data-ttu-id="6af22-107">Potwierdź, że etykieta czułości została [opublikowana](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) dla użytkowników i grup, które mają.</span><span class="sxs-lookup"><span data-stu-id="6af22-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="6af22-108">Potwierdź, że użytkownik korzysta z aplikacji obsługującej etykiety czułości — zobacz [etykiety czułości w dokumencie](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="6af22-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).</span></span>

- <span data-ttu-id="6af22-109">Jeśli [migrujesz etykiety usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), należy pamiętać o zagadnienia wymienione w [tym miejscu](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span><span class="sxs-lookup"><span data-stu-id="6af22-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="6af22-110">Obsługa zapobiegania utracie danych (DLP): obecnie tylko etykiety przechowywania mogą być użyte jako warunek w zasadach DLP.</span><span class="sxs-lookup"><span data-stu-id="6af22-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="6af22-111">Obsługa etykiet czułości w zasadach DLP nie jest jeszcze dostępna, ale pracujemy nad nim.</span><span class="sxs-lookup"><span data-stu-id="6af22-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="6af22-112">Gdy szyfrowanie jest włączone na etykiecie czułości, można wybrać opcję:</span><span class="sxs-lookup"><span data-stu-id="6af22-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="6af22-113">Przypisz uprawnienia teraz</span><span class="sxs-lookup"><span data-stu-id="6af22-113">Assign permissions now</span></span>
    - <span data-ttu-id="6af22-114">Pozwól użytkownikom przypisywać uprawnienia</span><span class="sxs-lookup"><span data-stu-id="6af22-114">Let users assign permissions</span></span>


<span data-ttu-id="6af22-115">Aby uzyskać więcej informacji na temat możliwych problemów, zobacz [znane problemy z etykietami czułości](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="6af22-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>