---
title: Raporty w centrum administracyjne platformy Microsoft 365 nie mają czytelnej nazwy użytkownika
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
ms.openlocfilehash: 16aa4f052c934421423c73244f03a20aa38e4785
ms.sourcegitcommit: 76c61dec041b93d0039764fae38107108da324aa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2021
ms.locfileid: "59316194"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Raporty w centrum administracyjne platformy Microsoft 365 nie mają czytelnej nazwy użytkownika

W raportach centrum administracyjne platformy Microsoft 365 nie są wyświetlane nazwy użytkowników, ale są wyświetlane wartości alfanumerczne, takie jak B2BC6C15BB9FCDEA71E5CD302D228CC8.

Jest to oczekiwane zachowanie i zostało przekazane w Centrum wiadomości (MC275344, opublikowane 3 sierpnia 2021 r.). 

Administratorzy globalni mogą przywrócić tę zmianę w swojej dzierżawie i pokazać identyfikowalne dane użytkowników, jeśli pozwalają na to ich organizacje. Aby przywrócić zmianę dla dzierżawy:

1. W centrum administracyjnym przejdź do pozycji **Ustawienia**  >  **ustawienia organizacji**  >  [**Usługi**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services)i wybierz pozycję **Raporty.** 
1. W **obszarze Wybierz sposób pokazywania informacji o użytkownikach** wybierz pozycję Pokaż identyfikowalne informacje o użytkownikach w raportach , a następnie ponownie uruchom raport. 