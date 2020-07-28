---
title: Sterowanie automatycznymi aktualizacjami aplikacji pakietu Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439920"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="ebef5-102">Sterowanie automatycznymi aktualizacjami aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="ebef5-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="ebef5-103">Domyślnie aktualizacje aplikacji pakietu Office są pobierane automatycznie i stosowane w tle bez interwencji użytkownika.</span><span class="sxs-lookup"><span data-stu-id="ebef5-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="ebef5-104">Administratorzy mogą jednak kontrolować sposób stosowania aktualizacji przy użyciu ustawień aktualizacji pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="ebef5-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="ebef5-105">Ustawienia aktualizacji umożliwiają administratorom włączanie lub wyłączanie aktualizacji automatycznych, pokazywanie lub ukrywanie przycisku **Aktualizuj teraz** w pakiecie Office, ustawianie terminów aktualizacji i inne.</span><span class="sxs-lookup"><span data-stu-id="ebef5-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="ebef5-106">Aby uzyskać szczegółowe informacje, zobacz:</span><span class="sxs-lookup"><span data-stu-id="ebef5-106">For detailed information, see:</span></span>

- [<span data-ttu-id="ebef5-107">Konfigurowanie ustawień aktualizacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="ebef5-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="ebef5-108">Automatyczne aktualizowanie pakietu Office nie jest włączone</span><span class="sxs-lookup"><span data-stu-id="ebef5-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="ebef5-109">Definiowanie sposobu aktualizowania pakietu Office po zainstalowaniu</span><span class="sxs-lookup"><span data-stu-id="ebef5-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="ebef5-110">Aby przejrzeć istniejące ustawienia aktualizacji zastosowane do komputera klienckiego, wykonaj następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="ebef5-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="ebef5-111">Otwórz Edytor rejestru, przechodząc do **ekranu**  >  **startowego**  >  **regedit**.</span><span class="sxs-lookup"><span data-stu-id="ebef5-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="ebef5-112">Przełącz się do następującej lokalizacji i przejrzyj ustawienia aktualizacji pakietu Office:</span><span class="sxs-lookup"><span data-stu-id="ebef5-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="ebef5-113">a.</span><span class="sxs-lookup"><span data-stu-id="ebef5-113">a.</span></span> <span data-ttu-id="ebef5-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="ebef5-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="ebef5-115">b.</span><span class="sxs-lookup"><span data-stu-id="ebef5-115">b.</span></span> <span data-ttu-id="ebef5-116">ClickToRun\Konfiguracja</span><span class="sxs-lookup"><span data-stu-id="ebef5-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="ebef5-117">**Uwaga**  Jeśli jest ustawiony klucz OfficeMgmtCOM, w **Office**  >  **Account**  >  **aktualizacjech pakietu**Office może zostać wyświetlony komunikat "Aktualizacje są zarządzane przez administratora systemu".</span><span class="sxs-lookup"><span data-stu-id="ebef5-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="ebef5-118">Aby uzyskać więcej informacji, zobacz [Zarządzanie aktualizacjami aplikacji usługi Microsoft 365 za pomocą programu Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="ebef5-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  