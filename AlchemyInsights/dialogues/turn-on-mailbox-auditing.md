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
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429738"
---
# <a name="turn-on-mailbox-auditing"></a>Włączanie inspekcji skrzynki pocztowej

Aby włączyć inspekcję skrzynki pocztowej dla jednego użytkownika lub całej organizacji, uruchom następujące polecenia cmdlet w zdalnym programie PowerShell:

- **Jeden użytkownik:** Set-Mailbox -Identity "Annie Dow" -AuditEnabled $true
- **Organizacja:** Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true

Aby dowiedzieć się więcej, zobacz [Zarządzanie inspekcją skrzynki pocztowej.](https://go.microsoft.com/fwlink/?linkid=2103668)