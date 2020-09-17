---
title: 1065 zaniechanie EOP wychodzącego adresu IP rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806805"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="df34e-102">Zaniechanie zakresów wychodzących adresów IP EOP</span><span class="sxs-lookup"><span data-stu-id="df34e-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="df34e-103">Wykryliśmy potencjalne problemy w Twojej organizacji, które (jeśli nie zostały naprawione przed 26 października 2018 r.), mogą spowodować przerwanie przepływu poczty w lokalnych lub zewnętrznych obszarach docelowych.</span><span class="sxs-lookup"><span data-stu-id="df34e-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="df34e-104">Jak już się przekazało, aby uprościć zarządzanie zakresem adresów IP, konsolidujemy zakresy adresów IP usługi Exchange Online Protection (EOP) używane do wysyłania i odbierania wiadomości e-mail poza systemem Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="df34e-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="df34e-105">Nasze analizy wskazują, że jeden lub więcej zewnętrznych źródeł wiadomości e-mail lub lokalizacji docelowych skonfigurowanych w łącznikach przepływu poczty nie akceptuje połączeń z pokazanych [tu](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)zakresów adresów IP.</span><span class="sxs-lookup"><span data-stu-id="df34e-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="df34e-106">Przed 26 października możesz zapewnić, że te źródła i miejsca docelowe będą akceptować połączenia z wszystkimi [opublikowanymi adresami IP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)i ze wszystkich opublikowanych EOP.</span><span class="sxs-lookup"><span data-stu-id="df34e-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="df34e-107">Aby uzyskać więcej informacji na temat tej zmiany, zobacz wpisy w centrum wiadomości [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)lub [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="df34e-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="df34e-108">**Uwaga**: Jeśli poprzednio korzystano z publikowania adresów IP lub adresów URL za pomocą funkcji HTML, XML i RSS dla aktualizacji punktów końcowych, należy również przeprowadzić migrację do nowych usług sieci Web, aby zautomatyzować te typy aktualizacji.</span><span class="sxs-lookup"><span data-stu-id="df34e-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="df34e-109">Aby uzyskać więcej informacji, zobacz [Kategorie punktów końcowych microsoft 365 oraz usługa sieci Web microsoft 365 adres IP i adres URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="df34e-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
