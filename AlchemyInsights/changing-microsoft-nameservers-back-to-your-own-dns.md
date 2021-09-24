---
title: Powrót z serwerów nazw firmy Microsoft na zarządzanie własnymi rekordami DNS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506968"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Powrót z serwerów nazw firmy Microsoft na zarządzanie własnymi rekordami DNS

Wcześniej zmieniono rekordy serwera nazw tak, aby wskazują firmę Microsoft (serwer ns1.bdm.microsoftonline.com), ale zdecydowano się teraz zarządzać własnymi rekordami DNS:

W witrynie internetowej rejestratora domen zmień serwer nazw z powrotem na swojego rejestratora lub poprzednie ustawienie. Jeśli nie masz wiedzy na temat systemu DNS, skontaktuj się z zespołem pomocy technicznej u rejestratora domen. Pamiętaj, że propagacja zmian serwera nazw może potrwać do 48 godzin. 

1. W portalu Microsoft 365 administracyjnego przejdź do pozycji **Ustawienia**  >  [**Domains**](https://admin.microsoft.com/Adminportal/Home#/Domains)(Domeny), zaznacz pole wyboru obok domeny i wybierz pozycję Manage DNS (Zarządzaj **systemem DNS).** 

2. W kreatorze wybierz pozycję **Dodaj własne rekordy DNS i** wykonaj zadania kreatora. To zmieni sposób zarządzania systemem DNS, a następnie umożliwi dodanie niestandardowych rekordów DNS wymaganych do obsługi wybranych usług.

Jeśli rekordy serwera nazw zostały zmienione na firmę Microsoft i masz witrynę internetową, możesz dodać rekordy DNS dla tej witryny sieci Web zamiast ponownie zmieniać serwery nazw. Aby uzyskać więcej informacji, zobacz Aktualizowanie rekordów DNS w celu [zachowania witryny sieci Web u obecnego dostawcy hostingu.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)


