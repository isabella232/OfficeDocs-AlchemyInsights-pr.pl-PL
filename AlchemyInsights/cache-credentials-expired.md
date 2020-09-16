---
title: 'Błąd: nie można przekazać ani pobrać zmian, ponieważ poświadczenia w pamięci podręcznej wygasły'
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "3534"
- "9001489"
ms.openlocfilehash: 8105fa7b311bc932f95c8bff4d6b58ed9aabe74a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734489"
---
# <a name="error-we-cant-upload-or-download-your-changes-because-your-cached-credentials-have-expired"></a>Błąd: nie można przekazać ani pobrać zmian, ponieważ poświadczenia w pamięci podręcznej wygasły

W przypadku zapisywania plików w aplikacji OneDrive, jeśli zostanie wyświetlony komunikat o błędzie zawierający frazę **"Twoje buforowane poświadczenia wygasły"**, wykonaj następujące czynności:

1. Zamknij wszystkie aplikacje pakietu Office.
1. Otwórz Menedżera poświadczeń i w polu wyszukiwania na pasku zadań wpisz nazwę **Menedżer poświadczeń** , a następnie wybierz pozycję **Panel sterowania Menedżera poświadczeń**.
1. Wybierz pozycję **poświadczenia systemu Windows**.
1. Znajdź dowolny wpis, który zaczyna się od aplikacji Word **OneDrive**.
1. Zaznacz wpis, a następnie naciśnij klawisz **Remove**.
1. Zamknij Menedżera poświadczeń, a następnie kliknij prawym przyciskiem myszy niebieską chmurę w usłudze Systray, a następnie wybierz polecenie **Zamknij usługę OneDrive**.
1. W polu wyszukiwania na pasku zadań wpisz **OneDrive** , a następnie wybierz pozycję **Aplikacja OneDrive** , aby uruchomić aplikację OneDrive.
1. Zalogowanie się do usługi OneDrive, a następnie spróbuj zapisać plik w usłudze OneDrive.
