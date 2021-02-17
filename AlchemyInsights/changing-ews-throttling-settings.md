---
title: Zmienianie ustawień ograniczania usługi EWS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075907"
---
# <a name="changing-ews-throttling-settings"></a>Zmienianie ustawień ograniczania usługi EWS

Uruchom nasz automatyczny test, który umożliwi zmodyfikowanie zasad ograniczania usługi EWS na czas trwania migracji. Pamiętaj, że nawet po uruchomieniu tego testu import usługi EWS będzie nadal ograniczony do 150 MB przez 5 minut na skrzynkę pocztową. Aby zwiększyć przepustowość migracji, migruj więcej użytkowników współbieżnie.

Pamiętaj, że zmiany zasad ograniczania usługi EWS nie wpływają na następujące typy migracji (za pomocą narzędzi firmy Microsoft): migracja hybrydowa, migracja jednorazowa/etapowa (RPC/HTTP), IMAP, G Suite, folder publiczny lub usługa importowania plików PST.