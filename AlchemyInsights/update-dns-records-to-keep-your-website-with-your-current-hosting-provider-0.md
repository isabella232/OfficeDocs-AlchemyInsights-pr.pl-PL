---
title: Aktualizowanie rekordów DNS w celu zachowania witryny sieci Web u obecnego dostawcy hostingu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: e437015d476c1417fa37e1b1c250e2205e9ce4d9
ms.sourcegitcommit: b825ced7b66d452b0f3874a57e033e690ec41c93
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2019
ms.locfileid: "35925295"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="c7eca-102">Aktualizowanie rekordów DNS w celu zachowania witryny sieci Web u obecnego dostawcy hostingu</span><span class="sxs-lookup"><span data-stu-id="c7eca-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="c7eca-103">Na stronie [domeny](https://portal.office.com/adminportal/home#/Domains) na liście domen, zaznacz domenę, którą używasz na swojej stronie internetowej.</span><span class="sxs-lookup"><span data-stu-id="c7eca-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="c7eca-104">Wybierz pozycję **+ Nowy rekord niestandardowy** i wprowadź następujące wartości:</span><span class="sxs-lookup"><span data-stu-id="c7eca-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="c7eca-105">W polu **Typ DNS** wprowadź: **A (Adres)**</span><span class="sxs-lookup"><span data-stu-id="c7eca-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="c7eca-106">W polu **Nazwa hosta lub alias** wpisz następujący tekst: **@**</span><span class="sxs-lookup"><span data-stu-id="c7eca-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="c7eca-107">W polu **Adres IP** wpisz statyczny adres IP, pod którym witryna sieci Web jest obecnie hostowana (na przykład 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="c7eca-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="c7eca-p101">Adres IP musi być  *statyczny*  , a nie  *dynamiczny*  . Skontaktuj się z dostawcą hostingu i upewnij się, że możesz uzyskać statyczny adres IP swojej publicznej witryny sieci Web.</span><span class="sxs-lookup"><span data-stu-id="c7eca-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="c7eca-110">Wybierz pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="c7eca-110">Select **Save**.</span></span>

<span data-ttu-id="c7eca-111">Możesz też utworzyć rekord CNAME, aby ułatwić klientom odnalezienie Twojej witryny sieci Web.</span><span class="sxs-lookup"><span data-stu-id="c7eca-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="c7eca-112">Wybierz pozycję **+ Nowy rekord niestandardowy** i wprowadź następujące wartości:</span><span class="sxs-lookup"><span data-stu-id="c7eca-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="c7eca-113">W polu **Typ DNS** wprowadź: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="c7eca-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="c7eca-114">W polu **Nazwa hosta lub alias** wpisz następujący tekst: **www**.</span><span class="sxs-lookup"><span data-stu-id="c7eca-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="c7eca-115">W polu **Wskazywany adres** wpisz w pełni kwalifikowaną nazwę domeny (FQDN) swojej witryny sieci Web (na przykład contoso.com).</span><span class="sxs-lookup"><span data-stu-id="c7eca-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="c7eca-116">Wybierz pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="c7eca-116">Select **Save**.</span></span>
