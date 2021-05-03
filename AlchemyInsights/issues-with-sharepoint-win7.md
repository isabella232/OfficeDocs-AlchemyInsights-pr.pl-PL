---
title: Problemy z SharePoint na Windows 7 komputerów
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
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/28/2021
ms.locfileid: "52125513"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a><span data-ttu-id="5aa15-102">Problemy z SharePoint na Windows 7 komputerów</span><span class="sxs-lookup"><span data-stu-id="5aa15-102">Issues with SharePoint on Windows 7 machines</span></span>

<span data-ttu-id="5aa15-103">Błędy, które wystąpiły na Windows 7 komputerach podczas pracy z programem SharePoint lub OneDrive, mogą być związane z dezkonywacją TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="5aa15-103">If you receive errors on Windows 7 machines while working on SharePoint or OneDrive, they might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="5aa15-104">Aby uzyskać więcej informacji, zobacz:</span><span class="sxs-lookup"><span data-stu-id="5aa15-104">For more information, see:</span></span>

- [<span data-ttu-id="5aa15-105">Przygotowanie do protokołu TLS 1.2 w usłudze Office 365 i usłudze Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="5aa15-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- <span data-ttu-id="5aa15-106">Windows 7 z dodatkiem SP1/Windows 8 muszą mieć włączoną obsługę TLS1.2.</span><span class="sxs-lookup"><span data-stu-id="5aa15-106">Windows 7 SP1/Windows 8 clients must have TLS1.2 enabled.</span></span> <span data-ttu-id="5aa15-107">Aby uzyskać więcej informacji, zobacz Błędy uwierzytelniania występują, gdy klient nie ma obsługi [protokołu TLS 1.2.](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span><span class="sxs-lookup"><span data-stu-id="5aa15-107">For more information, see [Authentication errors occur when client doesn't have TLS 1.2 support](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span></span>

- <span data-ttu-id="5aa15-108">Zainstaluj aktualizację KB3140245 i utwórz wartość rejestru.</span><span class="sxs-lookup"><span data-stu-id="5aa15-108">Install KB3140245 and create the registry value.</span></span> <span data-ttu-id="5aa15-109">Aby uzyskać więcej informacji, zobacz Aktualizowanie w celu włączenia [protokołów TLS 1.1 i TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) jako domyślnych protokołów bezpiecznego w winieHTTP w Windows</span><span class="sxs-lookup"><span data-stu-id="5aa15-109">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span></span>

- <span data-ttu-id="5aa15-110">Windows 7 z dodatkiem SP1/Windows 8 muszą upewnić się, że są zainstalowane najnowsze pakiety szyfrowania TLS.</span><span class="sxs-lookup"><span data-stu-id="5aa15-110">Windows 7 SP1/Windows 8 clients must ensure latest TLS cipher suites are installed.</span></span> <span data-ttu-id="5aa15-111">Aby uzyskać więcej informacji, zobacz [Porada firmy Microsoft ds. zabezpieczeń 3042058.](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058)</span><span class="sxs-lookup"><span data-stu-id="5aa15-111">For more information, see [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span></span> 


