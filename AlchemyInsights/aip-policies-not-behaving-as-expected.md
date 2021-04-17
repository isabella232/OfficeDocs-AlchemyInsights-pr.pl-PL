---
title: 'AIP: Zasady nie zachowują się zgodnie z oczekiwaniami'
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
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821637"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="49a96-102">AIP: Zasady nie zachowują się zgodnie z oczekiwaniami</span><span class="sxs-lookup"><span data-stu-id="49a96-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="49a96-103">Azure Information Protection: Zasady nie zachowują się zgodnie z oczekiwaniami, zobacz następujące zalecane wskazówki dotyczące różnych problemów z zasadami:</span><span class="sxs-lookup"><span data-stu-id="49a96-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="49a96-104">Jeśli masz problemy z oznaczeniami wizualnymi, zapoznaj się z [tematem Kiedy](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)są stosowane oznaczenia wizualne .</span><span class="sxs-lookup"><span data-stu-id="49a96-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="49a96-105">Jeśli masz problemy z automatycznym oznaczaniem etykiet, zapoznaj się z tematem Jak skonfigurować warunki dla klasyfikacji automatycznej i zalecanej dla usługi [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) i Czego szukać w przypadku typów informacji [poufnych.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="49a96-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="49a96-106">Jeśli masz problemy z ochroną natywnych/plików P, sprawdź [konfigurację interfejsu API plików.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)</span><span class="sxs-lookup"><span data-stu-id="49a96-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="49a96-107">Sprawdź, czy używasz zasad z zakresami, które nie zostały prawidłowo skonfigurowane: Jak skonfigurować zasady Azure Information Protection dla określonych użytkowników przy użyciu [zasad o zakresach.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)</span><span class="sxs-lookup"><span data-stu-id="49a96-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="49a96-108">Jeśli w programie Outlook nie działa automatyczne oznaczanie etykiet podczas dołączania dokumentu oznaczonego etykietą, sprawdź, czy funkcja DRMEncryptProperty nie jest zdefiniowana w sposób opisany tutaj: Ustawienia rejestru [usługi IRM](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)dla zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="49a96-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="49a96-109">Jeśli nadal występują problemy, zbierz dzienniki klienta usługi Azure Information Protection i dołącz wyeksportowane dzienniki do tego biletu.</span><span class="sxs-lookup"><span data-stu-id="49a96-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="49a96-110">Otwórz dokument pakietu Office lub utwórz nową wiadomość e-mail w programie Outlook.</span><span class="sxs-lookup"><span data-stu-id="49a96-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="49a96-111">Kliknij **pozycję Ochrona/czułość**  >  **Pomoc i opinie**.</span><span class="sxs-lookup"><span data-stu-id="49a96-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="49a96-112">Kliknij **pozycję Eksportuj dzienniki.**</span><span class="sxs-lookup"><span data-stu-id="49a96-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="49a96-113">Zapisz dzienniki w wybranej lokalizacji i dołącz je do tego żądania usługi.</span><span class="sxs-lookup"><span data-stu-id="49a96-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="49a96-114">Dodatkowe zasoby:</span><span class="sxs-lookup"><span data-stu-id="49a96-114">Additional resources:</span></span>

- [<span data-ttu-id="49a96-115">Jak skonfigurować etykietę oznaczania wizualnego dla usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="49a96-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="49a96-116">Przejrzyj dokumentację usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="49a96-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="49a96-117">Używanie etykiet wrażliwości w aplikacjach platformy Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="49a96-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

