---
title: Send As Mail Enabled Public Folder in EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 22aa3e8f46c2ff4f62cb520b9498041dffb9d3a3eb607d788cc97b10bf32dbb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052576"
---
# <a name="sendas-mail-enabled-public-folder"></a>Folder publiczny z włączoną obsługą poczty SendAs

W poniższym przykładzie użytkownikowi Jasonowi przypisano uprawnienia "Wyślij jako" dla folderu publicznego z obsługą poczty NewPF1.

Add-RecipientPermission -Identity "NewPF1" -Trustee "Jason" -AccessRights 'SendAs'

Aby uzyskać szczegółowe informacje o składni i parametrach, zobacz [Przypisywanie uprawnień "Wyślij jako"](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)lub "Wyślij w imieniu" dla folderów publicznych z obsługą poczty.

