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
# <a name="enable-teams-webinars"></a>Włączanie Teams seminariów w sieci Web

Seminaria internetowe są domyślnie włączone. Możesz zarządzać tym, kto może planować i rejestrować się w internetowych Teams internetowych, używając Teams programu PowerShell.

- Wszyscy użytkownicy, którzy mogą utworzyć spotkanie, mogą również utworzyć spotkanie w seminarium w sieci Web. Jeśli chcesz zarządzać tym, kto może planować seminaria Teams w sieci Web, użyj funkcji *AllowMeetingRegistration.* 
- Domyślnie funkcja *WhoCanRegister jest* włączona i jest ustawiona na wartość **Wszyscy.** Jeśli chcesz wyłączyć rejestrację spotkania, ustaw dla ustawienia *AllowMeetingRegistration wartość* **False.**

Aby zmienić te ustawienia, należy zainstalować program [Teams PowerShell.](/microsoftteams/teams-powershell-install) Ponadto zasady spotkań są wymuszane w internetowych Teams internetowych. Jeśli na przykład w ustawieniach spotkania wyłączysz dołączanie anonimowe, użytkownicy anonimowi nie mogą dołączać do seminariów internetowych.

Aby dowiedzieć się więcej o konfigurowaniu osób, które mogą rejestrować się w seminariach internetowych, zobacz Konfigurowanie osób, które mogą rejestrować się w [seminariach internetowych.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Aby uzyskać więcej informacji o ustawieniach list Microsoft, zobacz [Ustawienia sterowania dla list Microsoft.](/sharepoint/control-lists)