---
title: Odnajdowanie witryn
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694562"
---
# <a name="do-site-discovery"></a><span data-ttu-id="137ce-102">Odnajdowanie witryn</span><span class="sxs-lookup"><span data-stu-id="137ce-102">Do site discovery</span></span>

<span data-ttu-id="137ce-103">Jeśli Twoja organizacja nadal używa starszych aplikacji sieci Web i planuje korzystać z trybu programu Internet Explorer (co robi większość klientów), należy wykonać dodatkowe odnajdowanie witryn.</span><span class="sxs-lookup"><span data-stu-id="137ce-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="137ce-104">**Wdrożono już starszą wersję przeglądarki Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="137ce-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="137ce-105">Jeśli lista witryn przedsiębiorstwa została już skonfigurowana do działania w starszej wersji przeglądarki Microsoft Edge, odnajdowanie witryn jest prawie gotowe.</span><span class="sxs-lookup"><span data-stu-id="137ce-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="137ce-106">Jedną z rzeczy, które może być konieczne, jest dodanie witryn neutralnych.</span><span class="sxs-lookup"><span data-stu-id="137ce-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="137ce-107">Witryny neutralne to zazwyczaj witryny, które zapewniają logowanie jednokrotne.</span><span class="sxs-lookup"><span data-stu-id="137ce-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="137ce-108">Jeśli przejdź do witryny neutralnej z programu Microsoft Edge, chcesz pozostać w programie Microsoft Edge w celu uwierzytelnienia.</span><span class="sxs-lookup"><span data-stu-id="137ce-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="137ce-109">Jeśli przejdźsz do witryny neutralnej w trybie programu Internet Explorer, chcesz pozostać w trybie programu Internet Explorer w celu uwierzytelnienia.</span><span class="sxs-lookup"><span data-stu-id="137ce-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="137ce-110">Zidentyfikuj wszelkie logowania jednokrotne lub inne witryny neutralne, z których korzystasz, i dodaj je do listy witryn przedsiębiorstwa.</span><span class="sxs-lookup"><span data-stu-id="137ce-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="137ce-111">**Program Internet Explorer jest domyślną przeglądarką**</span><span class="sxs-lookup"><span data-stu-id="137ce-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="137ce-112">Jeśli teraz korzystasz tylko z programu Internet Explorer, być może nie wiesz, które witryny uaktualniły się do nowoczesnych standardów sieci Web, a które nadal wymagają programu Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="137ce-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="137ce-113">Warto znaleźć te witryny i dodać je do listy witryn przedsiębiorstwa, aby można było używać trybu programu Internet Explorer tylko dla tych witryn.</span><span class="sxs-lookup"><span data-stu-id="137ce-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="137ce-114">[Odnajdowanie witryn przedsiębiorstwa](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) wykrywa witryny, które mogą wymagać trybu programu Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="137ce-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="137ce-115">Może zbierać dane na komputerach z systemem Windows Internet Explorer 8 za pośrednictwem programu Internet Explorer 11 w systemie Windows 10, Windows 8.1 lub Windows 7.</span><span class="sxs-lookup"><span data-stu-id="137ce-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="137ce-116">**Analizowanie danych**</span><span class="sxs-lookup"><span data-stu-id="137ce-116">**Analyze the data**</span></span>

<span data-ttu-id="137ce-117">Po zebraniu danych witryny zalecamy, aby w celu ich przeanalizowania był następujący proces czteroetapowy:</span><span class="sxs-lookup"><span data-stu-id="137ce-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="137ce-118">Sortuj dane według domeny, a następnie według adresu URL.</span><span class="sxs-lookup"><span data-stu-id="137ce-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="137ce-119">Zdefiniuj granice aplikacji, aby skonfigurować tryb programu Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="137ce-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="137ce-120">Chcesz uwzględnić wszystkie witryny i kontrolki sieci Web definiujące aplikację, ale nie chcesz uwzględniać dodatkowych witryn i kontrolek.</span><span class="sxs-lookup"><span data-stu-id="137ce-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="137ce-121">Niektóre witryny mogą być tak proste, jak *https://contoso.com/app1* inne mogą wymagać zdefiniowania wielu witryn i stron.</span><span class="sxs-lookup"><span data-stu-id="137ce-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="137ce-122">Przetestuj aplikację, aby sprawdzić, czy nie działa natywnie.</span><span class="sxs-lookup"><span data-stu-id="137ce-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="137ce-123">Wiele witryn oferuje nowoczesną zawartość po wykryciu nowoczesnej przeglądarki i oferuje starszą zawartość tylko wtedy, gdy wykryje program Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="137ce-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="137ce-124">Dodaj aplikację do listy witryn przedsiębiorstwa, jeśli testy nie powiedzie się.</span><span class="sxs-lookup"><span data-stu-id="137ce-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="137ce-125">Najlepszym rozwiązaniem jest pogrupowanie wszystkich witryn składających się na aplikację.</span><span class="sxs-lookup"><span data-stu-id="137ce-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="137ce-126">Dzięki temu podczas uaktualniania aplikacji łatwiej będzie usunąć całą witrynę z trybu programu Internet Explorer i rozpocząć korzystanie z nowoczesnej przeglądarki dla tej aplikacji.</span><span class="sxs-lookup"><span data-stu-id="137ce-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="137ce-127">Po zakończeniu odnajdowania witryn i przeanalizowaniu danych możesz zacząć analizować strategię kanału.</span><span class="sxs-lookup"><span data-stu-id="137ce-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

