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
ms.openlocfilehash: ac2fe27a8e7b277bfaf18303bf5b792410a1ea6a
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539942"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Nieautoryzowany błąd w SharePoint

Jeśli w programie SharePoint zostanie wyświetlony komunikat o błędzie "(401) Unauthorized" (Nieautoryzowany), może on być związany z wyliżeniem TLS 1.0/1.1. Aby uzyskać więcej informacji, zobacz:

- [Przygotowanie do protokołu TLS 1.2 w usłudze Office 365 i usłudze Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Błędy uwierzytelniania występują, jeśli klient nie obsługuje protokołu TLS 1.2](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Zaktualizuj, aby włączyć protokoły TLS 1.1 i TLS 1.2 jako domyślne protokoły bezpiecznego w WinHTTP w Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Jeśli użytkownicy mają Windows 7, upewnij się, że sprawdzają pakiety [TLS Cipher Suites](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)w Windows 7.