---
title: Read-Only komunikat konserwacji podczas próby użycia SharePoint lub OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 376b653b18857103586e25edd0ad6801a7bbe0a1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329458"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only komunikat konserwacji podczas próby użycia SharePoint lub OneDrive

Użytkownicy mogą otrzymać komunikat **Tylko** do odczytu dla konserwacji podczas próby użycia SharePoint lub OneDrive w jednym z następujących scenariuszy. 

-   Planowane lub aktywne działanie konserwacyjne.  Sprawdź je, przechodząc do [Centrum wiadomości.](https://portal.office.com/adminportal/home#/messagecenter)
-   Może mieć miejsce zdarzenie o wysokim priorytecie aktywnej usługi. Sprawdź, czy nie ma żadnych porad i zdarzeń, przechodząc do [tematu Kondycja usługi.](https://portal.office.com/adminportal/home#/servicehealth)
-   Przykładowy scenariusz odzyskiwania autoodzywu, który może wystąpić z powodu nieoczekiwanych zdarzeń na serwerach, które mogą trwać dłużej niż 30 minut. 
    
    Nie ma żadnych wpisów w Centrum wiadomości ani kondycji usługi dotyczącej tych drobnych odzyskanych danych, ale wkrótce powinno się wrócić do normalnego stanu.

W bardzo niewielu przypadkach zauważyliśmy, że przyczyną jest jeden z trzech wymienionych powyżej scenariuszy i przywrócono usługę, ale pamięć podręczna przeglądarki użytkowników nie została wyczyszczana.

Przed przejściem do witryny spróbuj wyczyścić pamięć podręczną przeglądarki.

1. W przeglądarce Microsoft Edge wybierz pozycję **Ustawienia**, a następnie wybierz pozycję **Prywatność i zabezpieczenia**.
2. W **obszarze Wyczyść przeglądanie** wybierz pozycję **Wybierz, co chcesz wyczyścić**.
3. Wybierz pozycję **Pliki cookie i zapisane dane witryn** internetowych, a następnie wybierz pozycję **Wyczyść**.

**Uwaga:** Te kroki mogą się różnić w przypadku korzystania z innych przeglądarek, takich jak Mozilla Firefox lub Google Chrome.

**Uwaga:** Innym rozwiązaniem jest otwarcie SharePoint lub OneDrive w nowym oknie InPrivate.