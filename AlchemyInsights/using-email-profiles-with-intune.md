---
title: Korzystanie z profilów poczty e-mail w usłudze Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919433"
---
# <a name="using-email-profiles-with-intune"></a>Korzystanie z profilów poczty e-mail w usłudze Intune

Za pomocą usługi Intune można tworzyć i wdrażać profile poczty e-mail dla natywnego (wbudowanego) klienta poczty e-mail na wielu platformach urządzeń.

Aby uzyskać informacje o niektórych ograniczeniach związanych z profilami poczty e-mail, takich jak obsługa obecności istniejących profilów i usuwanie profilów poczty e-mail, zobacz Dodawanie ustawień poczty e-mail do urządzeń za pomocą usługi [Intune.](https://docs.microsoft.com/intune/email-settings-configure)

Aby uzyskać więcej informacji na temat tworzenia profilów poczty e-mail na poszczególnych platformach urządzeń, zobacz:

[Ustawienia urządzeń z systemem Android w celu skonfigurowania poczty e-mail, uwierzytelniania i synchronizacji w usłudze Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Dodawanie ustawień poczty e-mail dla urządzeń z systemem iOS i iPadOS w aplikacji Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Ustawienia profilu poczty e-mail Microsoft Intune urządzeniach z systemem Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Ustawienia profilu poczty e-mail dla urządzeń Windows 10 w Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Częsty problem z synchronizacją**

**KnOX w profilu poczty e-mail w systemie Android zapobiega synchronizacji kontaktów, kalendarza i zadań użytkownika z urządzeniami użytkownika.**

Funkcja KNOX w profilu poczty e-mail knOX systemu Android umożliwia administratorowi określenie, które typy zawartości mają być synchronizowane z urządzeniem przez ustawienie dla każdego z nich wartości włączonych.

Jeśli dla dowolnego z typów zawartości jest ustawione ustawienie Nieskonfigurowane **(ustawienie** domyślne), ten typ zawartości nie jest synchronizowany automatycznie. Użytkownik może ręcznie włączyć typ zawartości bezpośrednio na urządzeniu, ale ta konfiguracja zostanie zastąpiona ustawieniem zasad usługi Intune i synchronizacja tego typu zawartości zostanie zatrzymana.

