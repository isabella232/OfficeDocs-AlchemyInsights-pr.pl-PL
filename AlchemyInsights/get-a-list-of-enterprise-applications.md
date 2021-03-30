---
title: Uzyskiwanie listy aplikacji dla przedsiębiorstw
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
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404925"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="105c3-102">Uzyskiwanie listy aplikacji dla przedsiębiorstw</span><span class="sxs-lookup"><span data-stu-id="105c3-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="105c3-103">Aby uzyskać listę aplikacji **przedsiębiorstwa** (wszystkie aplikacje lub filtrowane według nazwy wyświetlanej, identyfikatora, identyfikatorów URI itp.) za pomocą polecenia programu PowerShell, zobacz [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)</span><span class="sxs-lookup"><span data-stu-id="105c3-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="105c3-104">Aby uzyskać listę obiektów głównych usługi (wszystkie obiekty lub obiekty filtrowane według identyfikatora) za pomocą polecenia programu PowerShell, zobacz [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span><span class="sxs-lookup"><span data-stu-id="105c3-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="105c3-105">Jeśli chcesz uzyskać listę aplikacji skonfigurowanych w języku **SAML, możesz użyć następujących skryptów programu PowerShell:**</span><span class="sxs-lookup"><span data-stu-id="105c3-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="105c3-106">Każda aplikacja, zarówno aplikacja OAuth, jak i aplikacja SAML (zarówno aplikacja galerii, jak i aplikacje niesklasywne), będzie mieć dwa obiekty utworzone w UAD podczas ich rejestracji.</span><span class="sxs-lookup"><span data-stu-id="105c3-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="105c3-107">Jeden z nich nosi nazwę Application Object, a drugi to obiekt Service Principal (Podmiot zabezpieczeń usługi).</span><span class="sxs-lookup"><span data-stu-id="105c3-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="105c3-108">Po zrzucie właściwości obiektu podmiotu zabezpieczeń usługi przy użyciu programu PowerShell można się dowiedzieć, że każda aplikacja ma skojarzoną z nią określoną liczbę tagów, na przykład:</span><span class="sxs-lookup"><span data-stu-id="105c3-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="105c3-109">Aplikacje OAuth będą miały tag o nazwie "**WindowsAzureActiveDirectoryIntegratedApp"**</span><span class="sxs-lookup"><span data-stu-id="105c3-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="105c3-110">Aplikacja Gallery SAML miałaby tag o nazwie "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1"**</span><span class="sxs-lookup"><span data-stu-id="105c3-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="105c3-111">Aplikacje SAML bez galerii będą miały tag o nazwie "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication"**</span><span class="sxs-lookup"><span data-stu-id="105c3-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="105c3-112">Dlatego można używać tych tagów i dowiedzieć się, jakiego rodzaju są to aplikacje.</span><span class="sxs-lookup"><span data-stu-id="105c3-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="105c3-113">Tag "**WindowsAzureActiveDirectoryIntegratedApp**" jest wspólny dla wszystkich typów aplikacji.</span><span class="sxs-lookup"><span data-stu-id="105c3-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="105c3-114">Za pomocą następującego fragmentu można wyświetlić listę wszystkich aplikacji SAML (zarówno galerii, jak i bez galerii):</span><span class="sxs-lookup"><span data-stu-id="105c3-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="105c3-115">Aby uzyskać więcej informacji, zobacz Identyfikowanie aplikacji z obsługą [saml w usłudze Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)</span><span class="sxs-lookup"><span data-stu-id="105c3-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="105c3-116">**Znajdowanie i lista tylko aplikacji sieci Web:** Użyj poniższego polecenia, aby pobrać wszystkie aplikacje usługi Azure AD o typie aplikacji "Aplikacja sieci Web/interfejs API"</span><span class="sxs-lookup"><span data-stu-id="105c3-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="105c3-117">Get-AzureADApplication —Wszystkie:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="105c3-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="105c3-118">**Znajdź i przygotuj listę samych aplikacji natywnych:** Uruchom następujące polecenie, aby pobrać wszystkie aplikacje natywnego klienta (stacjonarnego/przenośnego).</span><span class="sxs-lookup"><span data-stu-id="105c3-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="105c3-119">Get-AzureADApplication —Wszystkie:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="105c3-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="105c3-120">**Eksportuj wszystkie zarejestrowane szczegóły aplikacji usługi Azure AD** do pliku CSV: poniższe polecenie eksportuje wszystkie aplikacje usługi Azure AD ze szczegółami wymaganymi do pliku csv:</span><span class="sxs-lookup"><span data-stu-id="105c3-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="105c3-121">Get-AzureADApplication —Wszystkie:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="105c3-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="105c3-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="105c3-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="105c3-123">**Musisz wyeksportować listę nieużywanych aplikacji platformy Azure** — Raport inspekcji</span><span class="sxs-lookup"><span data-stu-id="105c3-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="105c3-124">Usługa Azure AD może wyświetlać dzienniki aplikacji tylko przez 30 dni pod warunkiem, że masz licencję usługi Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="105c3-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="105c3-125">Dostępne są dwie opcje przechowywania danych przez dłużej niż 30 dni.</span><span class="sxs-lookup"><span data-stu-id="105c3-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="105c3-126">Za pomocą interfejsów [API raportowania](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) usługi Azure AD można programowo pobierać dane i przechowywać je w bazie danych.</span><span class="sxs-lookup"><span data-stu-id="105c3-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="105c3-127">Możesz również zintegrować dzienniki inspekcji z systemem SIEM innej firmy.</span><span class="sxs-lookup"><span data-stu-id="105c3-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="105c3-128">Możesz również pobrać listę aplikacji dla wszystkich aplikacji i aplikacji należących do usługi Azure Active Directory>rejestracja aplikacji>Pobierz>Wszystkie aplikacje/Aplikacje posiadane.</span><span class="sxs-lookup"><span data-stu-id="105c3-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="105c3-129">Aby uzyskać listę aplikacji za pomocą programu MS Graph, zobacz Aplikacje listy [— Microsoft Graph 1.0](https://docs.microsoft.com/graph/api/application-list) i typ zasobu aplikacji [— Microsoft Graph 1.0.](https://docs.microsoft.com/graph/api/resources/application)</span><span class="sxs-lookup"><span data-stu-id="105c3-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
