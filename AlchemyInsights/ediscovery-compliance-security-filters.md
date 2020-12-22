---
title: W trakcie wyszukiwania i eksportowania zawartości nie są zwracane żadne wyniki
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727233"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="60db4-102">W trakcie wyszukiwania i eksportowania zawartości nie są zwracane żadne wyniki</span><span class="sxs-lookup"><span data-stu-id="60db4-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="60db4-103">Jeśli występują problemy z następującymi scenariuszami zbierania elektronicznych materiałów dowodowych:</span><span class="sxs-lookup"><span data-stu-id="60db4-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="60db4-104">Funkcja wyszukiwania zawartości/eksportowania nie zwraca żadnych danych lub nieoczekiwanych danych</span><span class="sxs-lookup"><span data-stu-id="60db4-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="60db4-105">Błąd wyszukiwania lub eksportu zbierania elektronicznych materiałów dowodowych</span><span class="sxs-lookup"><span data-stu-id="60db4-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="60db4-106">Może to być spowodowane pewnymi filtrami zabezpieczeń zgodności, które zostały skonfigurowane przez określonego administratora i nie są przekazywane do wszystkich administratorów.</span><span class="sxs-lookup"><span data-stu-id="60db4-106">This may be due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="60db4-107">Aby to naprawić, sprawdź, czy istnieją filtry zabezpieczeń zgodności, które mogą powodować następujące problemy:</span><span class="sxs-lookup"><span data-stu-id="60db4-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="60db4-108">Nawiązywanie połączenia z programem PowerShell w centrum zabezpieczeń i zgodności</span><span class="sxs-lookup"><span data-stu-id="60db4-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="60db4-109">Uruchom następujące commandlets:</span><span class="sxs-lookup"><span data-stu-id="60db4-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="60db4-110">Aby uzyskać dodatkowe informacje na temat filtrów zabezpieczeń zgodności, zobacz [filtrowanie uprawnień do wyszukiwania zawartości](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="60db4-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
