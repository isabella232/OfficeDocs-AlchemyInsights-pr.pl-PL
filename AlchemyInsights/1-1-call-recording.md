---
title: Nagrywanie rozmowy 1:1
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
ms.openlocfilehash: c17408442cec6c0877b7d66bc8a7fd3062eb0e47
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314394"
---
# <a name="11-call-recording"></a>Nagrywanie rozmowy 1:1

Jeśli przycisk **Rozpocznij nagrywanie** jest wyszarzony w czasie połączenia 1:1, musisz zmienić ustawienia zasad dla użytkownika, na który ma to wpływ. Aby sprawdzić ustawienie zasad, uruchom narzędzie Diagnostyczne dla użytkownika, u którym ma to wpływ, wpisując **Diag: Teams 1:1 Call Recording above (Rejestrowanie połączenia 1:1).**     

Począwszy od 31 maja 2021 r., zaczniemy wymuszanie nowej zasady połączeń telefonicznych usługi Teams *AllowCloudRecordingForCalls.* Przed tą zmianą nagrywanie połączeń 1:1 jest kontrolowane przez zasady spotkań Teams *AllowCloudRecording.* Ta zmiana została udokumentowana we wpisie w Centrum wiadomości: [(Zaktualizowano) 1:1 Wprowadzenie](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)do zasad nagrywania połączeń.  

*AllowCloudRecordingForCalls*   opcję zasad połączeń jest domyślnie **$False** domyślne. Jeśli wolisz zablokować wszystkim użytkownikom nagrywanie połączeń 1:1, nie musisz nic robić.  

Aby włączyć nagrywanie połączeń dla wszystkich użytkowników w połączeniach 1:1, użyj Teams [PowerShell,](https://docs.microsoft.com/microsoftteams/teams-powershell-install) aby uruchomić następujące polecenie cmdlet: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Ewentualnie możesz utworzyć nowe zasady i ustawić ustawienie **-AllowCloudRecordingForCalls** w celu $true i przypisania tych zasad do użytkowników.  

Aby uzyskać więcej informacji, zobacz 1:1 Kontrolki zasad nagrywania połączeń [są (prawie!) Tutaj](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
