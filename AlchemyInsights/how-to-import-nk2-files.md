---
title: how-to-import-nk2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043216"
---
# <a name="how-to-import-nk2-files"></a>Jak zaimportować pliki nk2 

Po uruchomieniu programu Microsoft Outlook 2013, Outlook 2016, Outlook 2019 lub Outlook dla Microsoft 365 po raz pierwszy pamięć podręczna nicków (przechowywana w pliku nk2 o nazwie profilu) jest importowana do ukrytej wiadomości w domyślnym magazynie wiadomości.

Aby zaimportować pliki nk2 do programu Outlook 2013, Outlook 2016, Outlook 2019 lub Outlook dla Microsoft 365 upewnij się, że plik nk2 znajduje się w następującym folderze: %appdata%\Microsoft\Outlook

**Uwaga:** plik nk2 musi mieć taką samą nazwę, jak bieżący Outlook 2013 lub Outlook 2016 profilu. Domyślnie nazwa profilu to "Outlook". Aby sprawdzić nazwę profilu, wykonaj następujące czynności: 
1. Kliknij przycisk **Start**, a następnie kliknij polecenie **Panel sterowania**.
2. Kliknij dwukrotnie pozycję **Poczta.**
3. W oknie dialogowym Konfiguracja poczty wybierz pozycję **Pokaż profile**.
4. Kliknij przycisk **Start** > **Uruchom**.
5. W polu **Otwórz** wpisz tekst *outlook.exe /importnk2,* a następnie wybierz przycisk **OK.** 

Po zaimportowaniu pliku nk2 zawartość pliku jest scalona z istniejącą pamięcią podręczną nicków przechowywaną w skrzynce pocztowej.

**Uwaga:** po następnym uruchomieniu programu Outlook 2013, Outlook 2016, Outlook 2019 lub Outlook dla Microsoft 365 zostanie zmieniona nazwa pliku nk2 na Outlook dla Microsoft 365. Jeśli chcesz ponownie zaimportować plik nk2, najpierw usuń rozszerzenie starej nazwy pliku.

Aby uzyskać więcej informacji, zobacz Importowanie lub kopiowanie listy [autouzupełnień na inny komputer.](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)