---
title: Ustaw wartość ClientAccessServerEnabled na True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749981"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="326de-102">Ustaw wartość ClientAccessServerEnabled na True</span><span class="sxs-lookup"><span data-stu-id="326de-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="326de-103">Jeśli nie możesz otworzyć zaszyfrowanej wiadomości e-mail i zamiast tego zobaczysz **załącznik,** wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="326de-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="326de-104">Połącz się z programem PowerShell dla usługi Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="326de-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="326de-105">Aby nawiązać połączenie z programem PowerShell dla usługi Exchange Online, musisz zalogować się przy użyciu konta administratora globalnego lub administratora programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="326de-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="326de-106">a.</span><span class="sxs-lookup"><span data-stu-id="326de-106">a.</span></span> <span data-ttu-id="326de-107">Otwórz program Windows PowerShell, a następnie uruchom następujące polecenie: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="326de-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="326de-108">b.</span><span class="sxs-lookup"><span data-stu-id="326de-108">b.</span></span> <span data-ttu-id="326de-109">W **oknie dialogowym** Żądanie poświadczeń programu Windows PowerShell wprowadź swoje konto służbowe i hasło, c.</span><span class="sxs-lookup"><span data-stu-id="326de-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="326de-110">Kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="326de-110">Click **OK**.</span></span> 

2. <span data-ttu-id="326de-111">Uruchom następujące polecenie, aby utworzyć nową sesję:</span><span class="sxs-lookup"><span data-stu-id="326de-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="326de-112">a.</span><span class="sxs-lookup"><span data-stu-id="326de-112">a.</span></span> <span data-ttu-id="326de-113">Uruchom następujące polecenie:</span><span class="sxs-lookup"><span data-stu-id="326de-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="326de-114">Polecenie `Get-IRMConfiguration` Uruchom.</span><span class="sxs-lookup"><span data-stu-id="326de-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="326de-115">Sprawdź ustawienie **ClientAccessServerEnabled.**</span><span class="sxs-lookup"><span data-stu-id="326de-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="326de-116">a.</span><span class="sxs-lookup"><span data-stu-id="326de-116">a.</span></span> <span data-ttu-id="326de-117">Jeśli **ustawienie ClientAccessServerEnabled** ma ustawioną wartość **False,** uruchom następujące polecenie cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="326de-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="326de-118">Zawsze zamykaj sesję programu PowerShell za pomocą następującego polecenia: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="326de-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="326de-119">Aby uzyskać więcej informacji, zobacz [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="326de-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

