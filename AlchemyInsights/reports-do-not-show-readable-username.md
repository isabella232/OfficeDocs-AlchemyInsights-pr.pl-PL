---
title: Raporty w centrum administracyjnym platformy Microsoft 365 nie pokazują czytelnej nazwy użytkownika
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327824"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Raporty w centrum administracyjnym platformy Microsoft 365 nie pokazują czytelnej nazwy użytkownika

Raporty w centrum administracyjnym platformy Microsoft 365 nie pokazują nazw użytkowników, ale zamiast tego pokazują wartości alfanumeryczne, takie jak B2BC6C15BB9FCDEA71E5CD302D228CC8.

Jest to spodziewane zachowanie i zostało przekazane w Centrum wiadomości (MC275344, opublikowano 3 sierpnia 2021 r.). 

Administratorzy globalni mogą cofnąć tę zmianę dla swojej dzierżawy i wyświetlać identyfikowalne informacje o użytkownikach, jeśli zezwalają na to ich praktyki ochrony prywatności w organizacji. Aby przywrócić zmianę dla dzierżawy:

1. W centrum administracyjnym przejdź do pozycji **Ustawienia** > **Ustawienia organizacji** > [**Usługi**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services ) i wybierz pozycję **Raporty**. 
1. W obszarze **Wybierz sposób wyświetlania informacji o użytkowniku** wybierz pozycję **Pokaż identyfikowalne informacje o użytkowniku w raportach**, a następnie uruchom ponownie raport.