---
title: Naprawianie pliku pst przed zaimportowaniem
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1226"
- "1800027"
ms.assetid: ''
ms.openlocfilehash: 1ed37192a6b054b745fd48fbc01a6b00fa7074ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799106"
---
# <a name="repair-pst-file-before-importing"></a>Naprawianie pliku pst przed zaimportowaniem

Przed zaimportowaniem pliku pst w programie Outlook sprawdź, czy plik nie jest uszkodzony, naprawiając plik:

1. Zakończ pracę programu Outlook.

2. Znajdowanie i uruchamianie `Scanpst.exe` w folderze programu pakietu Office (C:\Program Files (x86) \Microsoft Office\root\Office \<Version\> lub C:\Program Files\Microsoft Office\root\Office \<Version\> ).

3. W **narzędziu do naprawy skrzynki odbiorczej programu Microsoft Outlook**kliknij przycisk **Przeglądaj** , aby znaleźć plik PST (na przykład w witrynie C:\Users \\<username \> \AppData\Local\Microsoft\Outlook). Wybierz plik pst, a następnie kliknij przycisk **Otwórz**.

4. Kliknij przycisk **Rozpocznij** , aby rozpocząć skanowanie.

5. Jeśli w pliku znajdują się błędy, kliknij pozycję **napraw**, a następnie kliknij przycisk **OK** po zakończeniu naprawy.

6. Spróbuj ponownie zaimportować plik pst w programie Outlook.

Aby uzyskać więcej informacji, zobacz [naprawianie plików danych programu Outlook](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) i [Rozwiązywanie problemów z importowaniem pliku pst programu Outlook](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).
