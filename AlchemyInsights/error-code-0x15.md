---
title: Kod błędu 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jeśli otrzymujesz komunikat o błędzie podczas aktywowania pakietu Office 2013 we wdrożeniach usług pulpitu zdalnego (RDS), należy rozważyć włączenie ADAL przez edycję rejestru.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29929098"
---
Jeśli otrzymujesz komunikat o błędzie podczas aktywowania pakietu Office 2013 we wdrożeniach usług pulpitu zdalnego (RDS), należy rozważyć włączenie ADAL przez edycję rejestru. 
  
|**Klucz rejestru**|**Type**|**Value (Wartość)**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Aby uzyskać więcej informacji zobacz [Włączanie uwierzytelniania nowoczesnych 2013 pakietu Office na urządzeniach z systemem Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL jest włączona domyślnie w Office 365 ProPlus i 2016 pakietu Office. > usług pulpitu zdalnego (RDS) wcześniej nosił nazwę usług terminalowych. 
  

