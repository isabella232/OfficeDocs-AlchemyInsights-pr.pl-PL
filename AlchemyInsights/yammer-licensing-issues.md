---
title: Problemy z licencjonowaniem usługi Yammer
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
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657286"
---
# <a name="yammer-licensing-issues"></a>Problemy z licencjonowaniem usługi Yammer

Wszyscy użytkownicy muszą mieć licencję na korzystanie z usługi Yammer Enterprise, ale domyślnie usługa Yammer nie wymaga posiadania licencji na dostęp do usługi. Gdy administrator zmieni ustawienie w celu zablokowania użytkowników programu Microsoft 365 bez licencji usługi Yammer, użytkownicy, którym nie przypisano licencji usługi Yammer Enterprise, mogą uzyskać dostęp do usługi Yammer. Aby uzyskać więcej informacji, zobacz [Zarządzanie licencjami użytkowników usługi Yammer w pakiecie Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Po usunięciu licencji od użytkowników kafelek usługi Yammer nie jest już wyświetlany, a inne usługi mogą używać usuwania licencji w celu ukrycia funkcji. W innych przypadkach nadal mogą być wyświetlane funkcje, ale wymagane jest przypisanie licencji.  

**Licencja nie jest aktualizowana dla użytkownika**  

Czasami użytkownik ma przypisaną licencję, ale nadal nie może uzyskać dostępu do usługi Yammer. Prawdopodobieństwo wystąpienia opóźnień jest większe, gdy trwa przydział licencji masowej. Użytkownicy usługi Yammer mogą nie zostać zaktualizowani w takiej samej kolejności, w jakiej licencje są zmieniane w usłudze Azure AD, ponieważ system jest uruchamiany asynchronicznie. Poczekaj na 24 godziny przed otwarciem sprawy pomocy technicznej, aby raportować problemy z synchronizacją licencji.  

**Przydział licencji zbiorczej**  

Licencje można przypisywać za pośrednictwem Centrum administracyjnego lub skryptów programu PowerShell. Aby uzyskać więcej informacji, zobacz [Przypisywanie licencji do użytkowników](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) i [Przypisywanie licencji do kont użytkowników przy użyciu programu Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Pomoc techniczna firmy Microsoft nie zapewnia pomocy w tworzeniu skryptów, ale dostępna jest dokumentacja dotycząca przydziału licencji usługi Yammer. Aby uzyskać więcej informacji, zobacz [Zarządzanie licencjami usługi Yammer za pomocą programu Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).