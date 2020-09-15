---
title: Nawiązywanie połączenia z modułem MSCommerce
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3528"
ms.openlocfilehash: 41dd044d99d14f25ea15699bfb74f7c37e3928c1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713248"
---
# <a name="connect-to-the-mscommerce-module"></a><span data-ttu-id="35425-102">Nawiązywanie połączenia z modułem MSCommerce</span><span class="sxs-lookup"><span data-stu-id="35425-102">Connect to the MSCommerce module</span></span>

<span data-ttu-id="35425-103">Musisz mieć połączenie z modułem MSCommerce, aby móc wyświetlać lub ustawiać zasady AllowSelfServicePurchase.</span><span class="sxs-lookup"><span data-stu-id="35425-103">You must be connected to the MSCommerce module before you can view or set the AllowSelfServicePurchase policy.</span></span>  

<span data-ttu-id="35425-104">Aby połączyć się z modułem MSCommerce, w wierszu polecenia programu PowerShell (PS C: \) wprowadź następujące polecenie:</span><span class="sxs-lookup"><span data-stu-id="35425-104">To connect to the MSCommerce module, at the PowerShell prompt (PS C:\), enter the following command:</span></span>

`Connect-MSCommerce`

<span data-ttu-id="35425-105">Spowoduje to otwarcie okna dialogowego logowania.</span><span class="sxs-lookup"><span data-stu-id="35425-105">This will open a sign-in dialog.</span></span> <span data-ttu-id="35425-106">Wprowadź swoją nazwę użytkownika i hasło, aby się zalogować.</span><span class="sxs-lookup"><span data-stu-id="35425-106">Enter your username and password to sign-in.</span></span>

<span data-ttu-id="35425-107">**Uwaga:** &nbsp; &nbsp; Konto użyte do zalogowania się musi być kontem firmowym lub administratorem rozliczeń.</span><span class="sxs-lookup"><span data-stu-id="35425-107">**NOTE:**&nbsp;&nbsp;The account used to sign in must be a Company or Billing Administrator.</span></span>
