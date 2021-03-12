---
title: Problemy z instalowaniem programu Microsoft Defender na komputerach Mac lub Linux
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
- "6028"
- "9001222"
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713841"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="602b8-102">Problemy z instalowaniem programu Microsoft Defender na komputerach Mac lub Linux</span><span class="sxs-lookup"><span data-stu-id="602b8-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="602b8-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="602b8-103">**Mac**</span></span>

- <span data-ttu-id="602b8-104">Przed zainstalowaniem programu Microsoft Defender ATP dla komputerów Mac upewnij się, że są spełnione wymagania systemowe.</span><span class="sxs-lookup"><span data-stu-id="602b8-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="602b8-105">Aby uzyskać więcej informacji, zobacz [Jak zainstalować program Microsoft Defender ATP dla komputerów Mac.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)</span><span class="sxs-lookup"><span data-stu-id="602b8-105">For more info, see [How to install Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="602b8-106">Przejrzyj informacje w pliku: "/Library/Logs/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="602b8-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="602b8-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="602b8-107">**Linux**</span></span>

- <span data-ttu-id="602b8-108">Przed zainstalowaniem programu Microsoft Defender ATP dla systemu Linux upewnij się, że są spełnione wymagania systemowe.</span><span class="sxs-lookup"><span data-stu-id="602b8-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="602b8-109">Aby uzyskać więcej informacji, zobacz [Jak zainstalować program Microsoft Defender ATP dla systemu Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="602b8-109">For more info, see [How to install Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="602b8-110">Aby sprawdzić, czy usługa MDATP jest uruchomiona, zobacz [Instalacja nie powiodła się.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)</span><span class="sxs-lookup"><span data-stu-id="602b8-110">To verify that MDATP service is running, see [Installation failed](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="602b8-111">Aby rozwiązać i rozwiązać problemy, jeśli usługa nie jest uruchomiona, zobacz Kroki rozwiązywania problemów, jeśli usługa [MDATP nie jest uruchomiona.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)</span><span class="sxs-lookup"><span data-stu-id="602b8-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="602b8-112">Instrukcje sprawdzania konfiguracji klienta, sprawdzania kondycji produktu i uruchamiania testu wykrywania w pliku tekstowym EICAR można znaleźć w [teście konfiguracji klienta.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)</span><span class="sxs-lookup"><span data-stu-id="602b8-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="602b8-113">**Uwaga** Aby uzyskać listę obsługiwanych systemów plików do obsługi aktywności w dostępie, zobacz [Microsoft Defender ATP dla systemu Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="602b8-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>