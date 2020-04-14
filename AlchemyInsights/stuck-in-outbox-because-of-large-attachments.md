---
title: Utknął w skrzynce nadawczej z powodu dużych załączników
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
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241262"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Naprawianie wiadomości, które utknęły w skrzynce nadawczej

Zaleca się rozpoczęcie od uruchomienia scenariusza ["Mam problemy z wysyłaniem, odbieraniem lub znajdowaniem wiadomości e-mail"](https://aka.ms/SaRA-OutlookSendReceive) z narzędzia [Microsoft Support and Recovery Assistant.](https://diagnostics.office.com/#/)

Gdy wiadomość utknie w skrzynce nadawczej, najbardziej prawdopodobną przyczyną jest duży załącznik lub opcja "Wyślij natychmiast po podłączeniu" nie jest włączona.

**Usuń duży załącznik**

1. W programie Outlook wybierz pozycję **Wyślij / Odbierz** > **pracę w trybie offline**. 
2. W okienku nawigacji wybierz pozycję **Skrzynka nadawcza**. W tym miejscu możesz: 
    - Usuń wiadomość (zaznacz ją, a następnie wybierz pozycję **Usuń**).
    - Przeciągnij wiadomość do folderu Wersje robocze, kliknij dwukrotnie, aby ją otworzyć, a następnie usuń zaznacz załącznik, a następnie wybierz pozycję **Usuń**).
3. Jeśli pojawi się błąd informujący, że program Outlook próbuje przesłać wiadomość, zamknij program Outlook. Może upłynąć kilka chwil, aby wyjść. Jeśli program Outlook nie zostanie zamknięty, naciśnij klawisze Ctrl+Alt+Delete i wybierz pozycję **Rozpocznij Menedżera zadań**. W Menedżerze zadań wybierz kartę **Procesy,** przewiń w dół do programu outlook.exe i wybierz pozycję **Zakończ proces**.
4. Po zamknięciu programu Outlook uruchom go ponownie i powtórz kroki 2 i 3. 
5. Po usunięciu załącznika kliknij przycisk **Wyślij / Odbierz** > **pracę w trybie offline,** aby wznowić pracę w trybie online. 

Wiadomości utkną również w skrzynce nadawczej po **kliknięciu przycisku Wyślij**, ale nie masz połączenia. Kliknij **przycisk Wyślij / Odbierz** i spójrz na przycisk Praca w **trybie offline.** Jeśli jest niebieski, jesteś rozłączony. Kliknij go, aby się połączyć (przycisk zmieni kolor na biały) i kliknij przycisk **Wyślij wszystko**.
 
**Włącz wysyłanie natychmiast po podłączeniu**
 
1. Na karcie Plik kliknij pozycję **Opcje**.

2. W oknie dialogowym Opcje programu Outlook kliknij pozycję **Zaawansowane**.

3. W sekcji Wyślij i odbierz kliknij, aby natychmiast włączyć **opcję Wyślij po podłączeniu**. Kliknij przycisk **OK**.
 
Aby uzyskać szczegółowe informacje, zobacz:
- [Klip wideo: wysyłanie lub usuwanie zablokowanej wiadomości e-mail](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Poczta e-mail pozostaje w folderze Skrzynka nadawcza do czasu ręcznego zainicjowania operacji wysyłania/odbierania w programie Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
