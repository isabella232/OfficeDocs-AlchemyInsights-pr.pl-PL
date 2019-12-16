---
title: Tylko do odczytu dla konserwacji komunikat podczas próby użycia programu SharePoint lub OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051291"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Tylko do odczytu dla konserwacji komunikat podczas próby użycia programu SharePoint lub OneDrive

Użytkownicy mogą odbierać **tylko do odczytu dla komunikat konserwacji** podczas próby użycia programu SharePoint lub OneDrive dla jednego z następujących scenariuszy. 

-   Planowane lub aktywne czynności konserwacyjne.  Sprawdź je, przechodząc do [centrum wiadomości](https://portal.office.com/adminportal/home#/messagecenter).
-   Zdarzenia o wysokim priorytecie, aktywne usługi, które mogą mieć miejsce. Sprawdź, czy nie ma żadnych porad/incydentów, przechodząc do [usługi kondycji](https://portal.office.com/adminportal/home#/servicehealth).
-   Niewielki scenariusz odzyskiwania Auto-Healing, który może się wydarzy z powodu nieoczekiwanych zdarzeń na serwerach, które mogą trwać krócej niż 30 min lub więcej. 
    
    Nie ma żadnych wiadomości Center lub usługi zdrowia stanowisk dla tych drobnych odzyskuje, ale należy wrócić do normalnego bardzo szybko.

W bardzo niewielu przypadkach zaobserwowaliśmy, że jeden z trzech scenariuszy wymienionych powyżej był przyczyną, a usługa została przywrócona, ale pamięć podręczna przeglądarki użytkowników nie została wyczyszczona.

Spróbuj wyczyścić pamięć podręczną przeglądarki przed nawigacją do witryny.

1. W przeglądarce Microsoft Edge wybierz pozycję **Ustawienia**, a następnie wybierz pozycję **prywatność i zabezpieczenia**.
2. W obszarze **Wyczyść przeglądanie**wybierz pozycję **Wybierz, co chcesz wyczyścić**.
3. Wybierz **pliki cookie i zapisane dane witryny**, a następnie wybierz pozycję **Wyczyść**.

>[!Note] 
> Te kroki mogą się różnić w przypadku korzystania z innych przeglądarek, takich jak Mozilla Firefox lub Google Chrome.

>[!Note] 
> Inną opcją byłoby otworzyć witrynę programu SharePoint lub OneDrive w nowym oknie InPrivate.