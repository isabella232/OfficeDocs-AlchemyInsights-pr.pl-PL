---
title: Przesyłanie wiadomości e-mail przez podanie identyfikatora wiadomości sieciowej
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1a6f9815a36cc267a815ff9757d713afed5d95aec4f7c537135c88cadf26cc51
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929927"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>Przesyłanie wiadomości e-mail przez podanie identyfikatora wiadomości sieciowej

1. W **wysuwanych informacjach** Nowe przesyłanie wybierz pozycję Adres **e-mail** **i identyfikator wiadomości sieciowej**.
2. Wykonaj poniższe czynności, aby znaleźć identyfikator wiadomości e-mail w Outlook:
    1. Kliknij dwukrotnie wiadomość e-mail, aby ją otworzyć.
    1. Wybierz **pozycję Właściwości**  >  **pliku.**
    1. Otwórz Notatnik lub pusty dokument programu Word, a następnie skopiuj  i wklej zawartość znalezioną w polu nagłówków internetowych do otwartego dokumentu, aby poprawić widoczność.
    1. Zlokalizuj pole **X-MS-Exchange-Organization-Network-Message-Id.** Wartość po **:** to identyfikator potrzebny do przesłania.
3. W **obszarze Adresaci**, jeśli wiadomość e-mail trafiła do folderu wiadomości-śmieci dla wszystkich adresatów tej wiadomości, wybierz **pozycję Zaznacz wszystko.** Jeśli nie, wybierz tylko tego użytkownika, który zgłosił problem.
4. W obszarze Przyczyna przesłania , jeśli została wybrane polecenie Powinna zostać zablokowana **,** określ, czy wiadomość powinna zostać zablokowana jako **spam,** **wyłudzanie** informacji **lub** złośliwe **oprogramowanie,** a następnie wybierz **pozycję Prześlij.**

Aby dowiedzieć się więcej, zobacz Jak przesłać podejrzaną [wiadomość-chło-śmieci,](https://go.microsoft.com/fwlink/?linkid=2101479)wyłudzy, adresy URL i pliki do firmy Microsoft w celu skanowania.
