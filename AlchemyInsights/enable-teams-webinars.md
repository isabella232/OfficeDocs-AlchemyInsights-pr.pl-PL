---
title: Włączanie Teams seminariów w sieci Web
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793783"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="dcf93-102">Włączanie Teams seminariów w sieci Web</span><span class="sxs-lookup"><span data-stu-id="dcf93-102">Enable Teams Webinars</span></span>

<span data-ttu-id="dcf93-103">Seminaria internetowe są domyślnie włączone.</span><span class="sxs-lookup"><span data-stu-id="dcf93-103">Webinars are enabled by default.</span></span> <span data-ttu-id="dcf93-104">Możesz zarządzać tym, kto może planować i rejestrować się w internetowych Teams internetowych, używając Teams programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="dcf93-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="dcf93-105">Wszyscy użytkownicy, którzy mogą utworzyć spotkanie, mogą również utworzyć spotkanie w seminarium w sieci Web.</span><span class="sxs-lookup"><span data-stu-id="dcf93-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="dcf93-106">Jeśli chcesz zarządzać tym, kto może planować seminaria Teams w sieci Web, użyj funkcji *AllowMeetingRegistration.*</span><span class="sxs-lookup"><span data-stu-id="dcf93-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="dcf93-107">Domyślnie funkcja *WhoCanRegister jest* włączona i jest ustawiona na wartość **Wszyscy.**</span><span class="sxs-lookup"><span data-stu-id="dcf93-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="dcf93-108">Jeśli chcesz wyłączyć rejestrację spotkania, ustaw dla ustawienia *AllowMeetingRegistration wartość* **False.**</span><span class="sxs-lookup"><span data-stu-id="dcf93-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="dcf93-109">Aby zmienić te ustawienia, należy zainstalować program [Teams PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="dcf93-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="dcf93-110">Ponadto zasady spotkań są wymuszane w internetowych Teams internetowych.</span><span class="sxs-lookup"><span data-stu-id="dcf93-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="dcf93-111">Jeśli na przykład w ustawieniach spotkania wyłączysz dołączanie anonimowe, użytkownicy anonimowi nie mogą dołączać do seminariów internetowych.</span><span class="sxs-lookup"><span data-stu-id="dcf93-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="dcf93-112">Aby dowiedzieć się więcej o konfigurowaniu osób, które mogą rejestrować się w seminariach internetowych, zobacz Konfigurowanie osób, które mogą rejestrować się w [seminariach internetowych.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="dcf93-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="dcf93-113">Aby uzyskać więcej informacji o ustawieniach list Microsoft, zobacz [Ustawienia sterowania dla list Microsoft.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="dcf93-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>