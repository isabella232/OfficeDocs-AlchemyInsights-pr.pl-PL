---
title: Pomoc techniczna Microsoft Edge na potrzeby aplikacji Microsoft Defender Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584015"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="2042c-102">Pomoc techniczna Microsoft Edge na potrzeby aplikacji Microsoft Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="2042c-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="2042c-103">Funkcja Application Guard przeznaczona dla systemu Windows 10 i Microsoft Edge korzysta z podejścia do izolacji sprzętu, które umożliwia użytkownikowi nawigację po niezaufanej witrynie wewnątrz izolowanego kontenera funkcji Hyper-V, oddzielonym od systemu operacyjnego hosta.</span><span class="sxs-lookup"><span data-stu-id="2042c-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="2042c-104">Administrator przedsiębiorstwa zdefiniował listę zaufanych witryn internetowych, zasobów chmur i sieci wewnętrznych.</span><span class="sxs-lookup"><span data-stu-id="2042c-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="2042c-105">Gdy użytkownik odwiedzi witrynę, której nie ma na liście, program Microsoft Edge otworzy witrynę w kontenerze.</span><span class="sxs-lookup"><span data-stu-id="2042c-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="2042c-106">Oznacza to, że jeśli witryna stanie się szkodliwa, komputer hosta pozostanie chroniony, a osoba atakująca nie będzie mogła uzyskać dostępu do danych przedsiębiorstwa.</span><span class="sxs-lookup"><span data-stu-id="2042c-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="2042c-107">Instalacja rozszerzeń w kontenerze jest obsługiwana w programie Microsoft Edge w wersji 81 i może być kontrolowana za pośrednictwem zasad.</span><span class="sxs-lookup"><span data-stu-id="2042c-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="2042c-108">Adres updateURL, który jest wykorzystywany w zasadach ExtensionInstallForcelist, należy dodać jako zasób neutralny w zasadach izolacji sieciowej, które są używane przez funkcję Application Guard.</span><span class="sxs-lookup"><span data-stu-id="2042c-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="2042c-109">Aby uzyskać więcej informacji, zobacz [Pomoc techniczna Microsoft Edge dla usługi Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="2042c-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
