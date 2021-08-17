---
title: 618 Zasady udostępniania kalendarza
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091613"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Błąd zasad podczas udostępniania kalendarza

1. Wykonaj jedną z następujących czynności, odpowiednio do sytuacji:
    - Połączenie można Exchange Online przy użyciu zdalnej pracy z programem PowerShell. Aby uzyskać więcej informacji, [zobacz Połączenie do Exchange Online przy użyciu zdalnej pracy programu PowerShell.](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)
    - Na serwerze lokalnym otwórz powłokę Exchange zarządzania.
2. Określ zasady udostępniania przypisane do użytkownika. W tym celu uruchom następujące polecenie i zwróć uwagę na zwrócone zasady:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Zaktualizuj zasady udostępniania dla użytkownika. Aby to zrobić, wykonaj następujące kroki.
    - Otwórz Exchange administracyjnego.
    - Kliknij **pozycję** Organizacja, a następnie kliknij dwukrotnie zasady przypisane do użytkownika w obszarze **Udostępnianie indywidualne**. Jest to zasady zwrócone w kroku 2.
    - Na stronie Reguła udostępniania wybierz poziom udostępniania kalendarza, na który chcesz zezwolić, w obszarze Określ informacje, **które chcesz udostępnić**. kliknij **przycisk Zapisz**.

Aby uzyskać więcej informacji, zobacz: "Zasady nie zezwalają na udzielanie uprawnień na tym poziomie co najmniej jednem adresatom", gdy użytkownik próbuje [udostępnić kalendarz.](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)
