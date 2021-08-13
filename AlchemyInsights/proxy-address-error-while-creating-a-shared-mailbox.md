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
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062918"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Błąd adresu serwera proxy podczas tworzenia skrzynki pocztowej lub innego obiektu z włączoną obsługą poczty e-mail

Jeśli podczas próby utworzenia obiektu z obsługą poczty e-mail (skrzynka pocztowa, udostępniona skrzynka pocztowa itp.) został odebrany błąd "Adres serwera proxy "SMTP:alias@domain.com" jest już używany...", wybrany adres e-mail jest już używany przez inny obiekt w organizacji z obsługą poczty e-mail.
  
Znajdź użytkownika, grupę, udostępnioną skrzynkę pocztową lub folder publiczny z tym adresem e-mail i usuń go lub zmień jego adres e-mail. Następnie możesz utworzyć nowy obiekt z obsługą poczty e-mail z darmowym adresem e-mail. Aby go znaleźć, użyj funkcji wyszukiwania na stronie głównej. Aby wyszukać ten program, możesz Exchange Online użyć następującego polecenia programu PowerShell:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Jeśli nie chcesz usuwać istniejącego adresu e-mail, wybierz nowy adres e-mail dla nowego obiektu, który tworzysz.
  