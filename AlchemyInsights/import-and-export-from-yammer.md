---
title: Importowanie i eksportowanie z Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037252"
---
# <a name="import-and-export-from-yammer"></a>Importowanie i eksportowanie z Yammer

**Importowanie**

Opcje importowania użytkowników różnią się w zależności od tego, Yammer jest w trybie natywnym platformy [Microsoft 365.](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)

- Tryb **nienatywny:** Użytkowników można importować do grup przy użyciu pozycji Dodaj z książki adresowej [(ograniczenie](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) do 100 użytkowników) w ustawieniach grupy lub do sieci przy użyciu funkcji aktualizacji zbiorczej w obrębie administratora sieci. [](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users)
- **Tryb natywny:** Członkostwo w grupie i operacje członkostwa w sieci powinny być wykonywane z portalu administracyjnego [platformy Microsoft 365,](https://docs.microsoft.com/microsoft-365/admin/add-users)portalu [usługi Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)lub innej opcji usługi Azure AD. Sieci w trybie natywnym nie mają już dostępu do aktualizacji zbiorczej i innych starszych funkcji.

> [!IMPORTANT]
> Yammer nie było obsługiwane importowanie zawartości z poziomu administratora sieci nawet wtedy, gdy funkcja eksportowania danych była używana w innej sieci. Zawartość może być publikowana ponownie przez rozwiązania partnerów lub Yammer interfejsów API rest.

**Eksportowanie**

[Eksportowanie danych sieciowych przez administratora](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) sieci zezwala na eksportowanie zawartości z Yammer sieci, w tym wiadomości i plików. Załączniki mogą być bardzo duże, co spowoduje, że eksport będzie się odbywał bardzo długo. Zalecamy eksportowanie aktywnych sieci przy użyciu interfejsu [API eksportu danych](https://developer.yammer.com/docs/data-export-api) w fragmentach według dnia lub tygodnia. Pomoc techniczna firmy Microsoft nie udostępni w tym celu skryptów niestandardowych.

W celu [wyeksportowania](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) zawartości dla pojedynczego użytkownika istnieje osobny eksport RODO.