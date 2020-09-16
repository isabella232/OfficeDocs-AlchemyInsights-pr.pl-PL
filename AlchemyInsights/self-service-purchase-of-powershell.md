---
title: Zakup samoobsługowy programu PowerShell
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
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739980"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="38a06-102">Zakup samoobsługowy programu PowerShell</span><span class="sxs-lookup"><span data-stu-id="38a06-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="38a06-103">Aby użyć modułu programu PowerShell w programie MSCommerce, należy zainstalować go na urządzeniu z systemem Windows 10 z szyfrowaniem TLS 1,2 (wymagane są uprawnienia administratora lokalnego).</span><span class="sxs-lookup"><span data-stu-id="38a06-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="38a06-104">Zaimportuj i Połącz się z modułem MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="38a06-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="38a06-105">Gdy zostanie wyświetlony monit o zalogowanie się, musisz skorzystać z poświadczeń roli administratora globalnego lub rozliczeniowego.</span><span class="sxs-lookup"><span data-stu-id="38a06-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="38a06-106">Jeśli nie masz protokołu TLS 1,2, podczas próby uzyskania lub zaktualizowania zasad może zostać wyświetlony następujący komunikat o błędzie:</span><span class="sxs-lookup"><span data-stu-id="38a06-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="38a06-107">*ErrorMessage — połączenie podstawowe zostało przerwane: podczas wysyłania wystąpił nieoczekiwany błąd*.</span><span class="sxs-lookup"><span data-stu-id="38a06-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



