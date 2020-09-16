---
title: Informacje o tożsamości w usłudze Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664180"
---
# <a name="about-identity-in-yammer"></a>Informacje o tożsamości w usłudze Yammer

Zaleca się, aby w celu uniknięcia problemów związanych z tożsamością wszystkie sieci miały następujące kroki:

1. Wymuś tożsamość pakietu Office 365 po zainicjowaniu obsługi kont Microsoft 365 dla użytkowników w usłudze Azure AD, aby upewnić się, że wszyscy użytkownicy logują się przy użyciu ich podstawowego konta Microsoft 365. Aby uzyskać więcej informacji, zobacz [Wymuszaj tożsamość pakietu Office 365 dla użytkowników usługi Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Konsolidowanie wielu sieci usługi Yammer. Starsze konfiguracje usługi Yammer umożliwiają połączenie wielu sieci Yammer z jedną dzierżawą. Aby uzyskać więcej informacji, zobacz [Migrowanie sieci — konsolidowanie wielu sieci usługi Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Opcjonalnie Wymuś Licencjonowanie w usłudze Yammer, aby blokować użytkowników z usługi Yammer, jeśli nie mają licencji. Aby uzyskać więcej informacji, zobacz [Zarządzanie licencjami użytkowników usługi Yammer w pakiecie Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Na koniec Przeprowadź inspekcję listy użytkowników dla starszych sieci usługi Yammer i Zawieś starszych użytkowników. Zaleca się, aby zamiast usuwać użytkowników zawiesić (dezaktywować), ponieważ usunięcie jest nieodwracalne. Aby uzyskać więcej informacji, zobacz [Przeprowadź inspekcję użytkowników usługi Yammer w sieciach połączonych z pakietem Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) i [Usuń użytkowników](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Konfigurując usługę Yammer za pomocą tych kroków, możesz również skonfigurować sieć usługi Yammer dla trybu macierzystego programu Microsoft 365. Aby uzyskać więcej informacji, zobacz [Konfigurowanie sieci usługi Yammer dla trybu macierzystego dla programu Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).