---
title: Włącz inspekcję skrzynki pocztowej
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29500292"
---
# <a name="enable-mailbox-auditing"></a>Włącz inspekcję skrzynki pocztowej

Aby włączyć inspekcję, skrzynki pocztowej dla pojedynczego użytkownika lub całej organizacji następujące polecenia cmdlet należy uruchomić z powłoki zdalnej zasilania:
  
 **Pojedynczy użytkownik**
  
Set-Mailbox - tożsamości "Jane Dow" - AuditEnabled $true
  
 Organization
  
Get-Mailbox - ResultSize nieograniczony - filtr {RecipientTypeDetails - eq "UserMailbox"} | Set-Mailbox - AuditEnabled $true
  
Więcej informacji
  

