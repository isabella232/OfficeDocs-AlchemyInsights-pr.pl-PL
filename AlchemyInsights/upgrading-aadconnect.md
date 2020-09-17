---
title: 932 uaktualnianie AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806049"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="a3a6b-102">Uaktualnij usługę Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="a3a6b-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="a3a6b-103">Domyślnie automatyczne uaktualnienie jest włączone dla usługi Azure AD Connect, co zapewnia, że korzystasz z najnowszej wersji.</span><span class="sxs-lookup"><span data-stu-id="a3a6b-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="a3a6b-104">Aby sprawdzić ustawienia uaktualnienia automatycznego, użyj polecenia cmdlet **Get-ADSyncAutoUpgrade** w programie Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a3a6b-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="a3a6b-105">Polecenie cmdlet zwróci dowolną z następujących wartości:</span><span class="sxs-lookup"><span data-stu-id="a3a6b-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="a3a6b-106">**Włączone**: automatyczne uaktualnianie jest włączone.</span><span class="sxs-lookup"><span data-stu-id="a3a6b-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="a3a6b-107">**Wyłączone**: automatyczne uaktualnienie jest wyłączone.</span><span class="sxs-lookup"><span data-stu-id="a3a6b-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="a3a6b-108">**Zawieszone**: system nie kwalifikuje się już do otrzymywania automatycznych uaktualnień.</span><span class="sxs-lookup"><span data-stu-id="a3a6b-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="a3a6b-109">Tej wartości nie można skonfigurować; jest ona ustawiana przez system.</span><span class="sxs-lookup"><span data-stu-id="a3a6b-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="a3a6b-110">Aby uzyskać więcej informacji, zobacz [automatyczne uaktualnianie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="a3a6b-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="a3a6b-111">Aby pobrać najnowszą wersję usługi Azure AD Connect, przejdź do [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="a3a6b-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
