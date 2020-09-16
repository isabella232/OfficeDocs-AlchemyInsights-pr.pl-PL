---
title: Tworzenie zasad dotyczących etykiet dla produktów
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732185"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="a9e33-102">Tworzenie zasad dotyczących etykiet dla produktów</span><span class="sxs-lookup"><span data-stu-id="a9e33-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="a9e33-103">Etykiety usługi Azure Information Protection (dla instytucji nadzorowanej) mogą być używane z pełnym zakresem danych, które są zwykle tworzone i przechowywane w organizacji, od najniższej klasyfikacji danych osobowych do najwyższej klasyfikacji danych, które są wysoce poufne.</span><span class="sxs-lookup"><span data-stu-id="a9e33-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="a9e33-104">Zasady ochrony informacji o platformie Azure dotyczą klasycznego  [klienta usługi](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history)Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a9e33-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="a9e33-105">W zasadach dotyczących polityki nadzorowanej można skonfigurować wiele elementów, w tym następujące opcje:</span><span class="sxs-lookup"><span data-stu-id="a9e33-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="a9e33-106">Opcja, dla której etykieta będzie umożliwić administratorom lub klasyfikowaniu użytkowników oraz ochronę (opcjonalne) dokumentów i wiadomości e-mail</span><span class="sxs-lookup"><span data-stu-id="a9e33-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="a9e33-107">Opcja wymuszania klasyfikacji podczas zapisywania dokumentów i wysyłania wiadomości e-mail przez użytkowników</span><span class="sxs-lookup"><span data-stu-id="a9e33-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="a9e33-108">Opcja umożliwiająca automatyczne etykietowanie wiadomości e-mail na podstawie jej załączników.</span><span class="sxs-lookup"><span data-stu-id="a9e33-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="a9e33-109">Opcja umożliwiająca sterowanie tym, czy pasek ochrona informacji jest wyświetlany w aplikacjach pakietu Office</span><span class="sxs-lookup"><span data-stu-id="a9e33-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="a9e33-110">Aby uzyskać dodatkowe opcje i informacje dotyczące zasad usługi Azure Information Protection, zobacz: [Omówienie zasad dotyczących usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="a9e33-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="a9e33-111">W przypadku innych przydatnych zasobów związanych z zasadami dotyczącymi programu, zobacz:</span><span class="sxs-lookup"><span data-stu-id="a9e33-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="a9e33-112">Samouczek: Konfigurowanie ustawień zasad usługi Azure Information Protection i tworzenie nowej etykiety</span><span class="sxs-lookup"><span data-stu-id="a9e33-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="a9e33-113">Konfigurowanie zasad usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a9e33-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="a9e33-114">Tworzenie i Konfigurowanie etykiet wrażliwości oraz ich zasad</span><span class="sxs-lookup"><span data-stu-id="a9e33-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="a9e33-115">Przewodniki dotyczące typowych scenariuszy korzystających z usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a9e33-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="a9e33-116">Przegląd dokumentacji dotyczącej ochrony informacji platformy Azure</span><span class="sxs-lookup"><span data-stu-id="a9e33-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="a9e33-117">Wymagania dotyczące usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a9e33-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="a9e33-118">Przewodnik Szybki Start dla usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a9e33-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="a9e33-119">Pobierz klienta usługi Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a9e33-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)