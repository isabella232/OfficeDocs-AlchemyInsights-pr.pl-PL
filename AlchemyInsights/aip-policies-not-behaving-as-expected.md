---
title: 'AIP: Zasady nie zachowujące się zgodnie z oczekiwaniami'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506568"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="b84a1-102">AIP: Zasady nie zachowujące się zgodnie z oczekiwaniami</span><span class="sxs-lookup"><span data-stu-id="b84a1-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="b84a1-103">Usługa Azure Information Protection: Zasady nie zachowujące się zgodnie z oczekiwaniami, zobacz następujące wskazówki dotyczące zalecanych wskazówek dotyczących różnych problemów z zasadami:</span><span class="sxs-lookup"><span data-stu-id="b84a1-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="b84a1-104">Jeśli masz problemy z oznaczeniami wizualnymi, zapoznaj się z [oceną, kiedy stosowane są oznaczenia wizualne.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="b84a1-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="b84a1-105">Jeśli masz problemy z automatycznym etykietowaniem, zapoznaj się z [instrukcjami konfigurowania warunków automatycznej i zalecanej klasyfikacji dla usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) i czego szukają [typy poufnych informacji](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="b84a1-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="b84a1-106">Jeśli masz problemy z ochroną natywną/pfile, zapoznaj się z [konfiguracją interfejsu API plików](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="b84a1-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="b84a1-107">Sprawdź, czy używasz zasad o określonym zakresie, które nie są poprawnie skonfigurowane: [Jak skonfigurować zasady usługi Azure Information Protection dla określonych użytkowników przy użyciu zasad o określonym zakresie.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)</span><span class="sxs-lookup"><span data-stu-id="b84a1-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="b84a1-108">Jeśli automatyczne etykietowanie nie działa w programie Outlook podczas dołączania dokumentu z etykietą, sprawdź, czy drmencryptProperty nie jest zdefiniowany w sposób opisany w tym miejscu: [Ustawienia rejestru IRM dla zabezpieczeń](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="b84a1-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="b84a1-109">Jeśli nadal występują problemy, zbieraj dzienniki klientów usługi Azure Information Protection i dołączaj eksportowane dzienniki do tego biletu.</span><span class="sxs-lookup"><span data-stu-id="b84a1-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="b84a1-110">Otwórz dokument pakietu Office lub utwórz nową wiadomość e-mail w programie Outlook.</span><span class="sxs-lookup"><span data-stu-id="b84a1-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="b84a1-111">Kliknij pozycję **Chroń/Czułość**  >  **Pomoc i opinie**.</span><span class="sxs-lookup"><span data-stu-id="b84a1-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="b84a1-112">Kliknij **pozycję Eksportuj dzienniki**.</span><span class="sxs-lookup"><span data-stu-id="b84a1-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="b84a1-113">Zapisz dzienniki do wybranej lokalizacji i dołącz je do tego żądania usługi.</span><span class="sxs-lookup"><span data-stu-id="b84a1-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="b84a1-114">Dodatkowe zasoby:</span><span class="sxs-lookup"><span data-stu-id="b84a1-114">Additional resources:</span></span>

- [<span data-ttu-id="b84a1-115">Jak skonfigurować etykietę dla oznaczeń wizualnych dla usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="b84a1-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="b84a1-116">Zapoznaj się z dokumentacją usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="b84a1-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="b84a1-117">Używanie etykiet czułości w aplikacjach pakietu Office</span><span class="sxs-lookup"><span data-stu-id="b84a1-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

