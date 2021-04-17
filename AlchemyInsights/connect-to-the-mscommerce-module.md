---
title: Nawiązywanie połączenia z modułem MS Commerce
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3528"
ms.openlocfilehash: e77c6a329ac99a4cea4f143dcb3c661b6a518e35
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817038"
---
# <a name="connect-to-the-mscommerce-module"></a><span data-ttu-id="50098-102">Nawiązywanie połączenia z modułem MS Commerce</span><span class="sxs-lookup"><span data-stu-id="50098-102">Connect to the MSCommerce module</span></span>

<span data-ttu-id="50098-103">Aby można było wyświetlić lub skonfigurować zasady AllowSelfServicePurchase, musisz mieć połączenie z modułem MS Commerce.</span><span class="sxs-lookup"><span data-stu-id="50098-103">You must be connected to the MSCommerce module before you can view or set the AllowSelfServicePurchase policy.</span></span>  

<span data-ttu-id="50098-104">Aby nawiązać połączenie z modułem MS Commerce, w wierszu polecenia programu PowerShell (PS C: \) wprowadź następujące polecenie:</span><span class="sxs-lookup"><span data-stu-id="50098-104">To connect to the MSCommerce module, at the PowerShell prompt (PS C:\), enter the following command:</span></span>

`Connect-MSCommerce`

<span data-ttu-id="50098-105">Spowoduje to otwarcie okna dialogowego logowania.</span><span class="sxs-lookup"><span data-stu-id="50098-105">This will open a sign-in dialog.</span></span> <span data-ttu-id="50098-106">Wprowadź swoją nazwę użytkownika i hasło, aby się zalogować.</span><span class="sxs-lookup"><span data-stu-id="50098-106">Enter your username and password to sign-in.</span></span>

<span data-ttu-id="50098-107">**UWAGA:** &nbsp; &nbsp; Konto użyte do zalogowania się musi być kontem firmy lub administratorem rozliczeń.</span><span class="sxs-lookup"><span data-stu-id="50098-107">**NOTE:**&nbsp;&nbsp;The account used to sign in must be a Company or Billing Administrator.</span></span>
