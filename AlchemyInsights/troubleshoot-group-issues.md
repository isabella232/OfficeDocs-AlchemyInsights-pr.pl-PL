---
title: Rozwiązywanie problemów z grupą
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/18/2021
ms.locfileid: "50714050"
---
# <a name="troubleshoot-group-issues"></a>Rozwiązywanie problemów z grupą

**Muszę przypisać grupę do roli usługi Azure AD**

Aby przypisać grupę usługi Azure Active Directory (AD) do roli usługi Azure AD, wykonaj następujące czynności:

1. Tworzenie nowej grupy — aby utworzyć nową grupę:

    a. Zaloguj się do centrum administracyjnego usługi Azure AD z uprawnieniami administratora roli lub administratora globalnego. 
    b. Wybierz pozycję Grupy > usługi Azure Active Directory > Grupy > Nowa grupa. 
    c. Utwórz grupę.

2. Przypisz rolę do grupy podczas jej tworzenia lub po jej utworzeniu.

    a. Aby przypisać rolę do grupy w momencie tworzenia grupy, włącz przełącznik ról usługi Azure AD, które można przypisać do grupy, i utwórz grupę.
    b. Aby przypisać rolę do grupy po jej utworzeniu, przejdź do karty Przypisane role dla nowo utworzonej grupy i przypisz tę rolę do grupy.

**Muszę zarządzać członkostwem w grupie przypisanej do roli usługi Azure AD**

1. Aby uniemożliwić podwyższenie uprawnień, domyślnie tylko administrator roli z uprawnieniami i administrator globalny mogą modyfikować członkostwo w grupie przypisanej do roli. Mogą jednak przypisać właściciela do takiej grupy i delegować to zadanie. Aby uzyskać więcej informacji, zobacz: Zarządzanie przypisaniami ról w usłudze Azure Active Directory za pomocą grup w [chmurze.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)
2. Aby uzyskać typowe pytania i porady dotyczące rozwiązywania problemów dotyczące przypisywania ról do grup w usłudze Azure AD, zobacz Rozwiązywanie problemów z rolami przypisanymi [do grup w chmurze.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)

**Grupy dynamiczne**

