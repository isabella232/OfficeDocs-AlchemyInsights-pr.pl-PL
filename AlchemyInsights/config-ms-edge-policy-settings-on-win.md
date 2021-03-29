---
title: Konfigurowanie ustawień zasad przeglądarki Microsoft Edge w systemie Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003845"
- "9004632"
- "6894"
- "8358"
ms.openlocfilehash: e9bb489b4d8ecd76fd777ade9fb740ecad542900
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402385"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="ab855-102">Konfigurowanie ustawień zasad przeglądarki Microsoft Edge w systemie Windows</span><span class="sxs-lookup"><span data-stu-id="ab855-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="ab855-103">Aby skonfigurować ustawienia zasad i zarządzane aktualizacje dla przeglądarki Microsoft Edge, użyj funkcji obiekty zasady grupy (GPOS).</span><span class="sxs-lookup"><span data-stu-id="ab855-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="ab855-104">Zasady można także zapewniać za pośrednictwem rejestru. byłoby to odpowiednie dla (1) urządzeń z systemem Windows przyłączony do domeny Microsoft Active Directory i (2) wystąpień systemu Windows 10 Pro i Enterprise zarejestrowanych do zarządzania urządzeniami w usłudze Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="ab855-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="ab855-105">Aby skonfigurować program Microsoft Edge przy użyciu gpOs, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="ab855-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="ab855-106">Przejdź do magazynu zasady grupy centralnej w domenie usługi Active Directory lub do folderu szablonów definicji zasad na poszczególnych komputerach zainstaluj wszystkie szablony administracyjne, które dodają reguły i ustawienia dla przeglądarki Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="ab855-106">Go to the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="ab855-107">Skonfiguruj konkretne zasady, które chcesz ustawić.</span><span class="sxs-lookup"><span data-stu-id="ab855-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="ab855-108">Aby dowiedzieć się więcej, zobacz [Konfigurowanie ustawień zasad przeglądarki Microsoft Edge w systemie Windows.](https://go.microsoft.com/fwlink/?linkid=2135024)</span><span class="sxs-lookup"><span data-stu-id="ab855-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
