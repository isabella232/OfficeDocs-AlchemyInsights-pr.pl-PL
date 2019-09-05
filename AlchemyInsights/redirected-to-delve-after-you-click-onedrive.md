---
title: OneDrive dla Business Web OneDrive przekierowuje do Delve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 8ba296c6986c767939ef51076551f95719d11aa2
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752258"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Przekierowano do Delve po kliknięciu OneDrive

Aby rozwiązać ten problem, administrator pakietu Office 365 musi przyznać użytkownikom prawo do tworzenia witryny Moje witryny. Dzieje się tak, ponieważ na stronie Moje witryny jest tworzona Strona OneDrive dla firm.

Aby udzielić tego prawa, wykonaj następujące kroki:

1. W centrum administracyjnego programu SharePoint, kliknij przycisk **Profile użytkownika**.

2. W sekcji **osoby** kliknij przycisk **Zarządzaj uprawnieniami użytkownika**.

3. Dodaj użytkowników, którzy potrzebują uprawnień do tworzenia witryny Moje witryny. Domyślnie to ustawienie jest ustawione dla **wszystkich z wyjątkiem użytkowników zewnętrznych**.

4. Po dodaniu użytkownika, użytkowników lub grupy, upewnij się, że dodano użytkownika, użytkowników lub grupy jest zaznaczone, przewiń do sekcji **uprawnienia** , a następnie zaznacz pole wyboru obok **Tworzenie witryny osobistej (wymagane dla magazynu osobistego, kanału informacyjnego i po treści)**.

5. Kliknij przycisk **OK**, a następnie użytkownik przejdź do strony OneDrive, aby utworzyć witrynę.
