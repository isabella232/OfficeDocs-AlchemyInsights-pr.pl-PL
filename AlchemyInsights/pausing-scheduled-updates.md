---
title: Wstrzymywanie zaplanowanych aktualizacji
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555514"
---
# <a name="pausing-scheduled-updates"></a>Wstrzymywanie zaplanowanych aktualizacji

Po wydaniu polecenia pauzy urządzenia nie przetwarzają polecenia, dopóki następnym razem zaewidencjonują je w usłudze Intune. Z tego powodu urządzenia mogą mieć:

- Zainstalowano zaplanowane aktualizacje przed zameldowanie.
- Został wyłączony po wydaniu polecenia pauzy. W takim przypadku, gdy urządzenia były włączone, mogły pobrać i zainstalować zaplanowane aktualizacje przed zaewidencjonowania.