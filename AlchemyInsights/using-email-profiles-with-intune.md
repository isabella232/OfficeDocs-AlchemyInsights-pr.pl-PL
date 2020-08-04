---
title: Korzystanie z profili poczty e-mail w usłudze Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555249"
---
# <a name="using-email-profiles-with-intune"></a>Korzystanie z profili poczty e-mail w usłudze Intune

Usługa Intune może służyć do tworzenia i wdrażania profilów poczty e-mail dla macierzystego (wbudowanego) klienta poczty e-mail na wielu platformach urządzeń.

Aby uzyskać informacje o niektórych ograniczeniach związanych z profilami poczty e-mail, w tym o sposobie obsługi obecności istniejących profili i usuwaniu profilów poczty e-mail, zobacz [Dodawanie ustawień poczty e-mail do urządzeń korzystających z usługi Intune](https://docs.microsoft.com/intune/email-settings-configure).

Aby uzyskać więcej informacji na temat tworzenia profilów poczty e-mail dla każdej platformy urządzeń, zobacz:

[Ustawienia urządzenia z systemem Android do konfigurowania poczty e-mail, uwierzytelniania i synchronizacji w usłudze Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Dodawanie ustawień poczty e-mail dla urządzeń z systemem iOS i iPadOS w usłudze Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Ustawienia profilu poczty e-mail w usłudze Microsoft Intune dla urządzeń z systemem Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Ustawienia profilu poczty e-mail dla urządzeń z systemem Windows 10 w usłudze Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Typowy problem z synchronizacją**

**Knox w profilu e-mail systemu Android uniemożliwia synchronizację kontaktów użytkownika, kalendarza i zadań z urządzeniami użytkownika.**

Knox na Android KNOX profil e-mail oferuje administratorowi możliwość zdecydować, które typy zawartości są sync'd do urządzenia, ustawiając każdy z nich włączone.

Jeśli ustawienie dla dowolnego typu zawartości jest ustawione na **Nie skonfigurowano (domyślnie),** ten typ zawartości nie jest synchronizowany automatycznie. Użytkownik może ręcznie włączyć żądany typ zawartości bezpośrednio na urządzeniu, ale ta konfiguracja jest zastępowana przez ustawienie zasad usługi Intune, a synchronizacja zostanie zatrzymana dla tego typu zawartości.

