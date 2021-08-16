---
title: Yammer problemów z licencjonowaniem
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989744"
---
# <a name="yammer-licensing-issues"></a>Yammer problemów z licencjonowaniem

Wszyscy użytkownicy muszą mieć licencję, aby korzystać z usługi Yammer Enterprise, ale domyślnie Yammer nie wymaga, aby użytkownicy mieli licencję na dostęp do usługi. Gdy administrator zmieni to ustawienie w celu blokowania Microsoft 365 użytkowników bez Yammer licencji, użytkownicy, którym nie przypisano licencji Yammer Enterprise, nie mogą uzyskać dostępu do Yammer usługi. Aby uzyskać więcej informacji, zobacz [Zarządzanie Yammer użytkownikami w aplikacji Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Po usunięciu licencji użytkownikom kafelek licencji Yammer nie jest już wyświetlany, a inne usługi mogą ukrywać funkcje przy użyciu usuwania licencji. W innych przypadkach funkcje mogą być nadal wyświetlane, ale wymagają przypisania licencji do działania.  

**Licencja nie jest aktualizowana dla użytkownika**  

Od czasu do czasu użytkownikowi przypisywana jest licencja, ale nadal nie może on uzyskać dostępu do Yammer. Opóźnienia najprawdopodobniej występują w trakcie przypisywania licencji masowej. Yammer użytkownicy mogą nie być aktualizowani w tej samej kolejności co zmiany licencji w usłudze Azure AD, ponieważ system działa asynchronicznie. Przed otwarciem sprawy pomocy technicznej zgłoś problemy z synchronizacją licencji, poczekaj do 24 godzin.  

**Zbiorcze przypisywanie licencji**  

Licencje można przypisywać za pośrednictwem centrum administracyjnego lub skryptów programu PowerShell. Aby uzyskać więcej informacji, zobacz [Przypisywanie](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) licencji do użytkowników i Przypisywanie licencji do kont użytkowników za pomocą programu [Office 365 PowerShell.](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

Pomoc techniczna firmy Microsoft nie udziela pomocy przy tworzeniu skryptów, ale dostępna jest Yammer przypisywania licencji. Aby uzyskać więcej informacji, zobacz [Zarządzanie Yammer licencji przy użyciu programu Windows PowerShell.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)