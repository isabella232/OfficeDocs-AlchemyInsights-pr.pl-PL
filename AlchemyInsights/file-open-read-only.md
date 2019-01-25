---
title: Otwieranie pliku tylko do odczytu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.openlocfilehash: 46b2489e86c018b3cbd6feb07a3a2e397de383b6
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499536"
---
# <a name="file-open-read-only"></a>Otwieranie pliku tylko do odczytu

Może się okazać, że otwierając pliki, otworzyć jako tylko do odczytu. W niektórych przypadkach to aby zwiększyć bezpieczeństwo, takie jak otwierając pliki z Internetu, a innym razem, mogą występować z powodu ustawienia, które mogą być zmieniane. Poniżej przedstawiono kilka scenariuszy, w którym plik zostanie otwarty tylko do odczytu i czynności, jakie można podjąć, aby to zmienić.
  
 **Mój program antywirusowy jest przyczyną je otworzyć tylko do odczytu**
  
Niektóre programy antywirusowe mogą chronić potencjalnie niebezpiecznych plików przez otwarcie ich jako tylko do odczytu. Należy skontaktować się z dostawcą oprogramowania antywirusowego, aby dowiedzieć się, jak dostosować te ustawienia. BitDefender, na przykład ma zawartość na dodanie wykluczeń aplikacji tutaj: [jak dodać aplikację lub wykluczenia procesu w centrum sterowania Bitdefender](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).
  
 **Właściwości pliku ustawiono atrybut tylko do odczytu?**
  
Można sprawdzić właściwości pliku prawym przyciskiem myszy plik i wybierz polecenie Właściwości. Jeśli atrybut tylko do odczytu jest zaznaczone, można usunąć jego zaznaczenie i kliknij OK.
  
 **Zawartość jest w widoku chronionym**
  
Pliki z Internetu i innych potencjalnie niebezpiecznych lokalizacjach mogą zawierać wirusy, robaki lub inne rodzaje złośliwego oprogramowania, które mogą uszkodzić komputer. Jest to również często z załączników wiadomości e-mail lub pliki pobrane. Aby pomóc w ochronie tego komputera, pliki z lokalizacji tych potencjalnie niebezpieczne są otwierane w widoku chronionym. Za pomocą widoku chronionego, można czytać pliku i wyświetlić jego zawartość przy jednoczesnym zmniejszeniu ryzyka. Aby uzyskać więcej informacji w widoku chronionym i sposobu zmieniania ustawień, w tym artykule: [Co to jest widok chroniony?](https://support.office.com/en-us/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)
  
 **OneDrive jest zapełniony?**
  
Jeśli plik jest przechowywany na OneDrive i z przestrzeni magazynowania jest pełny, nie można zapisać dokumentu, dopóki nie są pod przydzielonego miejsca. Wolne miejsce na dysku OneDrive można sprawdzić, klikając ikonę OneDrive w Centrum powiadomień i wybierając polecenie Zarządzanie magazynem, lub możesz przejść do [http://onedrive.live.com](http://onedrive.live.com), zaloguj się i zanotuj ilość zajętego miejsca w dolnym lewym rogu ekranu.
  
 **Urząd jest aktywowany?**
  
Jeśli pakietu Office nie jest aktywowany lub jeśli Twoja subskrypcja wygasła, może być w trybie tylko do odczytu trybie zmniejszonej funkcjonalności. Szczegółowe informacje na temat aktywacji pakietu Office: [produkt bez licencji i błędów aktywacji pakietu Office](https://support.office.com/en-us/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).
  
 **Jeśli wszystkie inne źródła zawiodą...**
  
- Spróbuj ponownie uruchomić komputer
    
- Zainstaluj aktualizacje pakietu Office
    
- Wykonać naprawy w trybie Online pakietu Office
    

