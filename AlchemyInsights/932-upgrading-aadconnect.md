---
title: 932 AADConnect uaktualniania
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8038d5ef768d6ee228db7d038ad71d926f4047f3
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29937954"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="d460f-102">Podłącz uaktualnienia Azure AD</span><span class="sxs-lookup"><span data-stu-id="d460f-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="d460f-p101">Domyślnie automatyczne uaktualnienie jest włączona dla Azure AD Connect, które pomaga zapewnić, że korzystasz z najnowszej wersji. Aby sprawdzić ustawienia automatycznego uaktualniania, należy użyć polecenia cmdlet **Get-ADSyncAutoUpgrade** w programie AD PowerShell Azure. Polecenia cmdlet zwróci się jedną z następujących wartości:</span><span class="sxs-lookup"><span data-stu-id="d460f-p101">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version. To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell. The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="d460f-106">**Włączone**: automatyczne uaktualnienie jest włączona.</span><span class="sxs-lookup"><span data-stu-id="d460f-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="d460f-107">**Wyłączone**: automatyczne uaktualnienie jest wyłączane.</span><span class="sxs-lookup"><span data-stu-id="d460f-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="d460f-p102">**Zawieszone**: system nie jest już uprawniony do otrzymania automatycznych uaktualnień. Nie można skonfigurować tej wartości; jest on ustawiony przez system.</span><span class="sxs-lookup"><span data-stu-id="d460f-p102">**Suspended**: The system is no longer eligible to receive automatic upgrades. You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="d460f-110">Aby uzyskać więcej informacji zobacz temat [automatyczne uaktualnienie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="d460f-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="d460f-111">Aby pobrać najnowszą wersję programu Azure AD Connect, przejdź do [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="d460f-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

