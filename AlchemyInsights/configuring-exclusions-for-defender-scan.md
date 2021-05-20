---
title: Konfigurowanie wykluczeń do Microsoft Defender ATP skanowania
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543695"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="2296b-102">Konfigurowanie wykluczeń do Microsoft Defender ATP skanowania</span><span class="sxs-lookup"><span data-stu-id="2296b-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="2296b-103">Na ogół możesz wykluczyć pewne rozszerzenia plików i lokalizacje folderów z Microsoft Defender ATP skanów.</span><span class="sxs-lookup"><span data-stu-id="2296b-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="2296b-104">Możesz również skonfigurować wykluczenia dla plików otwieranych w określonych procesach.</span><span class="sxs-lookup"><span data-stu-id="2296b-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="2296b-105">Aby uzyskać więcej informacji, zobacz [Konfigurowanie](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) i weryfikowanie wykluczeń na podstawie rozszerzenia pliku i lokalizacji folderu oraz Konfigurowanie wykluczeń plików otwieranych [przez procesy.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="2296b-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="2296b-106">Aby skonfigurować wykluczenia dla programu **Windows Server 2016 i 2019,** zobacz Konfigurowanie Program antywirusowy Microsoft Defender wykluczeń [na Windows Server.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="2296b-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="2296b-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="2296b-107">**Mac**</span></span>

<span data-ttu-id="2296b-108">Aby uzyskać szczegółowe informacje na temat obsługiwanych typów wykluczeń i konfigurowania listy wykluczeń dla komputerów Mac, zobacz Obsługiwane typy wykluczeń i Jak skonfigurować [listę wykluczeń.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions) [](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="2296b-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="2296b-109">**Uwaga** Możesz również sprawdzić poprawność wykluczeń przy użyciu pliku testowego EICAR.</span><span class="sxs-lookup"><span data-stu-id="2296b-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="2296b-110">Aby uzyskać więcej informacji, zobacz Sprawdzanie poprawności [wykluczeń za pomocą pliku testowego EICAR.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="2296b-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="2296b-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="2296b-111">**Linux**</span></span>

<span data-ttu-id="2296b-112">Aby uzyskać szczegółowe informacje na temat obsługiwanych typów wykluczeń i konfigurowania listy wykluczeń dla systemu Linux, zobacz Obsługiwane typy wykluczeń oraz Konfigurowanie i weryfikowanie wykluczeń dla systemu [Microsoft Defender ATP Linux.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions) [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="2296b-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="2296b-113">**Uwaga** Możesz również sprawdzić poprawność wykluczeń przy użyciu pliku testowego EICAR.</span><span class="sxs-lookup"><span data-stu-id="2296b-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="2296b-114">Aby uzyskać więcej informacji, zobacz Sprawdzanie poprawności [wykluczeń za pomocą pliku testowego EICAR.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="2296b-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 