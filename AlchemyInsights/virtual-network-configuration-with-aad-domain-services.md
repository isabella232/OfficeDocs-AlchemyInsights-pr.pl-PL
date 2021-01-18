---
title: Konfiguracja wirtualna z usługami domenowymi w usłudze AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885645"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Konfiguracja wirtualna z usługami domenowymi w usłudze AAD

Konfiguracja wirtualna z usługami domenowymi w usłudze AAD obejmuje następujące kroki: 

1. Sprawdzanie kondycji domeny w portalu Azure https://aka.ms/aadds-health
2. Sprawdzanie NSG dla reguł, które blokują porty potrzebne do synchronizacji w usługach domenowych w usłudze Azure AD w portalu https://aka.ms/aadds-networking
3. Sprawdzanie, czy sieć wirtualna jest wdrożona w tym samym regionie platformy Azure, co domena zarządzana przez usługi domenowe w usłudze Azure AD.
4. Upewnianie się, że nie masz istniejącej domeny z tą samą nazwą domeny dostępną w sieci wirtualnej.

Aby uzyskać więcej szczegółowych informacji na temat zagadnień dotyczących projektowania sieci wirtualnej platformy Azure do obsługi usług domenowych w usłudze AAD, zobacz [zagadnienia dotyczące sieci wirtualnej](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

