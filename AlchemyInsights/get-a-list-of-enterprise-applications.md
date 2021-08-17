---
title: Uzyskiwanie listy aplikacji Enterprise aplikacji
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116738"
---
# <a name="get-a-list-of-enterprise-applications"></a>Uzyskiwanie listy aplikacji Enterprise aplikacji

1. Aby uzyskać listę aplikacji **przedsiębiorstwa** (wszystkie aplikacje lub filtrowane według nazwy wyświetlanej, identyfikatora, identyfikatorów URI itp.) za pomocą polecenia programu PowerShell, zobacz [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)
2. Aby uzyskać listę obiektów głównych usługi (wszystkie obiekty lub obiekty filtrowane według identyfikatora) za pomocą polecenia programu PowerShell, zobacz [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).
3. Jeśli chcesz uzyskać listę aplikacji skonfigurowanych w języku **SAML, możesz użyć następujących skryptów programu PowerShell:**

    Każda aplikacja, zarówno aplikacja OAuth, jak i aplikacja SAML (zarówno aplikacja galerii, jak i aplikacje niesklasywne), będzie mieć dwa obiekty utworzone w UAD podczas ich rejestracji. Jeden z nich nosi nazwę Application Object, a drugi to obiekt Service Principal (Podmiot zabezpieczeń usługi). Po zrzucie właściwości obiektu podmiotu zabezpieczeń usługi przy użyciu programu PowerShell można się dowiedzieć, że każda aplikacja ma skojarzoną z nią określoną liczbę tagów, na przykład:

    - Aplikacje OAuth będą miały tag o nazwie "**WindowsAzureActiveDirectoryIntegratedApp"**
    - Aplikacja Gallery SAML miałaby tag o nazwie "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1"**
    - Aplikacje SAML bez galerii będą miały tag o nazwie "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication"**

    Dlatego można używać tych tagów i dowiedzieć się, jakiego rodzaju są to aplikacje. Tag "**WindowsAzureActiveDirectoryIntegratedApp**" jest wspólny dla wszystkich typów aplikacji. Za pomocą następującego fragmentu można wyświetlić listę wszystkich aplikacji SAML (zarówno galerii, jak i bez galerii):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Aby uzyskać więcej informacji, zobacz Identyfikowanie aplikacji z obsługą [saml w usłudze Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **Znajdowanie i lista tylko aplikacji sieci Web:** Użyj poniższego polecenia, aby pobrać wszystkie aplikacje usługi Azure AD o typie aplikacji "Aplikacja sieci Web/interfejs API"

    Get-AzureADApplication —Wszystkie:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Znajdź i przygotuj listę samych aplikacji natywnych:** Uruchom następujące polecenie, aby pobrać wszystkie aplikacje natywnego klienta (stacjonarnego/przenośnego).

    Get-AzureADApplication —Wszystkie:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Eksportuj wszystkie zarejestrowane szczegóły aplikacji usługi Azure AD** do pliku CSV: poniższe polecenie eksportuje wszystkie aplikacje usługi Azure AD ze szczegółami wymaganymi do pliku csv:

    - Get-AzureADApplication —Wszystkie:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Musisz wyeksportować listę nieużywanych aplikacji platformy Azure** — Raport inspekcji

    Dzienniki aplikacji w usłudze Azure AD mogą być wyświetlane tylko przez 30 dni pod warunkiem Azure AD — wersja Premium licencji.
    Dostępne są dwie opcje przechowywania danych przez dłużej niż 30 dni. Za pomocą interfejsów [API raportowania](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) usługi Azure AD można programowo pobierać dane i przechowywać je w bazie danych. Możesz również zintegrować dzienniki inspekcji z systemem SIEM innej firmy.

    Możesz również pobrać listę aplikacji dla wszystkich aplikacji i aplikacji należących do usługi Azure Active Directory>rejestracja aplikacji>Pobierz>Wszystkie aplikacje/Aplikacje posiadane.

    Aby uzyskać listę aplikacji za pośrednictwem programu Microsoft Graph, zobacz Aplikacje listy — Microsoft Graph w wersji [1.0](https://docs.microsoft.com/graph/api/application-list) i typ zasobu aplikacji [— Microsoft Graph w wersji 1.0.](https://docs.microsoft.com/graph/api/resources/application)
