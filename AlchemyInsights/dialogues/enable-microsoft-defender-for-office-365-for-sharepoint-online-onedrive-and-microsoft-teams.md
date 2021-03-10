---
title: Włączanie usługi Microsoft Defender dla usługi Office 365 dla usług SharePoint Online, OneDrive i Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695649"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="4e138-102">Włączanie usługi Microsoft Defender dla usługi Office 365 dla usług SharePoint Online, OneDrive i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="4e138-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="4e138-103">Używając poświadczeń administratora globalnego lub administratora zabezpieczeń, zaloguj się do Centrum zabezpieczeń i zgodności usługi [Office 365.](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="4e138-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="4e138-104">Wybierz **pozycję Zarządzanie zagrożeniami** w okienku po lewej stronie, a następnie wybierz **pozycję Załączniki**  >  [bezpieczne zasad.](https://protection.office.com/safeattachment)</span><span class="sxs-lookup"><span data-stu-id="4e138-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="4e138-105">Wybierz **pozycję Włącz usługę Microsoft Defender dla usługi Office 365 dla programu SharePoint, usługi OneDrive** i aplikacji Microsoft Teams, a następnie wybierz pozycję **Zapisz.**</span><span class="sxs-lookup"><span data-stu-id="4e138-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="4e138-106">Jako administrator globalny lub administrator usługi SharePoint Online uruchom następujące polecenie cmdlet programu PowerShell z parametrem **DisallowInfectedFileDownload** ustawionym na *wartość True*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="4e138-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="4e138-107">Konfigurowanie alertów dotyczących wykrytych plików</span><span class="sxs-lookup"><span data-stu-id="4e138-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="4e138-108">Aby uzyskać więcej informacji, zobacz [Microsoft Defender for Office 365 for SharePoint, OneDrive i Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)</span><span class="sxs-lookup"><span data-stu-id="4e138-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
