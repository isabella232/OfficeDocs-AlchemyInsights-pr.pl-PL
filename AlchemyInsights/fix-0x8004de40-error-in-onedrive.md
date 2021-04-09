---
title: Naprawianie 0x8004de40 w usłudze OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649758"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="32892-102">Naprawianie 0x8004de40 w usłudze OneDrive</span><span class="sxs-lookup"><span data-stu-id="32892-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="32892-103">Jeśli używasz systemu Windows 7 i otrzymujesz ten błąd, zaktualizuj go, aby włączyć [protokoły TLS 1.1 i TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)jako domyślne protokoły bezpiecznego w systemie WinHTTP w systemie Windows.</span><span class="sxs-lookup"><span data-stu-id="32892-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="32892-104">Jeśli używasz systemu Windows 10 i jest wyświetlany komunikat o błędzie 0x8004de40 usługi OneDrive:</span><span class="sxs-lookup"><span data-stu-id="32892-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="32892-105">Uruchom ponownie komputer, którego dotyczy problem, podczas połączenia z domeną katalogu Acitve.</span><span class="sxs-lookup"><span data-stu-id="32892-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="32892-106">Jeśli ponowne uruchomienie nie rozwiąże problemu, rozłącz i ponownie dołącz do urządzenia z usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="32892-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="32892-107">**Uwaga:** podczas wykonywania tych czynności powinno się być w sieci firmowej.</span><span class="sxs-lookup"><span data-stu-id="32892-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="32892-108">Nie wykonuj tych czynności, gdy nie masz połączenia z infrastrukturą firmową (na przykład w podróży).</span><span class="sxs-lookup"><span data-stu-id="32892-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="32892-109">Otwórz wiersz polecenia z podwyższonym poziomem uprawnień, wybierając **przycisk Start**, kliknij prawym przyciskiem myszy pozycję Wiersz **polecenia**, a następnie wybierz pozycję Uruchom **jako administrator.**</span><span class="sxs-lookup"><span data-stu-id="32892-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="32892-110">Wpisz *dsregcmd /leave i* naciśnij klawisz **Enter.**</span><span class="sxs-lookup"><span data-stu-id="32892-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="32892-111">Po zakończeniu wpisz *dsregcmd /join* i naciśnij klawisz **Enter.**</span><span class="sxs-lookup"><span data-stu-id="32892-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="32892-112">Po zakończeniu zamknij wiersz polecenia.</span><span class="sxs-lookup"><span data-stu-id="32892-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="32892-113">Uruchom ponownie komputer i zaloguj się do usługi OneDrive.</span><span class="sxs-lookup"><span data-stu-id="32892-113">Reboot the computer, and log into OneDrive.</span></span>