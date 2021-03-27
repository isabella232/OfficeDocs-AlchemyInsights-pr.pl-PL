---
title: Automatyczne logowanie się do programu Microsoft Edge
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
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398739"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatyczne logowanie się do programu Microsoft Edge

Program Microsoft Edge używa domyślnego konta systemu operacyjnego do automatycznego logowania użytkownika zgodnie z konfiguracją urządzenia użytkownika. 

Poniżej opisano scenariusze dotyczące poszczególnych typów konfiguracji urządzenia i zależnego od niego procesu logowania użytkownika:

- **To urządzenie jest hybrydowe/AAD-J:** Ta opcja jest dostępna w systemie Windows 10 oraz w odpowiednich wersjach serwera. Użytkownicy są automatycznie zalogowani przy użyciu kont usługi Azure Active Directory (AD).
- **Urządzenie jest przyłączone do** domeny: Ta opcja jest dostępna w systemie Windows 10, na poziomie poprzednich wersji systemu Windows i w odpowiadających im wersjach serwera. Domyślnie użytkownicy z kontami domeny nie są zalogowani automatycznie. aby włączyć dla nich automatyczne logowanie się, użyj zasad **ConfigureOnPremisesAccountAutoSignIn.** Aby włączyć automatyczne logowanie dla użytkowników z kontami usługi Azure AD, rozważ dołączanie hybrydowe ich urządzeń.
- Konto domyślne systemu operacyjnego to konto **Microsoft:** Ta opcja jest dostępna w systemie Windows 10 RS3 (wersja 1709, kompilacja 10.0.16299) i w nowszych wersjach. Scenariusz jest mało prawdopodobny na urządzeniach w przedsiębiorstwie. Jeśli jednak kontem domyślnym systemu operacyjnego jest konto Microsoft, program Microsoft Edge automatycznie zaloguje się użytkownika za pomocą konta Microsoft.
 
 
