---
title: Aktualizowanie rekordów DNS w celu zachowania witryny sieci Web u obecnego dostawcy hostingu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827538"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="df0ef-102">Aktualizowanie rekordów DNS w celu zachowania witryny sieci Web u obecnego dostawcy hostingu</span><span class="sxs-lookup"><span data-stu-id="df0ef-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="df0ef-103">W centrum administracyjnym platformy Microsoft 365 przejdź do strony Konfiguracja domen i z listy domen wybierz domenę, która jest twoją   >  [](https://admin.microsoft.com/Adminportal#/Domains) witryną sieci Web.</span><span class="sxs-lookup"><span data-stu-id="df0ef-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="df0ef-104">Wybierz pozycję **+ Nowy rekord niestandardowy** i wprowadź następujące wartości:</span><span class="sxs-lookup"><span data-stu-id="df0ef-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="df0ef-105">W polu **Typ DNS** wprowadź: **A (Adres)**</span><span class="sxs-lookup"><span data-stu-id="df0ef-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="df0ef-106">W polu **Nazwa hosta lub alias** wpisz następujący tekst: **@**</span><span class="sxs-lookup"><span data-stu-id="df0ef-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="df0ef-107">W polu **Adres IP** wpisz statyczny adres IP, pod którym witryna sieci Web jest obecnie hostowana (na przykład 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="df0ef-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="df0ef-p101">Adres IP musi być  *statyczny*  , a nie  *dynamiczny*  . Skontaktuj się z dostawcą hostingu i upewnij się, że możesz uzyskać statyczny adres IP swojej publicznej witryny sieci Web.</span><span class="sxs-lookup"><span data-stu-id="df0ef-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="df0ef-110">Wybierz pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="df0ef-110">Select **Save**.</span></span>

<span data-ttu-id="df0ef-111">Możesz też utworzyć rekord CNAME, aby ułatwić klientom odnalezienie Twojej witryny sieci Web.</span><span class="sxs-lookup"><span data-stu-id="df0ef-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="df0ef-112">Wybierz pozycję **+ Nowy rekord niestandardowy** i wprowadź następujące wartości:</span><span class="sxs-lookup"><span data-stu-id="df0ef-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="df0ef-113">W polu **Typ DNS** wprowadź: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="df0ef-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="df0ef-114">W polu **Nazwa hosta lub alias** wpisz następujący tekst: **www**.</span><span class="sxs-lookup"><span data-stu-id="df0ef-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="df0ef-115">W polu **Wskazywany adres** wpisz w pełni kwalifikowaną nazwę domeny (FQDN) swojej witryny sieci Web (na przykład contoso.com).</span><span class="sxs-lookup"><span data-stu-id="df0ef-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="df0ef-116">Wybierz pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="df0ef-116">Select **Save**.</span></span>
