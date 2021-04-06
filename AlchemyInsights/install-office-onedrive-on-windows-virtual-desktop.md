---
title: Instalowanie pakietu Office i usługi OneDrive na pulpicie wirtualnym systemu Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595844"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a><span data-ttu-id="00554-102">Instalowanie pakietu Office i usługi OneDrive na pulpicie wirtualnym systemu Windows</span><span class="sxs-lookup"><span data-stu-id="00554-102">Install Office and OneDrive on Windows Virtual Desktop</span></span>

1. <span data-ttu-id="00554-103">[Przygotowywanie i dostosowywanie wzorca obrazu VHD.](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image)</span><span class="sxs-lookup"><span data-stu-id="00554-103">[Prepare and customize a master VHD image](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span></span> <span data-ttu-id="00554-104">Tworzenie maszyny wirtualnej, jeśli nie została jeszcze utworzona.</span><span class="sxs-lookup"><span data-stu-id="00554-104">Create a virtual machine (VM) if it hasn't already been created.</span></span>

1. <span data-ttu-id="00554-105">[Zainstaluj pakiet Office w trybie aktywacji na komputerze udostępnionym.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode)</span><span class="sxs-lookup"><span data-stu-id="00554-105">[Install Office in shared computer activation mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span></span> <span data-ttu-id="00554-106">Aktywacja na komputerze udostępnionym umożliwia wielu użytkownikom uzyskiwanie dostępu do pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="00554-106">Shared computer activation allows multiple users to access Office.</span></span>

1. <span data-ttu-id="00554-107">[Zainstaluj aplikację OneDrive w trybie dla 1 komputera.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode)</span><span class="sxs-lookup"><span data-stu-id="00554-107">[Install OneDrive in per-machine mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span></span> <span data-ttu-id="00554-108">Zwykle oneDrive jest instalowany na użytkownika, ale tutaj powinna zostać zainstalowana na komputerze.</span><span class="sxs-lookup"><span data-stu-id="00554-108">Normally, OneDrive is installed per user, but here, it should be installed per machine.</span></span>