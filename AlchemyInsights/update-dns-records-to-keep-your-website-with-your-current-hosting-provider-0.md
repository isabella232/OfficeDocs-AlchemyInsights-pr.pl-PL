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
ms.openlocfilehash: 62f49038cf541c2185ed6a60c6cb58fe2889342d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353187"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="542c7-102">Aktualizowanie rekordów DNS w celu zachowania witryny sieci Web u obecnego dostawcy hostingu</span><span class="sxs-lookup"><span data-stu-id="542c7-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="542c7-103">Na stronie [Domeny](https://portal.office.com/adminportal/home#/Domains) wybierz z listy domen tę domenę, której używasz dla witryny internetowej, a następnie w okienku zarządzania wybierz pozycję **Ustawienia DNS**.</span><span class="sxs-lookup"><span data-stu-id="542c7-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span>

2. <span data-ttu-id="542c7-104">Wybierz pozycję **+ Nowy rekord niestandardowy** i wprowadź następujące wartości:</span><span class="sxs-lookup"><span data-stu-id="542c7-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="542c7-105">W polu **Typ DNS** wprowadź: **A (Adres)**</span><span class="sxs-lookup"><span data-stu-id="542c7-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="542c7-106">W polu **Nazwa hosta lub alias** wpisz następujący tekst: **@**</span><span class="sxs-lookup"><span data-stu-id="542c7-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="542c7-107">W polu **Adres IP** wpisz statyczny adres IP, pod którym witryna sieci Web jest obecnie hostowana (na przykład 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="542c7-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="542c7-p101">Adres IP musi być  *statyczny*  , a nie  *dynamiczny*  . Skontaktuj się z dostawcą hostingu i upewnij się, że możesz uzyskać statyczny adres IP swojej publicznej witryny sieci Web.</span><span class="sxs-lookup"><span data-stu-id="542c7-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="542c7-110">Wybierz pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="542c7-110">Select **Save**.</span></span>

<span data-ttu-id="542c7-111">Możesz też utworzyć rekord CNAME, aby ułatwić klientom odnalezienie Twojej witryny sieci Web.</span><span class="sxs-lookup"><span data-stu-id="542c7-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="542c7-112">Wybierz pozycję **+ Nowy rekord niestandardowy** i wprowadź następujące wartości:</span><span class="sxs-lookup"><span data-stu-id="542c7-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="542c7-113">W polu **Typ DNS** wprowadź: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="542c7-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="542c7-114">W polu **Nazwa hosta lub alias** wpisz następujący tekst: **www**.</span><span class="sxs-lookup"><span data-stu-id="542c7-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="542c7-115">W polu **Wskazywany adres** wpisz w pełni kwalifikowaną nazwę domeny (FQDN) swojej witryny sieci Web (na przykład contoso.com).</span><span class="sxs-lookup"><span data-stu-id="542c7-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="542c7-116">Wybierz pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="542c7-116">Select **Save**.</span></span>
