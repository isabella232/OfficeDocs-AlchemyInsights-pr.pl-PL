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
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="48737-102">Zmienianie ustawień ograniczania usługi EWS</span><span class="sxs-lookup"><span data-stu-id="48737-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="48737-103">Uruchom nasz automatyczny test, który umożliwi zmodyfikowanie zasad ograniczania usługi EWS na czas trwania migracji.</span><span class="sxs-lookup"><span data-stu-id="48737-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="48737-104">Pamiętaj, że nawet po uruchomieniu tego testu import usługi EWS będzie nadal ograniczony do 150 MB przez 5 minut na skrzynkę pocztową. Aby zwiększyć przepustowość migracji, migruj więcej użytkowników współbieżnie.</span><span class="sxs-lookup"><span data-stu-id="48737-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="48737-105">Pamiętaj, że zmiany zasad ograniczania usługi EWS nie wpływają na następujące typy migracji (za pomocą narzędzi firmy Microsoft): migracja hybrydowa, migracja jednorazowa/etapowa (RPC/HTTP), IMAP, G Suite, folder publiczny lub usługa importowania plików PST.</span><span class="sxs-lookup"><span data-stu-id="48737-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>