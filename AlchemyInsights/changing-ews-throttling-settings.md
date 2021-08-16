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
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968387"
---
# <a name="changing-ews-throttling-settings"></a>Zmienianie ustawień ograniczania usługi EWS

Uruchom nasz automatyczny test, który umożliwi zmodyfikowanie zasad ograniczania usługi EWS na czas trwania migracji. Pamiętaj, że nawet po uruchomieniu tego testu import usługi EWS będzie nadal ograniczony do 150 MB przez 5 minut na skrzynkę pocztową. Aby zwiększyć przepustowość migracji, migruj więcej użytkowników współbieżnie.

Pamiętaj, że zmiany zasad ograniczania usługi EWS nie wpływają na następujące typy migracji (za pomocą narzędzi firmy Microsoft): migracja hybrydowa, migracja jednorazowa/etapowa (RPC/HTTP), IMAP, G Suite, folder publiczny lub usługa importowania plików PST.