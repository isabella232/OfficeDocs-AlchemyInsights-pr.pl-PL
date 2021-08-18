---
title: OneDrive błędu logowania AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112922"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive błędu logowania AADSTS50011

Jeśli podczas logowania do aplikacji OneDrive zostanie wyświetlony komunikat o błędzie "AADSTS50011: Adres URL odpowiedzi określony w żądaniu nie jest zgodne z odpowiedzią", sprawdź, czy są one następujące:

Twoja OneDrive musi być równa lub większa niż wersja 20.052.XXXX.XXXX. Aby sprawdzić wersję, kliknij niebieską ikonę OneDrive w obszar powiadomień pomoc, a następnie **& Ustawienia > Ustawienia > informacje**.

Twoja sieć może blokować ruch do **g.live.com** i **oneclient.sfx.ms.** Jeśli ruch zostanie zablokowany, oznacza to OneDrive nie może zaktualizować się. We współpracy z administratorem sieci upewnij się, że masz dostęp do tych adresów URL. [Te punkty końcowe powinny](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) być osiągalne dla klientów korzystających z Microsoft 365 sieci web.

Jeśli chcesz ręcznie uzyskać bieżącą wersję pakietu OneDrive, odwiedź stronę [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
