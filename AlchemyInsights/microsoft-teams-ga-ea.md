---
title: Microsoft Teams — dostęp gościa
ms.author: heidip
author: microsoftheidi
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "311"
- "6500001"
ms.openlocfilehash: da9ecca062bd5f1dcc169657483ba53eb201def0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798386"
---
# <a name="microsoft-teams---guest-access"></a>Microsoft Teams — dostęp gościa

Jeśli potrzebujesz pomocy dotyczącej komunikacji z użytkownikami spoza organizacji w usłudze Teams, musisz zdecydować, czy chcesz używać [dostępu gościa, dostępu zewnętrznego (Federacji)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access), czy można używać obu tych sposobów.

Pamiętaj o [przejrzeniu różnic](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) , aby zapoznać się z funkcjami dostępnymi dla każdego z nich.  Na przykład dostęp zewnętrzny (Federacja) umożliwia prowadzenie komunikacji z programem 1:1, takich jak czat i obecność.  Użytkownicy federacyjną nie mogą jednak uczestniczyć w współpracy z zespołami.  Jeśli chcesz, aby użytkownik zewnętrzny dołączył do konwersacji w aplikacji Teams i uczestniczył w nich lub udostępniać pliki, musisz włączyć dostęp gościa.

**Opcja 1: Włączanie dostępu gościa**   
W centrum administracyjnym zespołów przejdź do obszaru [Ustawienia organizacji > dostęp gościa](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) i Włącz opcję "Zezwalaj na dostęp Gości w zespołach".  W przypadku dzierżawy ze wszystkimi innymi ustawieniami domyślnymi powinno to wystarczyć.  Aby dostosować konfigurację dostępu gościa, upewnij się, że wykonano czynności opisane w [temacie Lista kontrolna dostępu gościa](https://docs.microsoft.com/microsoftteams/guest-access-checklist). Gdy wszystko będzie gotowe, musisz [poczekać na 24 godziny, aż](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) zaczną obowiązywać ustawienia.

Jeśli masz pewność, że wykonano wszystkie czynności z listy kontrolnej i że jest ona dłuższa niż 24 godziny, możesz spróbować [dodać gościa do zespołu](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop).

Aby uzyskać więcej informacji, w tym klipy wideo, zobacz [dostęp gościa w aplikacji Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access).

**Opcja 2: Włączanie dostępu zewnętrznego (Federacja)** Jeśli chcesz również włączyć dostęp zewnętrzny (Federacja), w centrum administracyjnym aplikacji Teams Center przejdź do obszaru [Ustawienia w całej organizacji > dostęp zewnętrzny](https://admin.teams.microsoft.com/company-wide-settings/external-communications) i Włącz opcję "użytkownicy mogą komunikować się z użytkownikami programu Skype dla firm i zespołów", a następnie postępuj zgodnie z instrukcjami, aby [umożliwić użytkownikom zespołu czatowanie i komunikację z użytkownikami w innej organizacji](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization).


