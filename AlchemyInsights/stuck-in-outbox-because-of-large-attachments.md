---
title: Stuck in Skrzynka nadawcza z powodu dużych załączników
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441315"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Naprawianie wiadomości, które są zablokowane w skrzynce nadawcza

Zaleca się rozpoczęcie od uruchomienia scenariusza ["Mam problemy z wysyłaniem, odbieraniem lub znajdowaniu wiadomości e-mail"](https://aka.ms/SaRA-OutlookSendReceive) w narzędziu [Pomoc techniczna i Asystent odzyskiwania firmy Microsoft](https://diagnostics.office.com/#/) .

Gdy wiadomość zostaje zablokowana w skrzynce nadawcza, najbardziej prawdopodobną przyczyną są:
- Duże załączniki.
- Opcja **Wyślij natychmiast po podłączeniu** nie jest włączona.

Aby usunąć duże załączniki: 

1. W programie Outlook wybierz opcję **Wyślij/Odbierz** > **pracę w trybie offline**. 
2. W okienku nawigacji wybierz opcję **Skrzynka nadawcza**. Tutaj możesz: 
    - Usuń wiadomość (zaznacz ją, a następnie wybierz **Usuń**).
    - Przeciągnij wiadomość do folderu wersje robocze, kliknij dwukrotnie, aby ją otworzyć, a następnie Usuń załącznik i wybierz go, a następnie wybierz pozycję **Usuń**).
3. Jeśli zostanie wyświetlony komunikat o błędzie informujący, że program Outlook próbuje przesłać wiadomość, Zamknij program Outlook. Wyjście może zająć kilka chwil. Jeśli program Outlook nie zostanie zamknięty, naciśnij kombinację Ctrl + Alt + Delete i wybierz pozycję **Uruchom Menedżera zadań**. W Menedżerze zadań wybierz kartę **procesy** , przewiń w dół do Outlook. exe i wybierz **Zakończ proces**.
4. Po zamknięciu programu Outlook, uruchom go ponownie i powtórz kroki 2 i 3. 
5. Po usunięciu załącznika kliknij przycisk **Wyślij/Odbierz** > **pracę w trybie offline** , aby wznowić pracę w trybie online. 

Wiadomości również utknąć w skrzynce nadawcza po kliknięciu przycisku **Wyślij**, ale nie są podłączone. Kliknij przycisk **Wyślij/Odbierz** i spójrz na przycisk **Pracuj w trybie offline** . Jeśli jest niebieska, zostanie rozłączona. Wybierz go, aby nawiązać połączenie (przycisk zmieni kolor na biały) i kliknij przycisk **Wyślij wszystko**.
 
Aby włączyć funkcję **Wyślij natychmiast po podłączeniu**:
 
- Wybierz **** > **** opcje >  pliku**Zaawansowane**.
W **wysyłania i odbierania** sekcji, wybierz opcję **Wyślij natychmiast po podłączeniu**, a następnie wybierz **OK**.
 
Aby uzyskać szczegółowe informacje, zobacz:
- [Wideo: wysyłanie lub usuwanie zablokowej wiadomości e-mail](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Wiadomość e-mail pozostaje w folderze Skrzynka nadawcza do momentu ręcznego zainicjowania operacji wysyłania/odbierania w programie Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
