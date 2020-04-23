---
title: 932 Modernizacja AAdConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766503"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="f1d85-102">Uaktualnianie usługi Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="f1d85-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="f1d85-103">Domyślnie automatyczne uaktualnianie jest włączone dla usługi Azure AD Connect, co pomaga upewnić się, że korzystasz z najnowszej wersji.</span><span class="sxs-lookup"><span data-stu-id="f1d85-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="f1d85-104">Aby sprawdzić ustawienia automatycznego uaktualniania, użyj polecenia cmdlet **Get-ADSyncAutoUpgrade** w programie Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f1d85-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="f1d85-105">Polecenie cmdlet zwróci jedną z następujących wartości:</span><span class="sxs-lookup"><span data-stu-id="f1d85-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="f1d85-106">**Włączone:** Automatyczne uaktualnianie jest włączone.</span><span class="sxs-lookup"><span data-stu-id="f1d85-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="f1d85-107">**Wyłączone**: Automatyczne uaktualnianie jest wyłączone.</span><span class="sxs-lookup"><span data-stu-id="f1d85-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="f1d85-108">**Zawieszone**: System nie kwalifikuje się już do automatycznych uaktualnień.</span><span class="sxs-lookup"><span data-stu-id="f1d85-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="f1d85-109">Nie można skonfigurować tej wartości; jest ustawiony przez system.</span><span class="sxs-lookup"><span data-stu-id="f1d85-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="f1d85-110">Aby uzyskać więcej informacji, zobacz [Automatyczne uaktualnianie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="f1d85-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="f1d85-111">Aby pobrać najnowszą wersję usługi Azure [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)AD Connect, przejdź do .</span><span class="sxs-lookup"><span data-stu-id="f1d85-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
