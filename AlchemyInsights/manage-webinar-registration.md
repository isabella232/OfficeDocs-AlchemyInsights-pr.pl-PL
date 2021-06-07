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
# <a name="manage-webinar-registration"></a>Zarządzanie rejestracją w seminariach internetowych

Możesz zarządzać tym, kto może rejestrować się w seminariach internetowych Teams internetowych, używając Teams programu PowerShell. Aby zainstalować Teams PowerShell, zobacz Teams [PowerShell.](/microsoftteams/teams-powershell-install) 

Domyślnie funkcja *WhoCanRegister jest* włączona i ustawiona na **wartość EveryoneInCompany.** Aby zezwolić wszystkim, w tym użytkownikom anonimowym, na rejestrację, musisz ustawić zasady spotkania na **Wszyscy** przy użyciu polecenia programu PowerShell:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Uwaga:** Jeśli w ustawieniach spotkania jest wyłączone dołączanie anonimowe, użytkownicy anonimowi nie mogą dołączać do seminariów internetowych. Aby dowiedzieć się więcej i włączyć to ustawienie, zobacz [Zarządzanie ustawieniami spotkania w programie Microsoft Teams.](/microsoftteams/meeting-settings-in-teams)

Jeśli chcesz wyłączyć rejestrację spotkania, ustaw dla ustawienia *AllowMeetingRegistration wartość* **False.**

Aby dowiedzieć się więcej o konfigurowaniu osób, które mogą rejestrować się w seminariach internetowych, zobacz Konfigurowanie osób, które mogą rejestrować się w [seminariach internetowych.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Aby uzyskać więcej informacji o ustawieniach list Microsoft, zobacz [Ustawienia sterowania dla list Microsoft.](/sharepoint/control-lists)
