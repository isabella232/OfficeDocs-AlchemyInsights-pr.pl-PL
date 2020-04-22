---
title: jak importować-nk2-pliki
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 83d30b2d62908db791f21ec5ed7fd5537e7a0944
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759342"
---
# <a name="how-to-import-nk2-files"></a>Jak zaimportować pliki .nk2 

Po uruchomieniu programu Microsoft Outlook 2013, Outlook 2016, Outlook 2019 lub Outlook dla usługi Microsoft 365 po raz pierwszy pamięć podręczna pseudonimu (przechowywana w pliku .nk2 *nazwy profilu)* jest importowana do ukrytej wiadomości w domyślnym magazynie wiadomości.

Aby zaimportować pliki nk2 do programu Outlook 2013, Outlook 2016, Outlook 2019 lub Outlook dla usługi Microsoft 365, upewnij się, że plik .nk2 znajduje się w następującym folderze: %appdata%\Microsoft\Outlook

**Uwaga:** Plik .nk2 musi mieć taką samą nazwę jak bieżący profil programu Outlook 2013 lub Outlook 2016. Domyślnie nazwa profilu to "Outlook". Aby sprawdzić nazwę profilu, wykonaj następujące czynności: 
1. Kliknij **przycisk Start**, a następnie kliknij pozycję Panel **sterowania**.
2. Kliknij dwukrotnie pozycję **Poczta**.
3. W oknie dialogowym Ustawienia poczty wybierz pozycję **Pokaż profile**.
4. Wybierz **pozycję Rozpocznij** > **bieg**.
5. W polu **Otwórz** wpisz program *outlook.exe /importnk2*, a następnie wybierz przycisk **OK**. 

Po zaimportowaniu pliku .nk2 zawartość pliku zostanie scalona z istniejącą pamięcią podręczną pseudonimów przechowywaną w skrzynce pocztowej.

**Uwaga:** Nazwa pliku .nk2 została zmieniona na rozszerzenie nazwy .old przy następnym uruchomieniu programu Outlook 2013, Outlook 2016, Outlook 2019 lub Outlook dla microsoftu 365. Jeśli chcesz ponownie zaimportować plik .nk2, najpierw usuń rozszerzenie nazwy .old.

Aby uzyskać więcej informacji, zobacz [Importowanie lub kopiowanie listy autouzupełniania na inny komputer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).