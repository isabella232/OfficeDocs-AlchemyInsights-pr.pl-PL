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
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906742"
---
<span data-ttu-id="76766-p101">Skrzynki pocztowej użytkownika można konwertować na udostępnionej skrzynki pocztowej tylko, jeśli użytkownik ma licencję Exchange. Po przekonwertowaniu skrzynki pocztowej, nadal będzie wyświetlane na liście aktywnych użytkowników, ponieważ ten wykaz zawiera udostępnionych skrzynek pocztowych. Jednak przekonwertowane skrzynki pocztowej także pojawi się na liście udostępnionej skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="76766-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="76766-p102">Jeśli podczas próby konwersji skrzynek pocztowych w konsoli administracyjnej programu Exchange i konwersja kończy się niepowodzeniem, wyczyść pamięć podręczną przeglądarki i pliki cookie i spróbuj ponownie. Jeśli nadal nie działa, spróbuj wykonać konwersji skrzynki pocztowej w programu Exchange Management Shell, uruchamiając następujące polecenie:</span><span class="sxs-lookup"><span data-stu-id="76766-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="76766-107">Więcej informacji o konwersji skrzynki pocztowej jest dostępna w [konwersji skrzynki pocztowej użytkownika na udostępnionej skrzynki pocztowej](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="76766-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
