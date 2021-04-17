---
title: Zmienianie ustawień ograniczania usługi EWS
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818046"
---
# <a name="changing-ews-throttling-settings"></a>Zmienianie ustawień ograniczania usługi EWS

Uruchom nasz automatyczny test, który umożliwi zmodyfikowanie zasad ograniczania usługi EWS na czas trwania migracji. Pamiętaj, że nawet po uruchomieniu tego testu import usługi EWS będzie nadal ograniczony do 150 MB przez 5 minut na skrzynkę pocztową. Aby zwiększyć przepustowość migracji, migruj więcej użytkowników współbieżnie.

Pamiętaj, że zmiany zasad ograniczania usługi EWS nie wpływają na następujące typy migracji (za pomocą narzędzi firmy Microsoft): migracja hybrydowa, migracja jednorazowa/etapowa (RPC/HTTP), IMAP, G Suite, folder publiczny lub usługa importowania plików PST.