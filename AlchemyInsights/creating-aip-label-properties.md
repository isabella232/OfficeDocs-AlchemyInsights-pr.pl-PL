---
title: Tworzenie zasad etykiety AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569507"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="a936f-102">Tworzenie zasad etykiety AIP</span><span class="sxs-lookup"><span data-stu-id="a936f-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="a936f-103">Etykiety usługi Azure Information Protection(AIP) mogą być używane z pełnym zakresem danych, które organizacja zazwyczaj tworzy i przechowuje, od najniższej klasyfikacji danych osobowych do najwyższej klasyfikacji wysoce poufnych danych.</span><span class="sxs-lookup"><span data-stu-id="a936f-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="a936f-104">Zasady usługi Azure Information Protection mają zastosowanie do klasycznego klienta usługi Azure Information Protection(AIP), a nie [do klienta ujednoliconego etykietowania AIP.](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history)</span><span class="sxs-lookup"><span data-stu-id="a936f-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="a936f-105">Można skonfigurować wiele elementów w zasadach AIP, w tym opcje, takie jak:</span><span class="sxs-lookup"><span data-stu-id="a936f-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="a936f-106">Opcja, dla której etykieta pozwoli administratorom lub użytkownikom klasyfikować i chronić (opcjonalne) dokumenty i wiadomości e-mail</span><span class="sxs-lookup"><span data-stu-id="a936f-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="a936f-107">Opcja wymuszania klasyfikacji, gdy użytkownicy zapisują dokumenty i wysyłają wiadomości e-mail</span><span class="sxs-lookup"><span data-stu-id="a936f-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="a936f-108">Opcja automatycznego oznaczania wiadomości e-mail na podstawie jej załączników.</span><span class="sxs-lookup"><span data-stu-id="a936f-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="a936f-109">Opcja określania, czy pasek ochrony informacji jest wyświetlany w aplikacjach pakietu Office</span><span class="sxs-lookup"><span data-stu-id="a936f-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="a936f-110">Aby uzyskać dodatkowe opcje i informacje dotyczące zasad usługi Azure Information Protection, zobacz: [Omówienie zasad usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="a936f-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="a936f-111">Aby uzyskać inne przydatne zasoby dotyczące zasad AIP, zobacz:</span><span class="sxs-lookup"><span data-stu-id="a936f-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="a936f-112">Samouczek: Konfigurowanie ustawień zasad usługi Azure Information Protection i tworzenie nowej etykiety</span><span class="sxs-lookup"><span data-stu-id="a936f-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="a936f-113">Konfigurowanie zasad usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a936f-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="a936f-114">Tworzenie i konfigurowanie etykiet czułości i ich zasad</span><span class="sxs-lookup"><span data-stu-id="a936f-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="a936f-115">Instrukcje dotyczące typowych scenariuszy korzystających z usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a936f-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="a936f-116">Zapoznaj się z dokumentacją usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a936f-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="a936f-117">Wymagania dotyczące usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a936f-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="a936f-118">Szybki start samouczek dotyczący usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a936f-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="a936f-119">Pobierz klienta usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a936f-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)