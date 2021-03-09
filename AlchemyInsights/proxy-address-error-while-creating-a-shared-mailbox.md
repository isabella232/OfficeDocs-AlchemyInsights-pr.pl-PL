---
title: Błąd adresu serwera proxy podczas tworzenia udostępnionej skrzynki pocztowej
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568300"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="8eb5e-102">Błąd adresu serwera proxy podczas tworzenia skrzynki pocztowej lub innego obiektu z włączoną obsługą poczty e-mail</span><span class="sxs-lookup"><span data-stu-id="8eb5e-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="8eb5e-103">Jeśli podczas próby utworzenia obiektu z obsługą poczty e-mail (skrzynka pocztowa, udostępniona skrzynka pocztowa itp.) jest wyświetlany komunikat o błędzie "Adres serwera proxy "SMTP:alias@domain.com" jest już używany...", wybrany adres e-mail jest już używany przez inny obiekt w organizacji z obsługą poczty e-mail.</span><span class="sxs-lookup"><span data-stu-id="8eb5e-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="8eb5e-104">Musisz znaleźć użytkownika, grupę, udostępnioną skrzynkę pocztową lub folder publiczny z tym adresem e-mail i usunąć go lub zmienić jego adres e-mail.</span><span class="sxs-lookup"><span data-stu-id="8eb5e-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="8eb5e-105">Następnie możesz utworzyć nowy obiekt z obsługą poczty e-mail z darmowym adresem e-mail.</span><span class="sxs-lookup"><span data-stu-id="8eb5e-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="8eb5e-106">Użyj funkcji wyszukiwania na stronie głównej, aby ją znaleźć.</span><span class="sxs-lookup"><span data-stu-id="8eb5e-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="8eb5e-107">Możesz również wyszukać to polecenie za pomocą następującego polecenia programu PowerShell dla usługi Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="8eb5e-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="8eb5e-108">Jeśli nie chcesz usuwać istniejącego adresu e-mail, wybierz nowy adres e-mail dla nowego obiektu, który tworzysz.</span><span class="sxs-lookup"><span data-stu-id="8eb5e-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  