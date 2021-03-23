---
title: Konfigurowanie punktu połączenia usługi (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037295"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="3f83d-102">Konfigurowanie punktu połączenia usługi (SCP)</span><span class="sxs-lookup"><span data-stu-id="3f83d-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="3f83d-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="3f83d-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="3f83d-104">**Przyczyna:** Nie można odczytać obiektu SCP i pobrać informacji o dzierżawie usługi Azure AD</span><span class="sxs-lookup"><span data-stu-id="3f83d-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="3f83d-105">**Rozwiązanie:** zobacz sekcję [Konfigurowanie punktu połączenia usługi.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="3f83d-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="3f83d-106">**Plan działań**</span><span class="sxs-lookup"><span data-stu-id="3f83d-106">**Action plan**</span></span>

- <span data-ttu-id="3f83d-107">Sprawdź, czy urządzenie otrzymało regułę zasad grupy dla kontrolowanej weryfikacji.</span><span class="sxs-lookup"><span data-stu-id="3f83d-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="3f83d-108">Upewnij się, że klucz rejestru został utworzony przez urząd zasad grupy.</span><span class="sxs-lookup"><span data-stu-id="3f83d-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="3f83d-109">Upewnij się, że masz 2 klucze utworzone przy użyciu identyfikatora katalogu i domeny onmicrosoft.</span><span class="sxs-lookup"><span data-stu-id="3f83d-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="3f83d-110">**Konfigurowanie ustawienia rejestru po stronie klienta dla ustawienia SCP**</span><span class="sxs-lookup"><span data-stu-id="3f83d-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="3f83d-111">Użyj poniższego przykładu, aby utworzyć obiekt zasady grupy (GPO) w celu wdrożenia ustawienia rejestru, które konfiguruje wpis SCP w rejestrze urządzeń.</span><span class="sxs-lookup"><span data-stu-id="3f83d-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="3f83d-112">Otwórz konsolę zasady grupy zarządzania i utwórz nowy magazyn zasad grupy w swojej domenie.</span><span class="sxs-lookup"><span data-stu-id="3f83d-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="3f83d-113">Podaj nazwę nowo utworzonego klienta (na przykład ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="3f83d-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="3f83d-114">Przeedytuj wpis zasad grupy i znajdź następującą ścieżkę: Konfiguracja **komputera > Preferencje > Windows > Rejestru.**</span><span class="sxs-lookup"><span data-stu-id="3f83d-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="3f83d-115">Kliknij prawym przyciskiem myszy **pozycję Rejestr i** wybierz > element **rejestru.**</span><span class="sxs-lookup"><span data-stu-id="3f83d-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="3f83d-116">Na **karcie Ogólne** skonfiguruj następujące opcje:</span><span class="sxs-lookup"><span data-stu-id="3f83d-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="3f83d-117">**Akcja:** Aktualizacja</span><span class="sxs-lookup"><span data-stu-id="3f83d-117">**Action**: Update</span></span>
    
- <span data-ttu-id="3f83d-118">**Gałąź:** HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="3f83d-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="3f83d-119">**Ścieżka klucza:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="3f83d-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="3f83d-120">**Nazwa wartości:** TenantId</span><span class="sxs-lookup"><span data-stu-id="3f83d-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="3f83d-121">**Typ wartości:** REG_SZ</span><span class="sxs-lookup"><span data-stu-id="3f83d-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="3f83d-122">**Dane wartości:** Identyfikator GUID lub identyfikator katalogu wystąpienia usługi Azure AD (tę wartość można znaleźć w portalu Azure Portal > właściwości usługi **Azure Active Directory > właściwości > katalogu)**</span><span class="sxs-lookup"><span data-stu-id="3f83d-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="3f83d-123">Kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="3f83d-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="3f83d-124">Kliknij prawym przyciskiem myszy **pozycję Rejestr i** wybierz > element **rejestru.**</span><span class="sxs-lookup"><span data-stu-id="3f83d-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="3f83d-125">Na **karcie Ogólne** skonfiguruj następujące opcje:</span><span class="sxs-lookup"><span data-stu-id="3f83d-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="3f83d-126">**Akcja:** Aktualizacja</span><span class="sxs-lookup"><span data-stu-id="3f83d-126">**Action**: Update</span></span>
    
- <span data-ttu-id="3f83d-127">**Gałąź:** HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="3f83d-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="3f83d-128">**Ścieżka klucza:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="3f83d-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="3f83d-129">**Nazwa wartości:** TenantName</span><span class="sxs-lookup"><span data-stu-id="3f83d-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="3f83d-130">**Typ wartości:** REG_SZ</span><span class="sxs-lookup"><span data-stu-id="3f83d-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="3f83d-131">**Dane wartości:** zweryfikowana nazwa domeny, jeśli korzystasz ze środowiska feder finansowego, takiego jak usługi AD FS.</span><span class="sxs-lookup"><span data-stu-id="3f83d-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="3f83d-132">Zweryfikowana nazwa domeny lub onmicrosoft.com domeny (na przykład contoso.onmicrosoft.com, jeśli korzystasz ze środowiska zarządzanego)</span><span class="sxs-lookup"><span data-stu-id="3f83d-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="3f83d-133">Kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="3f83d-133">Click **OK**.</span></span>

7. <span data-ttu-id="3f83d-134">Zamknij edytor nowo utworzonego edytora zasad grupy.</span><span class="sxs-lookup"><span data-stu-id="3f83d-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="3f83d-135">Połącz nowo utworzony zestaw zasad grupy z żądaną nazwą użytkownika zawierającą komputery przyłączone do domeny, które należą do twojej populacji kontrolowanego rzutowania.</span><span class="sxs-lookup"><span data-stu-id="3f83d-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="3f83d-136">Aby uzyskać więcej informacji, zobacz Kontrolowane sprawdzanie poprawności hybrydowego dołączania do [usługi Azure AD — usługa Azure AD | Dokumenty Microsoft i](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) rozwiązywanie problemów dotyczących urządzeń przyłącznych do hybrydowej  [usługi Azure Active Directory | Dokumenty Microsoft](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="3f83d-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









