---
title: Kod błędu 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jeśli podczas aktywowania programu Office 2013 we wdrożeniach usług pulpitu zdalnego (RDS) jest wyświetlany komunikat o błędzie, rozważ włączenie usługi ADAL przez edytowanie rejestru.
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316696"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Błąd podczas aktywacji programu Office 2013 w usługach pulpitu zdalnego

Jeśli podczas aktywowania programu Office 2013 we wdrożeniach usług pulpitu zdalnego (RDS) jest wyświetlany komunikat o błędzie, rozważ włączenie usługi ADAL przez edytowanie rejestru.
  
|**Klucz rejestru**|**Type**|**Wartość**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Aby uzyskać więcej informacji, [zobacz Włączanie nowoczesnego uwierzytelniania Office 2013 na Windows urządzeniach.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
**Uwaga:** W programach Aplikacje Microsoft 365 dla przedsiębiorstw i Office 2016 ADAL jest domyślnie włączone. Usługi pulpitu zdalnego (RDS) wcześniej nazywały się Usługi terminalowe.
  