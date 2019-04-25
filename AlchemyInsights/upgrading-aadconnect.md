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
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389733"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="aaf82-102">Podłącz uaktualnienia Azure AD</span><span class="sxs-lookup"><span data-stu-id="aaf82-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="aaf82-103">Domyślnie automatyczne uaktualnienie jest włączona dla Azure AD Connect, które pomaga zapewnić, że korzystasz z najnowszej wersji.</span><span class="sxs-lookup"><span data-stu-id="aaf82-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="aaf82-104">Aby sprawdzić ustawienia automatycznego uaktualniania, należy użyć polecenia cmdlet **Get-ADSyncAutoUpgrade** w programie AD PowerShell Azure.</span><span class="sxs-lookup"><span data-stu-id="aaf82-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="aaf82-105">Polecenia cmdlet zwróci się jedną z następujących wartości:</span><span class="sxs-lookup"><span data-stu-id="aaf82-105">The cmdlet will return one of following values:</span></span> 

- <span data-ttu-id="aaf82-106">**Włączone**: automatyczne uaktualnienie jest włączona.</span><span class="sxs-lookup"><span data-stu-id="aaf82-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="aaf82-107">**Wyłączone**: automatyczne uaktualnienie jest wyłączane.</span><span class="sxs-lookup"><span data-stu-id="aaf82-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="aaf82-108">**Zawieszone**: system nie jest już uprawniony do otrzymania automatycznych uaktualnień.</span><span class="sxs-lookup"><span data-stu-id="aaf82-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="aaf82-109">Nie można skonfigurować tej wartości; jest on ustawiony przez system.</span><span class="sxs-lookup"><span data-stu-id="aaf82-109">You can't configure this value; it's set by the system.</span></span> 

<span data-ttu-id="aaf82-110">Aby uzyskać więcej informacji zobacz temat [automatyczne uaktualnienie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="aaf82-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="aaf82-111">Aby pobrać najnowszą wersję programu Azure AD Connect, przejdź do [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="aaf82-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
