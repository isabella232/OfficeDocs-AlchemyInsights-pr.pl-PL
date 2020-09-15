---
title: 618 zasady udostępniania kalendarza
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
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684240"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Błąd zasad podczas udostępniania kalendarza

1. Wykonaj dowolną z następujących czynności, stosownie do sytuacji:
    - Nawiązywanie połączenia z usługą Exchange Online przy użyciu zdalnego programu PowerShell. Aby uzyskać więcej informacji, zobacz [łączenie się z usługą Exchange Online przy użyciu zdalnego programu PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Na serwerze lokalnym Otwórz powłokę zarządzania programu Exchange.
2. Określ zasady udostępniania przypisane do użytkownika. Aby to zrobić, uruchom następujące polecenie i zanotuj zwrócone zasady:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Zaktualizuj zasady udostępniania dla użytkownika. Aby to zrobić, wykonaj następujące kroki.
    - Otwórz Centrum administracyjne programu Exchange.
    - Kliknij pozycję **organizacja**, a następnie kliknij dwukrotnie zasadę przypisaną do użytkownika w obszarze **udostępnianie indywidualne**. Są to zasady zwrócone w kroku 2.
    - Na stronie reguła udostępniania wybierz poziom udostępniania kalendarza, dla którego chcesz zezwolić na **Określanie informacji, które chcesz udostępnić**. Kliknij przycisk **Zapisz**.

Aby uzyskać więcej informacji, zobacz: ["zasady nie zezwalają na udzielanie uprawnień na tym poziomie do jednego lub większej liczby adresatów", gdy użytkownik próbuje udostępnić kalendarz](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
