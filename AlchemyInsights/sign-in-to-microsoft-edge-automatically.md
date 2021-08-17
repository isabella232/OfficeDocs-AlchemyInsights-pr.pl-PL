---
title: Automatyczne logowanie Microsoft Edge konta
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050704"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatyczne logowanie Microsoft Edge konta

Microsoft Edge konta domyślnego systemu operacyjnego są używane do automatycznego logowania użytkownika zgodnie z konfiguracją urządzenia użytkownika. 

Poniżej opisano scenariusze dotyczące poszczególnych typów konfiguracji urządzenia i zależnego od niego procesu logowania użytkownika:

- **Urządzenie jest hybrydowe/AAD-J:** Ta opcja jest dostępna w Windows 10 wersji Windows i odpowiednich wersjach serwera. Użytkownicy są automatycznie zalogowani przy użyciu kont Azure Active Directory (AD).
- **Urządzenie jest przyłączone do** domeny: ta opcja jest dostępna Windows 10 serwerach, Windows i odpowiadających im wersjach serwera. Domyślnie użytkownicy z kontami domeny nie są zalogowani automatycznie. aby włączyć dla nich automatyczne logowanie się, użyj zasad **ConfigureOnPremisesAccountAutoSignIn.** Aby włączyć automatyczne logowanie dla użytkowników z kontami usługi Azure AD, rozważ dołączanie hybrydowe ich urządzeń.
- Konto domyślne systemu operacyjnego to konto **Microsoft:** Ta opcja jest dostępna w systemie Windows 10 RS3 (wersja 1709, kompilacja 10.0.16299) i nowszych wersjach. Scenariusz jest mało prawdopodobny na urządzeniach w przedsiębiorstwie. Jeśli jednak kontem domyślnym systemu operacyjnego jest konto Microsoft, Microsoft Edge automatycznie zaloguje się do użytkownika za pomocą konta Microsoft.
 
 
