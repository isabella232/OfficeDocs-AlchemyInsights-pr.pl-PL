---
title: 126 Nie można odnaleźć skrzynki pocztowej w programie OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: aca0371dad9ba43fa21b0df8e50f1b8ee536528af90d6bda401995c6e5796be4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54056500"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Błąd nie można odnaleźć skrzynki pocztowej w Outlook w sieci Web?

Jeśli korzystasz z programu Outlook w sieci Web i  nie można odnaleźć skrzynki pocztowej z powodu błędu, oznacza to, że konta użytego do nawiązania połączenia z programem Outlook w sieci Web nie ma licencji usługi Exchange Online, więc z kontem nie jest skojarzona żadna skrzynka pocztowa. Administrator może przypisać licencję do Twojego konta, korzystając z następujących kroków:

1. Otwórz [centrum administracyjne platformy Microsoft 365](https://portal.office.com/adminportal/home#/homepage) i przejdź **do** sekcji Aktywni użytkownicy w sekcji Użytkownicy, a następnie wybierz użytkownika, dla którym jest wyświetlany komunikat o błędzie. 

2. Na otwartej stronie użytkownika przejdź  do sekcji Licencje i  aplikacje, wybierz odpowiednią wartość Lokalizacja i przypisz licencję zawierającą usługę Exchange Online (rozwiń tę licencję, aby wyświetlić jej szczegóły). Po zakończeniu kliknij pozycję **Zapisz zmiany**.

W niektórych przypadkach, jeśli licencja jest już przypisana do konta użytkownika, usunięcie i ponowne przypisanie licencji pomaga rozwiązać ten problem i uzyskać jego poprawnie aprowizowane w systemie: 

- Sprawdź, czy Twoja subskrypcja usługi M365 Exchange Online (i inne, jeśli masz subskrypcje) jest aktualna i nie wygasła niedawno.

Gdy już upewnisz się, że Twoja subskrypcja nie wygasła, a do konta użytkownika przypisano ważną licencję, może upłynąć do 24 godzin, aby uzyskać inicjowanie obsługi administracyjnej, dlatego może być konieczne zaczekanie na rozwiązanie problemu. Aby uzyskać więcej informacji, zobacz [Przypisywanie licencji i zarządzanie nimi.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)