1. Jeśli nie możesz znaleźć wbudowanych atrybutów użytkownika, upewnij się, że ten atrybut znajduje się na liście obsługiwanych właściwości.
2. Jeśli szukasz wbudowanych atrybutów urządzenia, upewnij się, że ten atrybut znajduje się na liście atrybutów urządzenia. 
3. Oprócz wbudowanych atrybutów użytkownika i urządzenia można także używać [atrybutów rozszerzenia.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties) Po zsynchronizowaniu atrybutów rozszerzenia z lokalnej usługi Windows Server AD lub z połączonej aplikacji SaaS atrybuty powinny być widoczne na liście rozwijanej konstruktora reguł. Niestandardową nazwę atrybutu można znaleźć w katalogu przez zapytanie dotyczące atrybutu użytkownika przy użyciu programu PowerShell i wyszukanie nazwy tego atrybutu. Mogą one być także używane podczas konstruowania reguł w składni reguły.
4. Upewnij się, że dzierżawa ma odpowiednią licencję. Grupy dynamiczne wymagają, aby dzierżawa posiadała licencję Azure AD P1 Premium. Lista planów licencyjnych usługi Azure AD jest dostępna [tutaj.](https://azure.microsoft.com/pricing/details/active-directory/) Tutaj można uzyskać dostęp do planów licencjonowania Enterprise Mobility + [Security.](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)
5. Upewnij się, że rolę użytkownika tworzącego grupę dynamiczną pełni administrator globalny, administrator intune, administrator grupy lub administrator użytkownika.
6. Należy zezwolić grupie na jej wypełnienie. W zależności od rozmiaru dzierżawy wypełnianie grupy po raz pierwszy lub po zmianie reguły może potrwać do 24 godzin.
7. Aby uzyskać więcej informacji, zobacz Tworzenie reguł opartych na [atrybutach dla dynamicznego członkostwa w grupach.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership)

**Muszę usunąć grupę**

1. Grupy można usuwać z katalogu za pomocą polecenia cmdlet Remove-AzureADGroup w module powershell usługi Azure AD.
2. Przed podjęciem próby usunięcia zsynchronizowanej grupy w usłudze Azure AD upewnij się, że usunięto wszystkie przypisane licencje, aby uniknąć błędów.
3. Aby uzyskać więcej informacji na temat usuwania grup, zobacz [Usuwanie grupy z przypisaną licencją.](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license)

**Muszę przywrócić usuniętą grupę**

1. Jeśli grupa usługi Office 365 zostanie usunięta, można ją przywrócić tylko do 30 dni przed trwałym usunięciem. Po trwałym usunięciu grupy nie będzie już można jej przywrócić. Dowiedz się więcej o przywracaniu grup [tutaj.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)
2. Ta funkcja nie jest obsługiwana w przypadku grup zabezpieczeń ani grup dystrybucyjnych.
3. Upewnij się, że masz upoważnienie do przywracania grupy usługi Office 365. Administratorzy globalni, administratorzy grup, administratorzy kont użytkowników, administratorzy usługi Intune, pomoc techniczna dla partnerów (warstwa 1 lub warstwa 2) oraz właściciel grupy mogą przywrócić grupę.
4. Po usunięciu i przywróceniu grupy dynamicznej jest ona widziana jako nowa grupa i ponownie wypełniana zgodnie z regułą. Ten proces może potrwać do 24 godzin.
5. Aby uzyskać więcej informacji na temat przywracania usuniętej grupy, zobacz Przywracanie usuniętej grupy [usługi Office 365 w usłudze Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Konfiguracja zasad wygasania grup**

1. Ta funkcja jest obsługiwana tylko w przypadku grup usługi Office 365 i nie jest obsługiwana w przypadku grup zabezpieczeń i grup dystrybucyjnych.
2. Do konfigurowania i używania zasad wygasania grup usługi Office 365 jest wymagana licencja usługi Azure AD Premium.
3. Obecnie dla grup usługi Office 365 w dzierżawie można skonfigurować tylko jedną z zasad wygasania.
4. Tylko administratorzy globalni, administratorzy grup, administratorzy użytkowników i właściciel grupy mogą odnowić grupę.
5. Jeśli grupa usługi Office 365 wygasła, zostanie usunięta i można ją przywrócić tylko do 30 dni przed trwałym usunięciem. Po trwałym usunięciu grupy nie będzie już można jej przywrócić. Dowiedz się więcej o przywracaniu grup [tutaj.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Automatyczne odnawianie oparte na działaniach**

Działania użytkowników z programów SharePoint, Outlook i Teams mogą wyzwalać automatyczne odnawianie grup. Działania są sprawdzane na 35 dni przed wygaśnięciem grupy. Jeśli w bieżącym cyklu życia grupy istnieją działania, grupa zostanie automatycznie odnowiona i powiadomienia e-mail nie zostaną wysłane do właścicieli grupy.

**Chronometraż powiadomień o wygasłych grupach**

1. Powiadomienia e-mail są wysyłane do właścicieli grupy usługi Office 365 na 30 dni, 15 dni i 1 dzień przed wygaśnięciem grupy.
2. Po pierwszym skonfigurowaniu wygasania wszystkie grupy starsze niż interwał wygasania są ustawiane na 35 dni do wygaśnięcia.
3. Data wygaśnięcia grupy jest obliczana na podstawie daty odnowienia grupy, a nie na podstawie daty aktualizacji zasad. Jeśli zasady wygasania zostaną zaktualizowane, data wygaśnięcia nie zmieni się.
4. Aby uzyskać więcej [informacji,](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) zobacz zasady wygasania grupy i wiadomości e-mail dotyczące odnawiania oraz Przywracanie usuniętej grupy usługi [Office 365 w usłudze Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Uprawnienie do tworzenia grupy**

Upewnij się, że masz upoważnienie do tworzenia nowej grupy. Administratorzy globalni mogą wyłączyć możliwość tworzenia grup w Portalu Azure lub Panelu dostępu. Administrator może tworzyć nową grupę lub udzielać odpowiednich uprawnień.

1. [Tworzenie nowej grupy i dodawanie członków w portalu Azure Portal](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Tworzenie grup w programie PowerShell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Wyłączanie możliwości tworzenia grup w programie PowerShell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Zarządzanie tym, kto może tworzyć grupy w usłudze Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Wyłączanie powitania usługi Office 365 za pomocą programu PowerShell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Role administracyjne usługi Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Zarządzanie uprawnieniami do tworzenia grup**

1. Administratorzy globalni mogą zarządzać uprawnieniami do tworzenia grup zabezpieczeń lub grupami usługi Office 365 utworzonymi w Portalu Azure lub Panelu dostępu, ustawiając ustawienie Użytkownicy mogą tworzyć grupy zabezpieczeń w portalach **Azure** lub użytkownicy mogą tworzyć grupy usługi **Office 365** w ustawieniach portalu Azure w grupie Wszystkie grupy > Ogólne **(Ustawienia).**
2. Jeśli masz licencję Usługi Azure AD P1 Premium, możesz też ograniczyć możliwość tworzenia grup w celu wybrania grupy użytkowników.

**Wyłączanie powiadomień powitalnych dla nowych członków grupy usługi Office 365**

Powiadomienie powitane wysyłane do użytkowników dodanych do grup usługi Office 365 można wyłączyć, ustawiając wartość `UnifiedGroupWelcomeMessageEnabled` **Fałsz** w programie PowerShell. Tutaj znajdziesz informacje o tym [ustawieniu.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)













