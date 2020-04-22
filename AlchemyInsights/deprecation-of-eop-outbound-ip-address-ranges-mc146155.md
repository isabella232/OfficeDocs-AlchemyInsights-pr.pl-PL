---
title: 1065 Wycofanie wychodzących zakresów adresów IP EOPMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704607"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="bce31-102">Wycofanie zakresów wychodzących adresów IP EOP</span><span class="sxs-lookup"><span data-stu-id="bce31-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="bce31-103">Wykryliśmy potencjalny problem z Twoją organizacją, który (jeśli nie zostanie poprawiony do 26 października 2018 r.) może przerwać przepływ poczty do lokalnych lub zewnętrznych miejsc docelowych.</span><span class="sxs-lookup"><span data-stu-id="bce31-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="bce31-104">Jak wcześniej informowaliśmy, aby uprościć zarządzanie zakresem adresów IP, konsolidujemy zakresy adresów IP usługi Exchange Online Protection (EOP), które są używane do wysyłania i odbierania wiadomości e-mail poza usługą Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bce31-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="bce31-105">Nasza analiza wskazuje, że co najmniej jedno z zewnętrznych źródeł poczty e-mail lub miejsc docelowych skonfigurowanych w łącznikach przepływu poczty nie akceptuje połączeń z zakresów adresów IP pokazanych [tutaj.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)</span><span class="sxs-lookup"><span data-stu-id="bce31-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="bce31-106">Działaj przed 26 października, aby zapewnić, że te źródła i miejsca docelowe będą akceptować połączenia ze wszystkimi [opublikowanymi adresami IP EOP.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)</span><span class="sxs-lookup"><span data-stu-id="bce31-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="bce31-107">Aby uzyskać więcej informacji na temat tej zmiany, zobacz Posty Centrum wiadomości [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)lub [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="bce31-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="bce31-108">**Uwaga:** Jeśli wcześniej używano publikowania adresów IP lub ADRESU URL za pośrednictwem html, XML i RSS do aktualizacji punktów końcowych, należy również przeprowadzić migrację do nowych usług sieci web w celu automatyzacji tego typu aktualizacji.</span><span class="sxs-lookup"><span data-stu-id="bce31-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="bce31-109">Aby uzyskać więcej informacji, zobacz [kategorie punktów końcowych usługi Microsoft 365 oraz adres IP i usługa sieci web usługi adresów IP i adresu URL firmy Microsoft 365](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="bce31-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
