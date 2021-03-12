---
title: Nagrywanie rozmów 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733859"
---
# <a name="11-call-recording"></a>Nagrywanie rozmów 1:1

Administratorzy muszą teraz podjąć działania, aby nadal zezwalać użytkownikom na nagrywanie rozmów 1:1.
 
Począwszy od 12 kwietnia 2021 r., zaczniemy wymuszać nową opcję zasad połączeń usługi Teams *AllowCloudRecordingForCalls.* 

Obecnie możliwości nagrywania rozmów 1:1 są kontrolowane przez opcję *AllowCloudRecording* w zasadach spotkania usługi Teams. Jeśli użytkownicy mogą nagrywać spotkania w aplikacji Teams, mogą również nagrywać połączenia 1:1.

Jeśli wolisz zablokować wszystkim użytkownikom nagrywanie rozmów 1:1, nie musisz nic robić. *Opcja zasad połączeń AllowCloudRecordingForCalls* zostanie domyślnie $False domyślne.

Tę zmianę oprowadzono w następującym wpisie w Centrum wiadomości: (Zaktualizowano) Wprowadzenie do zasad nagrywania połączeń [(1:1)](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Aby ustawić opcję zasad połączeń aplikacji Teams, należy użyć [programu Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)

Aby włączyć rejestrowanie połączeń w połączeniach **1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True

Aby wyłączyć rejestrowanie połączeń w połączeniach **1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False

