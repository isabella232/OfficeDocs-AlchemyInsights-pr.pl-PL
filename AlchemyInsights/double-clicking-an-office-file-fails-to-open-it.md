---
title: Dwukrotne kliknięcie pliku pakietu Office nie powoduje otwarcia go
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812089"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Dwukrotne kliknięcie pliku pakietu Office nie powoduje otwarcia go

Po dwukrotnym kliknięciu pliku pakietu Office może zostać wyświetlony program otwarty, ale sam plik nie jest otwierany. Może też zostać wyświetlony komunikat o błędzie: "Wystąpił problem podczas wysyłania polecenia do programu". Istnieje wiele powodów tego problemu, ale dwa najczęstsze rozwiązania to:

- W programie Excel upewnij się, że opcja DDE nie jest zaznaczona. Tę opcję można znaleźć, tworząc nowy skoroszyt, a następnie wybierając pozycję **opcje > plików > zaawansowane**. W sekcji **Ogólne** Usuń zaznaczenie pola wyboru **Ignoruj inne aplikacje korzystające z dynamicznej wymiany danych (DDE)**.

- Uruchom naprawę online, aby przywrócić ustawienia domyślne. Kliknij przycisk Start systemu Windows i wyszukaj ciąg "Panel sterowania". Otwórz **Panel sterowania**i przejdź do **apletu programy > programy i funkcje**. Następnie kliknij prawym przyciskiem myszy pozycję **Microsoft Office [Version]** i wybierz polecenie **Zmień > naprawy online**.

Jeśli żadne z tych rozwiązań nie działa, można znaleźć bardziej kompletną listę rozwiązań w artykule pomocy technicznej, [klikając dwukrotnie plik pakietu Office nie może go otworzyć](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).
