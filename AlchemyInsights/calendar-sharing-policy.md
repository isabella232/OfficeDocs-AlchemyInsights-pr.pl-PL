---
title: 618 Zasady udostępniania kalendarza
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373009"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Błąd zasad podczas udostępniania kalendarza

1. Wykonaj jedną z następujących czynności, odpowiednio do sytuacji:
    - Połącz się z usługą Exchange Online przy użyciu programu Remote PowerShell. Aby uzyskać więcej informacji, zobacz [Łączenie się z usługą Exchange Online przy użyciu programu Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Na serwerze lokalnym otwórz powłokę zarządzania programem Exchange.
2. Określ zasady udostępniania przypisane do użytkownika. Aby to zrobić, uruchom następujące polecenie i zanotuj zwrócone zasady:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Zaktualizuj zasady udostępniania dla użytkownika. W tym celu wykonaj następujące czynności:
    - Otwórz centrum administracyjne programu Exchange.
    - Kliknij pozycję **Organizacja**, a następnie kliknij dwukrotnie zasadę przypisaną do użytkownika w obszarze **Udostępnianie indywidualne**. Jest to zasada, która została zwrócona w kroku 2.
    - Na stronie Reguła udostępniania wybierz poziom udostępniania kalendarza, na który chcesz zezwolić w obszarze **Określanie informacji, które chcesz udostępnić;** kliknij przycisk **Zapisz**.

Aby uzyskać więcej informacji, zobacz: ["Zasady nie zezwalają na udzielanie uprawnień na tym poziomie jednemu lub większej liczbie adresatów" błędu podczas próby udostępnienia kalendarza](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)przez użytkownika .
