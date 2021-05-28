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
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696968"
---
# <a name="11-call-recording"></a>Nagrywanie rozmowy 1:1

Jeśli przycisk **Rozpocznij nagrywanie** jest wyszarzony w czasie połączenia 1:1, musisz zmienić ustawienia zasad dla użytkownika, na który ma to wpływ.   

Począwszy od 31 maja 2021 r., zaczniemy wymuszanie nowej zasady połączeń usługi Teams *AllowCloudRecordingForCalls.* Przed tą zmianą nagrywanie połączeń 1:1 jest kontrolowane przez zasady spotkań Teams *AllowCloudRecording.* Ta zmiana została udokumentowana we wpisie w Centrum wiadomości: [(Zaktualizowano) 1:1 Wprowadzenie](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)do zasad nagrywania połączeń.  

*AllowCloudRecordingForCalls*   opcję zasad połączeń jest domyślnie **$False** domyślne. Jeśli wolisz zablokować wszystkim użytkownikom nagrywanie połączeń 1:1, nie musisz nic robić.  

Aby włączyć nagrywanie połączeń dla wszystkich użytkowników w połączeniach 1:1, użyj Teams PowerShell, aby uruchomić następujące polecenie cmdlet: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Ewentualnie możesz utworzyć nowe zasady i ustawić ustawienie **-AllowCloudRecordingForCalls** w celu $true i przypisania tych zasad do użytkowników.  

Aby uzyskać więcej informacji, zobacz 1:1 Kontrolki zasad nagrywania połączeń [są (prawie!) Tutaj](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
