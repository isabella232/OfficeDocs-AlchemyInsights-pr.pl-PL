---
title: Obraz użytkownika jest nadal wyświetlany na Microsoft Teams schematu organizacyjnego
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422247"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Obraz użytkownika jest nadal wyświetlany na Microsoft Teams schematu organizacyjnego

Jeśli co najmniej jedna osoba w organizacji została wyłączona lub usunięta, a jej zdjęcie profilowe nadal jest widoczne na schematze organizacyjnym, może to być możliwe, że ustawienie **ShowInAddressLists ma** ustawioną wartość False: 

1. Przejdź do centrum administracyjne platformy Microsoft 365 > [Aktywni użytkownicy](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) i wybierz użytkownika, dla których nadal jest wyświetlane zdjęcie. 
1. Wybierz **kartę Poczta** i upewnij się, że dla opcji Pokaż **na globalnej liście adresowej** ustawiono wartość **Nie**.

Jeśli ustawienie **wartości ShowInAddressLists na** **No** nie działa, sprawdź następujące kwestie: 

- Użytkownik może być wyświetlany z listy adresatów w programie Exchange. Aby uzyskać więcej informacji, zobacz [Zarządzanie listami adresów w programie Exchange Online.](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists) 
- Użytkownik może być widoczny z listy adresów w programie Azure Active Directory. Aby uzyskać więcej informacji, [zobacz Set-AzureADUser.](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0) 