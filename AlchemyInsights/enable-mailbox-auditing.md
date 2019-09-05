---
title: Włącz inspekcję skrzynek pocztowych
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736263"
---
# <a name="enable-mailbox-auditing"></a>Włącz inspekcję skrzynek pocztowych

Aby włączyć inspekcję skrzynek pocztowych dla jednego użytkownika lub całej organizacji, należy uruchomić następujące polecenia cmdlet z zdalnej powłoki zasilania:
  
 **Pojedynczy użytkownik**
  
Zestaw-Mailbox-tożsamość "Jane Dow"-AuditEnabled $true
  
 **Organizacji**
  
Pobierz skrzynki pocztowej-ResultSize nieograniczony-filtr {RecipientTypeDetails-EQ "UserMailbox"} | $true AuditEnabled zestawu skrzynek pocztowych
  
[Dowiedz się więcej](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

