---
title: Konwertowanie skrzynki pocztowej użytkownika na udostępnionej skrzynki pocztowej?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496445"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="792d1-102">Konwertowanie skrzynki pocztowej użytkownika na udostępnionej skrzynki pocztowej</span><span class="sxs-lookup"><span data-stu-id="792d1-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="792d1-103">Skrzynki pocztowej użytkownika można konwertować na udostępnionej skrzynki pocztowej tylko, jeśli użytkownik ma licencję Exchange.</span><span class="sxs-lookup"><span data-stu-id="792d1-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="792d1-104">Po przekonwertowaniu skrzynki pocztowej, nadal będzie wyświetlane na liście aktywnych użytkowników, ponieważ ten wykaz zawiera udostępnionych skrzynek pocztowych.</span><span class="sxs-lookup"><span data-stu-id="792d1-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="792d1-105">Jednak przekonwertowane skrzynki pocztowej także pojawi się na liście udostępnionej skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="792d1-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="792d1-106">Jeśli podczas próby konwersji skrzynek pocztowych w konsoli administracyjnej programu Exchange i konwersja kończy się niepowodzeniem, wyczyść pamięć podręczną przeglądarki i pliki cookie i spróbuj ponownie.</span><span class="sxs-lookup"><span data-stu-id="792d1-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="792d1-107">Jeśli nadal nie działa, spróbuj wykonać konwersji skrzynki pocztowej w programu Exchange Management Shell, uruchamiając następujące polecenie:</span><span class="sxs-lookup"><span data-stu-id="792d1-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="792d1-108">Więcej informacji o konwersji skrzynki pocztowej jest dostępna w [konwersji skrzynki pocztowej użytkownika na udostępnionej skrzynki pocztowej](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span><span class="sxs-lookup"><span data-stu-id="792d1-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
