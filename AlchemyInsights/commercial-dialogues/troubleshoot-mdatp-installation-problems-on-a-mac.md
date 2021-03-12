---
title: Rozwiązywanie problemów z instalacją MDATP na komputerze Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749773"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="6dafe-102">Rozwiązywanie problemów z instalacją MDATP na komputerze Mac</span><span class="sxs-lookup"><span data-stu-id="6dafe-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="6dafe-103">Jeśli instalacja ręczna nie powiedzie się, **na stronie Podsumowanie** kreatora instalacji jest wyświetlany następujący błąd:</span><span class="sxs-lookup"><span data-stu-id="6dafe-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="6dafe-104">"Wystąpił błąd podczas instalacji.</span><span class="sxs-lookup"><span data-stu-id="6dafe-104">"An error occurred during installation.</span></span> <span data-ttu-id="6dafe-105">Instalator napotkał błąd, który powodował niepowodzenie instalacji.</span><span class="sxs-lookup"><span data-stu-id="6dafe-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="6dafe-106">Aby uzyskać pomoc, skontaktuj się z producentem oprogramowania".</span><span class="sxs-lookup"><span data-stu-id="6dafe-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="6dafe-107">W przypadku wdrożeń MDM na stronie przedstawiono również ogólny błąd instalacji.</span><span class="sxs-lookup"><span data-stu-id="6dafe-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="6dafe-108">Chociaż użytkownicy końcowi nie wyświetlają dokładnych błędów, plik dziennika jest w toku instalacji, w **/Library/Logs/Microsoft/mdatp/install.log.**</span><span class="sxs-lookup"><span data-stu-id="6dafe-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="6dafe-109">Każda sesja instalacji jest dołączana do tego pliku dziennika.</span><span class="sxs-lookup"><span data-stu-id="6dafe-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="6dafe-110">Aby wy wyprowadzić tylko ostatnią sesję instalacji, użyj `sed` .</span><span class="sxs-lookup"><span data-stu-id="6dafe-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="6dafe-111">Aby dowiedzieć się więcej, zobacz Rozwiązywanie problemów z instalacją [programu Microsoft Defender ATP dla komputerów Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)</span><span class="sxs-lookup"><span data-stu-id="6dafe-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
