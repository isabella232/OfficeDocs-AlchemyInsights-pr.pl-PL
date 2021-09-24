---
title: Dodawanie poddomeny
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506775"
---
# <a name="adding-a-sub-domain"></a>Dodawanie poddomeny

Domeny podrzędne można dodawać do tej samej lub innej dzierżawy niż domena nadrzędna. W obu przypadkach musisz zarządzać własnymi ustawieniami DNS w witrynie internetowej rejestratora. Jeśli chcesz, aby firma Microsoft zarządzała ustawieniami DNS za pomocą rekordów serwera nazw lub domena kupiona od firmy Microsoft, nie możesz dodać poddomen bez uprzedniej zmiany tej nazwy.

Najpierw dodaj domenę nadrzędną, a następnie dodaj poddomeną. Jeśli poddomena znajduje się w tej samej dzierżawie, nie jest konieczna dodatkowa weryfikacja. Jeśli dodanie poddomeny do oddzielnej dzierżawy wymaga rekordu DNS txt na potrzeby weryfikacji własności przed dodaniem domeny i dodatkowych rekordów DNS dla wybranych usług.

- Aby dodać domenę lub poddomenę, wykonaj czynności kreatora Dodawanie domeny lub ręcznie dodaj domenę lub poddomenę, przechodząc do **tematu Ustawianie** domen Dodaj [](https://admin.microsoft.com/Adminportal#/Domains/Wizard)  >    >  **domenę.**

W razie potrzeby:

- Aby zmienić ustawienia systemu DNS dla istniejącej domeny, przejdź do Ustawienia Domains (Domeny), zaznacz pole wyboru obok domeny, a następnie wybierz pozycję Manage DNS (Zarządzaj  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains) **systemem DNS).** W kreatorze wybierz pozycję **Dodaj własne rekordy DNS i** wykonaj zadania kreatora.
- Aby dodać poddomeny do kupionej domeny firmy Microsoft, najpierw przenieś domenę do innego rejestratora, a następnie zmień ją powyżej w celu zarządzania własnymi rekordami DNS. Aby uzyskać instrukcje, [zobacz Przenoszenie domeny z firmy Microsoft do innego hosta.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
- Jeśli zostanie wyświetlony komunikat o błędzie, że Twoja domena jest już używania przez innych członków lub osoby w Twojej organizacji, przed rozpoczęciem korzystania z tej domeny musisz przejąć to konto niezamówione. Aby uzyskać instrukcje, zobacz Przejmij kontrolę nad katalogiem niezawiązyanego [jako administrator w programie Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover)
