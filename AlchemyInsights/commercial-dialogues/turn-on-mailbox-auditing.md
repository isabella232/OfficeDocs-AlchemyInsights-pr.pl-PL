---
title: Włączanie inspekcji skrzynki pocztowej
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482474"
---
# <a name="turn-on-mailbox-auditing"></a>Włączanie inspekcji skrzynki pocztowej

Aby włączyć inspekcję skrzynki pocztowej dla jednego użytkownika lub całej organizacji, uruchom następujące polecenia cmdlet w zdalnym programie PowerShell:

- **Jeden użytkownik:** Set-Mailbox -Identity "Annie Dow" -AuditEnabled $true
- **Organizacja:** Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true

Aby dowiedzieć się więcej, zobacz [Zarządzanie inspekcją skrzynki pocztowej.](https://go.microsoft.com/fwlink/?linkid=2103668)