---
title: Kod błędu 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jeśli podczas włączania wdrożeń usługi RDS (Remote Desktop Services) pojawia się błąd, należy rozważyć włączenie usługi ADAL przez edycję rejestru.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506856"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Błąd podczas aktywacji pakietu Office 2013 w usługach pulpitu zdalnego

Jeśli podczas włączania wdrożeń usługi RDS (Remote Desktop Services) pojawia się błąd, należy rozważyć włączenie usługi ADAL przez edycję rejestru.
  
|**Klucz rejestru**|**Type**|**Wartość**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Oprogramowanie\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Aby uzyskać więcej informacji, zobacz [Włączanie nowoczesnego uwierzytelniania dla pakietu Office 2013 na urządzeniach z systemem Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  Usługa ADAL jest domyślnie włączona w usłudze Microsoft 365 Apps dla przedsiębiorstw i pakiecie Office 2016. Usługi pulpitu zdalnego (RDS) były wcześniej nazywane usługami terminalowymi.
  