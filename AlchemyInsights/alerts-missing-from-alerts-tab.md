---
title: Na karcie Alerty brakuje alertów
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12732"
ms.openlocfilehash: 9fbd9a32e40d858f0ba49931c723a824478aaa12
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454971"
---
# <a name="alerts-missing-from-alerts-tab"></a>Na karcie Alerty brakuje alertów

Karta **Alerty** działa w oparciu o zasady konfigurowane i aktywowane z portalu zarządzania aplikacją w dzierżawie. Aby sygnały przepływały na kartę **Alerty,** należy również uaktywnić zasady, które są włączone w zarządzaniu aplikacją. 

Potwierdź wygenerowanie alertu:

1. Przejdź do zasad zarządzania [aplikacją i](https://compliance.microsoft.com/m365appprotection?viewid=policies) upewnij się, że utworzono co najmniej jedną aktywną lub aktywna zasady inspekcji.

1. Wybierz zasady, a następnie wybierz pozycję Edytuj **w** okienku wysuwanych. 

1. Sprawdź konfigurację zasad, aby upewnić się, że alert powinien zostać wygenerowany na podstawie zdarzenia zasad zainicjowanego ponad 24 godziny temu.

Aby uzyskać więcej informacji na temat alertów w zarządzaniu aplikacją, zobacz Wprowadzenie do wykrywania zagrożeń aplikacji [i rozwiązywania problemów.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-detect-remediate-get-started)