---
title: Problemy z aplikacją Teams często występujące u klientów z instytucji edukacyjnych
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000701"
- "3831"
- "3832"
ms.openlocfilehash: d61d4484c720db51e7377201067008192940d1f8
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43739446"
---
# <a name="teams-common-issues-for-education-customers"></a>Problemy z aplikacją Teams często występujące u klientów z instytucji edukacyjnych

**Dla klientów z instytucji edukacyjnych**:

Jeśli potrzebujesz pomocy przy wdrażaniu aplikacji Teams jako narzędzia do nauczania zdalnego, przejdź na stronę [FastTrack Center](https://www.microsoft.com/fasttrack), aby przesłać wniosek. Zobacz poniższe problemy z aplikacją Teams, które często występują u klientów z instytucji edukacyjnych:

- Wyświetla Ci się komunikat „**Coś Cię omija!**”? Upewnij się, że poczyniono wszystkie kroki opisane w artykule [Włączanie usługi Microsoft Teams dla szkoły](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams). W dzierżawach edukacyjnych usługa Microsoft Teams nie jest domyślnie włączona. Należy najpierw włączyć tę funkcję.

- **Dopiero zaczynasz korzystać z aplikacji Teams?** Przeczytaj artykuł [Zdalne nauczanie i uczenie się w ramach pakietu Office 365 Education](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4), aby zapoznać się z najnowszymi wskazówkami dotyczącymi konfigurowania szkoły, planowania lekcji, wirtualnych spotkań i udostępniania treści uczniom i studentom.

- Po udostępnieniu aplikacji Teams użytkownicy będą mogli ją uruchomić poprzez zainstalowanie wersji [klasycznych](https://docs.microsoft.com/MicrosoftTeams/get-clients#desktop-client) i [klientów mobilnych](https://docs.microsoft.com/MicrosoftTeams/get-clients#mobile-clients) lub za pomocą przeglądarki na stronie https://teams.microsoft.com.

- **Włącz dostęp gości do aplikacji Teams**: sprawdź [listę kontrolną dostępu gości do aplikacji Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist), aby upewnić się, że poczyniono wszystkie niezbędne kroki.
    - [Objaśnienie dostępu gości do aplikacji Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access)
    - [Konfigurowanie — lista kontrolna dostępu gości do aplikacji Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [Jak gość dołącza do zespołu](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Spotkania i konferencje telefoniczne w aplikacji Teams**: potrzebujesz pomocy dotyczącej włączania lub konfigurowania konferencji głosowych w aplikacji Microsoft Teams? Czy ten użytkownik został ostatnio utworzony? Jeśli tak, trzeba odczekać od 2 do 24 godzin, aby ustawienia zaczęły obowiązywać. Aby sprawdzić, czy użytkownik ma licencję na konferencje głosowe oraz domyślny numer płatny:
    1. Przejdź do pozycji Aktywni użytkownicy i wybierz odpowiedniego użytkownika.
    2. W zależności od wersji centrum administracyjnego wybierz pozycję **Licencje i aplikacje** lub kliknij **Edytuj** w sekcji **Licencje na produkt**.
    3. Upewnij się, że użytkownik ma wybrane licencje na Konferencje głosowe, Microsoft Teams oraz usługę Skype dla firm Online (plan 2).
    4. W sekcji Centra administracyjne użytkownika kliknij pozycję **Pokaż wszystko**, a następnie kliknij pozycję **Teams**.
    5. W centrum administracyjnym aplikacji Microsoft Teams kliknij pozycję **Stary portal**.
    6. W centrum administracyjnym programu Skype dla firm kliknij pozycję **konferencja głosowa**, a następnie **użytkownicy**.
    7. Zaznacz danego użytkownika i sprawdź, czy ma domyślny numer płatny.

    Aby uzyskać więcej informacji, przeczytaj artykuł [Pakiety telefoniczne](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365) lub zadzwoń do zespołu ds. rozliczeń z przedsiębiorstwami firmy Microsoft, aby uzyskać pomoc dotyczącą licencji.

    Dodatkowe zasoby

    - [Spotkania i konferencje w aplikacji Microsoft Teams](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Konferencje głosowe](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **Zasady dotyczące spotkań**: zasady dotyczące spotkań służą do określania, które funkcje są dostępne dla uczestników spotkania zaplanowanego przez użytkowników w Twojej organizacji. Po utworzeniu zasady i wprowadzeniu zmian możesz przypisać użytkowników do danej zasady.

    - **Zmienianie lub tworzenie zasady dotyczącej spotkań**: aby zmienić lub utworzyć zasadę dotyczącą spotkania, przejdź do **centrum administracyjnego usługi Microsoft Teams > Spotkania > Zasady dotyczące spotkań**. Wybierz zasadę z listy i kliknij **Dodaj**. Jeśli tworzysz nową zasadę, dodaj nazwę i opis. Nazwa nie może zawierać znaków specjalnych ani być dłuższa niż 64 znaki. Wybierz odpowiednie ustawienia, a następnie kliknij przycisk **Zapisz**. 
    
        Załóżmy na przykład, że masz wielu użytkowników i chcesz ograniczyć przepustowość, która zostanie wykorzystana do obsługi ich spotkania. W takim przypadku należy utworzyć nową zasadę niestandardową o nazwie „Ograniczona przepustowość” i wyłączyć następujące ustawienia:

        W sekcji **Dźwięk i wideo**:
        - wyłącz opcję **Zezwalaj na nagrywanie w chmurze**;
        - wyłącz opcję **Zezwalaj na IP wideo**.

        W sekcji **Udostępnianie treści**:

        - wyłącz tryb udostępniania ekranu;
        - wyłącz opcję **Zezwalaj na tablicę**;
        - wyłącz opcję **Zezwalaj na notatki udostępnione**.

        Następnie **przypisz tę zasadę do użytkowników**:

    1. W lewej części obszaru nawigacji centrum administracyjnego usługi Microsoft Teams przejdź do pozycji **Użytkownicy**, a następnie kliknij użytkownika.
    2. Kliknij z lewej strony nazwy użytkownika, aby go zaznaczyć, a następnie kliknij pozycję **Edytuj ustawienia**.
    3. W sekcji **Zasady dotyczące spotkań** wybierz zasadę, którą chcesz przydzielić, I kliknij pozycję **Zastosuj**.

    Aby przypisać zasadę kilku użytkownikom jednocześnie, zapoznaj się z artykułem [Masowe edytowanie ustawień użytkowników aplikacji Teams](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk).

    Możesz też wykonać następujące czynności:
    1. W lewej części obszaru nawigacji centrum administracyjnego usługi Microsoft Teams przejdź do pozycji **Spotkania > Zasady dotyczące spotkań**.
    2. Kliknij po lewej stronie nazwy zasady, aby ją zaznaczyć.
    3. Kliknij pozycję **Zarządzaj użytkownikami**.
    4. W okienku **Zarządzaj użytkownikami** wyszukaj użytkownika według nazwy wyświetlanej lub nazwy użytkownika, zaznacz nazwę, a następnie kliknij pozycję **Dodaj**. Powtórz ten krok dla każdego użytkownika, którego chcesz dodać.
    5. Po zakończeniu dodawania użytkowników kliknij pozycję **Zapisz**.

- **Rozwiązywanie problemów związanych z brakującą konsolą wybierania numerów**:
    - Upewnij się, że użytkownik ma [przypisaną licencję na aplikację Teams](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses).
    - Upewnij się, że użytkownikowi przypisano [pakiet telefoniczny](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page).
    - Udostępnij użytkownikom usługę [Enterprise Voice](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail).

- **Rozwiązywanie problemów z logowaniem się w usłudze Teams**: najpierw sprawdź, czy [usługa Microsoft Teams jest dostępna](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth). Następnie sprawdź, czy pojawiają się znane kody błędów i zapoznaj się z artykułem [Dlaczego mam problem z logowaniem do aplikacji Microsoft Teams](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f)?. Konieczne może być również zapoznanie się z artykułem [Modele uwierzytelniania i tożsamości w aplikacji Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication).
