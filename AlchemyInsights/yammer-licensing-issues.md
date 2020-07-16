---
title: Problemy z licencjonowaniem usługi Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148316"
---
# <a name="yammer-licensing-issues"></a>Problemy z licencjonowaniem usługi Yammer

Wszyscy użytkownicy muszą mieć licencję na korzystanie z usługi Yammer Enterprise, ale domyślnie usługa Yammer nie wymaga od użytkowników licencji na dostęp do usługi. Gdy administrator zmieni to ustawienie, aby zablokować użytkowników usługi Microsoft 365 bez licencji Yammer, użytkownicy, którym nie przypisano licencji Yammer Enterprise, nie mogą uzyskać dostępu do usługi Yammer. Aby uzyskać więcej informacji, zobacz [Zarządzanie licencjami użytkowników usługi Yammer w usłudze Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Gdy licencje są usuwane z użytkowników, kafelek Yammer nie jest już wyświetlany, a inne usługi mogą używać usuwania licencji do ukrywania funkcji. W innych przypadkach funkcje mogą nadal pojawiać się, ale wymagają przypisania licencji do działania.  

**Licencja nie jest aktualizowana dla użytkownika**  

Od czasu do czasu użytkownikowi jest przypisywana licencja, ale nadal nie może uzyskać dostępu do usługi Yammer. Opóźnienia są bardziej prawdopodobne, gdy trwa przypisanie licencji masowej. Użytkownicy usługi Yammer mogą nie być aktualizowane w tej samej kolejności, jak licencje są zmieniane w usłudze Azure AD, ponieważ system działa asynchronicznie. Poczekaj do 24 godzin przed otwarciem sprawy pomocy technicznej, aby zgłosić problemy z synchronizacją licencji.  

**Zbiorcze przydzielanie licencji**  

Licencje można przypisać za pośrednictwem centrum administracyjnego lub skryptów programu PowerShell. Aby uzyskać więcej informacji, zobacz [Przypisywanie licencji użytkownikom](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) i [Przypisywanie licencji do kont użytkowników w usłudze Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Pomoc techniczna firmy Microsoft nie zapewnia pomocy w tworzeniu skryptów, ale dostępna jest dokumentacja dotycząca przypisywania licencji usługi Yammer. Aby uzyskać więcej informacji, zobacz [Zarządzanie licencjami usługi Yammer przy użyciu programu Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).