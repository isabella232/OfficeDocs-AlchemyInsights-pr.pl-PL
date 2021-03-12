---
title: Konfigurowanie wykluczeń dla skanowania ATP programu Microsoft Defender
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
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713901"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="9d730-102">Konfigurowanie wykluczeń dla skanowania ATP programu Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="9d730-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="9d730-103">Na ogół możesz wykluczyć określone rozszerzenia plików i lokalizacje folderów z skanów Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="9d730-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="9d730-104">Możesz również skonfigurować wykluczenia dla plików otwieranych przez określone procesy.</span><span class="sxs-lookup"><span data-stu-id="9d730-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="9d730-105">Aby uzyskać więcej [informacji,](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) zobacz konfigurowanie i weryfikowanie wykluczeń na podstawie rozszerzenia pliku i lokalizacji folderu oraz Konfigurowanie wykluczeń dla plików otwieranych [przez procesy.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="9d730-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="9d730-106">Aby skonfigurować wykluczenia w systemie **Windows Server 2016 i 2019,** zobacz Konfigurowanie wykluczeń programu [antywirusowego Microsoft Defender w systemie Windows Server.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="9d730-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="9d730-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="9d730-107">**Mac**</span></span>

<span data-ttu-id="9d730-108">Aby uzyskać szczegółowe informacje na temat obsługiwanych typów wykluczeń i konfigurowania listy wykluczeń dla komputerów Mac, zobacz Obsługiwane typy wykluczeń oraz Jak skonfigurować [listę wykluczeń.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions) [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="9d730-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="9d730-109">**Uwaga** Możesz również sprawdzić, czy listy wykluczeń są wykluczeń, korzystając z pliku testowego EICAR.</span><span class="sxs-lookup"><span data-stu-id="9d730-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="9d730-110">Aby uzyskać więcej informacji, zobacz [weryfikację list wykluczeń za pomocą pliku testowego EICAR.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="9d730-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="9d730-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="9d730-111">**Linux**</span></span>

<span data-ttu-id="9d730-112">Aby uzyskać szczegółowe informacje na temat obsługiwanych typów wykluczeń i konfigurowania listy wykluczeń dla systemu Linux, zobacz Obsługiwane typy wykluczeń oraz Konfigurowanie i weryfikowanie wykluczeń dla programu [Microsoft Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)dla systemu Linux. [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="9d730-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="9d730-113">**Uwaga** Możesz również sprawdzić, czy listy wykluczeń są wykluczeń, korzystając z pliku testowego EICAR.</span><span class="sxs-lookup"><span data-stu-id="9d730-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="9d730-114">Aby uzyskać więcej informacji, zobacz [weryfikację list wykluczeń za pomocą pliku testowego EICAR.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="9d730-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 