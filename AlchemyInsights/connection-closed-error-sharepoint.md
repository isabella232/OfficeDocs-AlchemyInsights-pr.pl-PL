---
title: Błąd połączenia bazowego został zamknięty w SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 101c0ba90d2bec6b1684fd63645ba2f8f89783ad5bfdf0efe739d31dfd951f66
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044422"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Błąd "Połączenie podstawowe zostało zamknięte" w SharePoint

Jeśli w programie SharePoint jest wyświetlany komunikat o błędzie "Połączenie podstawowe zostało zamknięte", może to być związane z wymuszeniem wartości TLS 1.0/1.1. Aby uzyskać więcej informacji, zobacz następujące artykuły:

- [Przygotowanie do protokołu TLS 1.2 w usłudze Office 365 i usłudze Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Błędy uwierzytelniania występują, jeśli klient nie obsługuje protokołu TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Zaktualizuj, aby włączyć protokoły TLS 1.1 i TLS 1.2 jako domyślne protokoły bezpiecznego w WinHTTP w Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Jeśli użytkownicy mają Windows 7, upewnij się, że sprawdzają pakiety [TLS Cipher Suites](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)w Windows 7.