---
title: 401 Nieautoryzowany błąd w SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 6799b2112458a7ab3715c9b63e03c2c7ca3fe6be
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233517"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Nieautoryzowany błąd w SharePoint

Jeśli w programie SharePoint zostanie wyświetlony komunikat o błędzie "(401) Unauthorized" (Nieautoryzowany), może on być związany z wyliżeniem TLS 1.0/1.1. Aby uzyskać więcej informacji, zobacz:

[Przygotowanie do protokołu TLS 1.2 w usłudze Office 365 i usłudze Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

[Błędy uwierzytelniania występują, jeśli klient nie obsługuje protokołu TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

Jeśli użytkownicy mają Windows 7, upewnij się, że sprawdzają pakiety [TLS Cipher Suites](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)w Windows 7.