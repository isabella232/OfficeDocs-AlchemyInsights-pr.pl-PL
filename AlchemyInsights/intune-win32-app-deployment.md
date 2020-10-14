---
title: Wdrożenie aplikacji Intune Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461875"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="933ec-102">Wdrożenie aplikacji Intune Win32</span><span class="sxs-lookup"><span data-stu-id="933ec-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="933ec-103">Usługa Microsoft Intune umożliwia aplikacjom systemu Win32, między innymi MSI i bez ograniczeń. EXE, który ma zostać wdrożony na urządzeniach z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="933ec-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="933ec-104">Do korzystania z tego mechanizmu wdrażania jest wymagane rozszerzenie zarządzania usługą Intune (IME) na urządzeniu docelowym.</span><span class="sxs-lookup"><span data-stu-id="933ec-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="933ec-105">Edytor IME zostanie zainstalowany automatycznie w wyniku przekierowania skryptu programu PowerShell lub wdrożenia aplikacji systemu Win32 do użytkownika/urządzenia.</span><span class="sxs-lookup"><span data-stu-id="933ec-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="933ec-106">Ponadto są dostępne wymagania wstępne, które muszą być spełnione w celu wdrożenia aplikacji Win32 zawierających następujące funkcje:</span><span class="sxs-lookup"><span data-stu-id="933ec-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="933ec-107">Obsługiwane platformy: Windows 10 w wersji 1607 lub nowszej (wersje Enterprise, Pro i Education).</span><span class="sxs-lookup"><span data-stu-id="933ec-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="933ec-108">Obsługiwana architektura: x86 i x64.</span><span class="sxs-lookup"><span data-stu-id="933ec-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="933ec-109">Zarządzanie urządzeniami: dołączona i automatycznie zarejestrowana w usłudze AAD (w tym przyłączone domeny hybrydowe i zasady grupy są automatycznie rejestrowane).</span><span class="sxs-lookup"><span data-stu-id="933ec-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="933ec-110">Format pakietu aplikacji:. **intunewin**  plik przygotowany za pomocą [narzędzia Microsoft Win32 Content przygotowywanie](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="933ec-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="933ec-111">Określone</span><span class="sxs-lookup"><span data-stu-id="933ec-111">Limitations:</span></span>
    - <span data-ttu-id="933ec-112">Maksymalny rozmiar: 8 GB.</span><span class="sxs-lookup"><span data-stu-id="933ec-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="933ec-113">Nieobsługiwana architektura: poręcze.</span><span class="sxs-lookup"><span data-stu-id="933ec-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="933ec-114">Przejrzyj dokument "[Dodawanie, przypisywanie i monitorowanie aplikacji systemu Win32 w usłudze Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)", aby uzyskać informacje dotyczące tych kroków.</span><span class="sxs-lookup"><span data-stu-id="933ec-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="933ec-115">Szczegółowe informacje dotyczące rozwiązywania problemów z wdrażaniem aplikacji w systemie Windows, w tym aplikacje systemu Win32, można przejrzeć w następujących dokumentach</span><span class="sxs-lookup"><span data-stu-id="933ec-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="933ec-116">Rozwiązywanie problemów z instalacją aplikacji</span><span class="sxs-lookup"><span data-stu-id="933ec-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="933ec-117">Rozwiązywanie problemów z aplikacjami Win32</span><span class="sxs-lookup"><span data-stu-id="933ec-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)