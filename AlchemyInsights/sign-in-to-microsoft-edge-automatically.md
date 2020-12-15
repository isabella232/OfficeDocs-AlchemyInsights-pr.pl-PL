---
title: Automatyczne logowanie w przeglądarce Microsoft Edge
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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678811"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatyczne logowanie w przeglądarce Microsoft Edge

Program Microsoft Edge używa domyślnego konta systemu operacyjnego do automatycznego logowania użytkownika zgodnie z konfiguracją urządzenia użytkownika. 

Poniżej opisano scenariusze poszczególnych typów konfiguracji urządzeń oraz proces logowania się do niego zależne.

1. To **urządzenie jest hybrydowe/AAD-J**: Ta opcja jest dostępna w systemie Windows 10, w systemie Windows, na poziomie niższego poziomu i w odpowiednich wersjach serwera. Użytkownicy są automatycznie logowani przy użyciu kont usługi Azure Active Directory (AD).
2. **Urządzenie jest przyłączone do domeny**: Ta opcja jest dostępna w systemie Windows 10, na poziomie systemu Windows i w odpowiednich wersjach serwera. Domyślnie użytkownicy z kontami domeny nie są zalogowani automatycznie; Aby włączyć automatyczne logowanie, użyj zasad **ConfigureOnPremisesAccountAutoSignIn** . Aby włączyć automatyczne logowanie użytkowników z kontami usługi Azure AD, weź pod ³ ¹ łączenie hybrydowe urządzeń.
3. **Domyślne konto systemu operacyjnego to konto Microsoft**: Ta opcja jest dostępna w systemie Windows 10 RS3 (wersja 1709, Kompilacja 10.0.16299) i w nowszych wersjach. W przypadku urządzeń z jednostkami biznesowymi nie ma mało prawdopodobnego scenariusza. Jeśli jednak domyślnym kontem systemu operacyjnego jest konto Microsoft, program Microsoft Edge automatycznie zaloguje użytkownika przy użyciu konta Microsoft.
 
 
