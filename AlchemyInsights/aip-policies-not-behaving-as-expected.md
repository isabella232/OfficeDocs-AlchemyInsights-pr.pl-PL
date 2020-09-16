---
title: 'Podzasada: zasady niezachowuje się zgodnie z oczekiwaniami'
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
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663199"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="746f4-102">Podzasada: zasady niezachowuje się zgodnie z oczekiwaniami</span><span class="sxs-lookup"><span data-stu-id="746f4-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="746f4-103">Ochrona informacji na platformie Azure: zasady nie zachowuje się zgodnie z oczekiwaniami, zapoznaj się z poniższymi wskazówkami dotyczącymi różnych zagadnień dotyczących zasad:</span><span class="sxs-lookup"><span data-stu-id="746f4-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="746f4-104">Jeśli występują problemy z oznaczeniami wizualnymi, sprawdź, czy [zostaną zastosowane oznaczenia wizualne](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="746f4-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="746f4-105">Jeśli występują problemy z automatycznym oznaczaniem etykietami, zobacz [Konfigurowanie warunków automatycznej i zalecanej klasyfikacji usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) oraz tego [, co szukają typy informacji poufnych](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="746f4-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="746f4-106">Jeśli masz problemy z ochroną w trybie macierzystym/Pfileym, sprawdź [konfigurację interfejsu API pliku](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="746f4-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="746f4-107">Sprawdzanie, czy są używane zasady dotyczące zakresu, które nie są poprawnie skonfigurowane: [jak skonfigurować zasady usługi Azure Information Protection dla określonych użytkowników przy użyciu zasad dotyczących zakresu](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="746f4-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="746f4-108">Jeśli automatyczne etykietowanie nie działa w programie Outlook podczas dołączania dokumentu opatrzonego etykietą, sprawdź, czy DRMEncryptProperty nie jest zdefiniowany w następujący sposób: [Ustawienia rejestru usługi IRM dotyczące zabezpieczeń](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="746f4-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="746f4-109">Jeśli nadal występują problemy, Zbierz dzienniki klienta usługi Azure Information Protection i Dołącz wyeksportowane dzienniki do tego biletu.</span><span class="sxs-lookup"><span data-stu-id="746f4-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="746f4-110">Otwórz dokument pakietu Office lub Utwórz nową wiadomość e-mail w programie Outlook.</span><span class="sxs-lookup"><span data-stu-id="746f4-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="746f4-111">Kliknij pozycję Pomoc dotycząca **ochrony/wrażliwości**  >  **i opinie**.</span><span class="sxs-lookup"><span data-stu-id="746f4-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="746f4-112">Kliknij pozycję **Eksportuj dzienniki**.</span><span class="sxs-lookup"><span data-stu-id="746f4-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="746f4-113">Zapisz dzienniki w wybranym miejscu, a następnie dołącz je do tego żądania usługi.</span><span class="sxs-lookup"><span data-stu-id="746f4-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="746f4-114">Dodatkowe zasoby:</span><span class="sxs-lookup"><span data-stu-id="746f4-114">Additional resources:</span></span>

- [<span data-ttu-id="746f4-115">Jak skonfigurować etykietę wizualnych oznaczeń dla usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="746f4-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="746f4-116">Przegląd dokumentacji dotyczącej ochrony informacji platformy Azure</span><span class="sxs-lookup"><span data-stu-id="746f4-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="746f4-117">Używanie etykiet liter w aplikacjach Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="746f4-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

