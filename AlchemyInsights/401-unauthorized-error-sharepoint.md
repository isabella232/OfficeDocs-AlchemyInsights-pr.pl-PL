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
ms.openlocfilehash: 04f56dfc7ebe7de91bc64a5e6d2b480b07741c6e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314358"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Nieautoryzowany błąd w SharePoint

Jeśli w programie SharePoint zostanie wyświetlony komunikat o błędzie "(401) Nieautoryzowany", może on być związany z dekonfekcją TLS 1.0/1.1. Aby uzyskać więcej informacji, zobacz:

- [Przygotowanie do protokołu TLS 1.2 w usłudze Office 365 i usłudze Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Błędy uwierzytelniania występują, jeśli klient nie obsługuje protokołu TLS 1.2](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Aktualizowanie w celu włączenia protokołów TLS 1.1 i TLS 1.2 jako domyślnych protokołów bezpiecznego w winieHTTP w Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Jeśli użytkownicy mają Windows 7, upewnij się, że sprawdzają pakiety [TLS Cipher Suites w Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)