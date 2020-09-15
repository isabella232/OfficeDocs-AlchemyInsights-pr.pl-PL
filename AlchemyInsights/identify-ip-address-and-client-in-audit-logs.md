---
title: Identyfikowanie adresu IP i klienta w dziennikach inspekcji
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668320"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identyfikowanie adresu IP i klienta w dziennikach inspekcji

W dziennikach inspekcji jest wyświetlany adres IP, który odpowiada działaniu użytkownika lub administratora usługi Microsoft 365. Informacje dotyczące klienta są również rejestrowane. Poniżej przedstawiono procedurę identyfikowania takich informacji

1. Zaloguj się do [Centrum zabezpieczeń & programu Microsoft 365](https://protection.office.com/).

2. Przejdź do strony **Search**  >  **wyszukiwania dziennika inspekcji** wyszukiwania.

   Jeśli chcesz skorzystać z określonej czynności, wybierz ją z listy **działań** . Jeśli nie, wszystkie działania zostaną zwrócone dla wybranego użytkownika (ustawienie domyślne).

   **Uwaga**: niektóre działania mogą nie być dostępne w menu **działania** ; Jednak te elementy inspekcji zostaną zwrócone, jeśli wybrano opcję **Pokaż wyniki dla wszystkich działań** (ustawienie domyślne).

3. Określ nazwę użytkownika w polu **Użytkownicy** , wybierz odpowiedni zakres dat dla działania, a następnie kliknij przycisk **Wyszukaj**.

W wynikach wyszukiwania w okienku wyniki jest widoczny adres IP dla tego działania. Wybierz rekord inspekcji, aby wyświetlić szczegółowe informacje w menu wysuwanym **szczegóły** (na przykład klient, użytkownik, który wykonał akcję itd.).

Aby uzyskać więcej informacji, zobacz [Znajdowanie adresu IP komputera, za pomocą którego można uzyskać dostęp do złamanego konta](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
