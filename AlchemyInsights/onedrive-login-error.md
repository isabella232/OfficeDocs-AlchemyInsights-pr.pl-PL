---
title: Błąd logowania do usługi OneDrive AADSTS50011
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
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982485"
---
# <a name="onedrive-login-error-aadsts50011"></a>Błąd logowania do usługi OneDrive AADSTS50011

Jeśli zostanie wyświetlony komunikat o błędzie "AADSTS50011: adres URL odpowiedzi określony w żądaniu jest niezgodny z odpowiedzią" podczas logowania się do aplikacji OneDrive, sprawdź następujące elementy:

Wersja usługi OneDrive musi być równa lub większa niż wersja 20.052. XXXX. XX. Aby sprawdzić wersję, kliknij niebieską ikonę usługi OneDrive w obszarze powiadomień, wybierz pozycję **pomoc & ustawienia > ustawienia > informacje**.

Sieć może blokować ruch do **g.Live.com** i **oneclient.SFX.MS**. Jeśli ten ruch jest zablokowany, usługa OneDrive nie może go zaktualizować. Skontaktuj się z administratorem sieci, aby upewnić się, że masz dostęp do tych adresów URL. [Te punkty końcowe](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) powinny być dostępne dla klientów korzystających z planów Microsoft 365.

Jeśli chcesz ręcznie uzyskać aktualną wersję usługi OneDrive, odwiedź stronę [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
