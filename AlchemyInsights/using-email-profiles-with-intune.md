---
title: Korzystanie z profilów e-mail w usłudze Intune
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
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653298"
---
# <a name="using-email-profiles-with-intune"></a>Korzystanie z profilów e-mail w usłudze Intune

Usługa Intune może służyć do tworzenia i wdrażania profilów e-mail dla macierzystego (wbudowanego) klienta poczty e-mail na wielu platformach urządzeń.

Aby uzyskać informacje na temat ograniczeń dotyczących profilów e-mail, w tym sposobu obsługi obecności istniejących profilów i usuwania profilów poczty e-mail, zobacz [Dodawanie ustawień poczty e-mail do urządzeń przy użyciu usługi Intune](https://docs.microsoft.com/intune/email-settings-configure).

Aby uzyskać więcej informacji na temat tworzenia profilów poczty e-mail dla poszczególnych platform urządzeń, zobacz:

[Ustawienia urządzeń z systemem Android umożliwiające konfigurowanie poczty e-mail, uwierzytelniania i synchronizacji w usłudze Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Dodawanie ustawień poczty e-mail dla urządzeń z systemem iOS i iPadOS w usłudze Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Ustawienia profilu e-mail w usłudze Microsoft Intune dla urządzeń z systemem Windows Phone 8,1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Ustawienia profilu e-mail dotyczące urządzeń z systemem Windows 10 w usłudze Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Typowy problem z synchronizacją**

**Profil e-mail w programie KNOX w systemie Android uniemożliwia zsynchronizowanie z innymi użytkownikami kontaktów, kalendarza i zadań.**

Profil e-mail KNOX w systemie Android KNOX oferuje administratorowi możliwość podjęcia decyzji, które typy zawartości są synchronizowane z urządzeniem przez ustawienie każdego do włączenia.

Jeśli ustawienie dla dowolnego typu zawartości jest skonfigurowane jako **Nieskonfigurowane** (domyślne), ten typ zawartości nie jest synchronizowany automatycznie. Użytkownik może włączyć ten typ zawartości bezpośrednio na urządzeniu, ale ta konfiguracja zostanie zastąpiona przez ustawienie zasad usługi Intune, a synchronizacja zostanie zatrzymana dla tego typu zawartości.

