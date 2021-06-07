---
title: Zarządzanie rejestracją w seminariach internetowych
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793912"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="8cbdf-102">Zarządzanie rejestracją w seminariach internetowych</span><span class="sxs-lookup"><span data-stu-id="8cbdf-102">Manage webinar registration</span></span>

<span data-ttu-id="8cbdf-103">Możesz zarządzać tym, kto może rejestrować się w seminariach internetowych Teams internetowych, używając Teams programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8cbdf-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="8cbdf-104">Aby zainstalować Teams PowerShell, zobacz Teams [PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="8cbdf-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="8cbdf-105">Domyślnie funkcja *WhoCanRegister jest* włączona i ustawiona na **wartość EveryoneInCompany.**</span><span class="sxs-lookup"><span data-stu-id="8cbdf-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="8cbdf-106">Aby zezwolić wszystkim, w tym użytkownikom anonimowym, na rejestrację, musisz ustawić zasady spotkania na **Wszyscy** przy użyciu polecenia programu PowerShell:</span><span class="sxs-lookup"><span data-stu-id="8cbdf-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="8cbdf-107">**Uwaga:** Jeśli w ustawieniach spotkania jest wyłączone dołączanie anonimowe, użytkownicy anonimowi nie mogą dołączać do seminariów internetowych.</span><span class="sxs-lookup"><span data-stu-id="8cbdf-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="8cbdf-108">Aby dowiedzieć się więcej i włączyć to ustawienie, zobacz [Zarządzanie ustawieniami spotkania w programie Microsoft Teams.](/microsoftteams/meeting-settings-in-teams)</span><span class="sxs-lookup"><span data-stu-id="8cbdf-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="8cbdf-109">Jeśli chcesz wyłączyć rejestrację spotkania, ustaw dla ustawienia *AllowMeetingRegistration wartość* **False.**</span><span class="sxs-lookup"><span data-stu-id="8cbdf-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="8cbdf-110">Aby dowiedzieć się więcej o konfigurowaniu osób, które mogą rejestrować się w seminariach internetowych, zobacz Konfigurowanie osób, które mogą rejestrować się w [seminariach internetowych.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="8cbdf-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="8cbdf-111">Aby uzyskać więcej informacji o ustawieniach list Microsoft, zobacz [Ustawienia sterowania dla list Microsoft.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="8cbdf-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
