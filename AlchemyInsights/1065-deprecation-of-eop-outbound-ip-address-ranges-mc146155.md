---
title: 1065 oczekiwany podniesienie uprawnień wychodzących rangesMC146155 adres IP
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: ec87141ffaa2fa3484620a9b52851e3e92f20b6b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29483204"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="43dcb-102">Oczekiwany podniesienie poziomu uprawnień wychodzących zakresów adresów IP</span><span class="sxs-lookup"><span data-stu-id="43dcb-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="43dcb-p101">Wykryto potencjalny problem z organizacji, (Jeśli nie zostaną usunięte przez 26 października 2018) może przerwać przepływ poczty do lokalnego lub zewnętrznych miejsc docelowych. Jak wcześniej przekazanych Aby uprościć zarządzanie zakres adresów IP, możemy jest konsolidowany na podstawie zakresów adresów IP Exchange Online ochrony (podniesienie uprawnień), które są używane do wysyłania i odbierania wiadomości e-mail, poza usługi Office 365. Nasza analiza wskazuje, że jedną lub kilkoma e-mail zewnętrznych źródeł i miejsc docelowych, które zostały skonfigurowane w łączniki przepływu poczty nie są akceptowanie połączeń z IP adres zakresów pokazano [tutaj](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="43dcb-p101">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations. As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365. Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="43dcb-106">Działania przed 26 października do upewnij się, że te źródła i miejsca docelowe będzie akceptować połączenia z wszystkie [opublikowane adresy IP podniesienie poziomu uprawnień](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="43dcb-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="43dcb-107">Aby uzyskać więcej informacji o tej zmianie zobacz Centrum wiadomości poczty, [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)lub [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="43dcb-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="43dcb-p102">**Uwaga**: Jeśli poprzednio używane adres IP lub adres URL publikowania przez HTML, XML i RSS dla aktualizacji punktu końcowego, również należy dokonać migracji do nowych usług sieci web do automatyzacji typów aktualizacji. Aby uzyskać więcej informacji zobacz [kategorii punktu końcowego usługi Office 365 i adres IP pakietu Office 365 i adres URL usługi sieci web](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="43dcb-p102">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates. For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

