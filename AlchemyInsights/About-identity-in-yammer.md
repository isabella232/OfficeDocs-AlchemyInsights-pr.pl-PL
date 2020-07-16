---
title: Informacje o tożsamości w usłudze Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148307"
---
# <a name="about-identity-in-yammer"></a>Informacje o tożsamości w usłudze Yammer

Zaleca się, aby wszystkie sieci podjęła następujące kroki w celu uniknięcia problemów związanych z tożsamością:

1. Wymuszaj tożsamość usługi Office 365 po zainicjowaniu obsługi administracyjnej kont usługi Microsoft 365 dla użytkowników usługi Azure AD, aby upewnić się, że wszyscy użytkownicy logują się przy użyciu podstawowego konta usługi Microsoft 365. Aby uzyskać więcej informacji, zobacz [Wymuszanie tożsamości usługi Office 365 dla użytkowników usługi Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Skonsoliduj wiele sieci yammer. Starsze konfiguracje usługi Yammer umożliwiają podłączenie wielu sieci usługi Yammer do jednej dzierżawy. Aby uzyskać więcej informacji, zobacz [Migracja sieci — konsolidacja wielu sieci usługi Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Opcjonalnie wymuś licencjonowanie usługi Yammer, aby zablokować użytkownikom usługę Yammer, jeśli nie mają licencji. Aby uzyskać więcej informacji, zobacz [Zarządzanie licencjami użytkowników usługi Yammer w usłudze Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Na koniec inspekcji listy użytkowników dla starszych sieci Yammer i zawiesić starszych użytkowników. Zaleca się zawieszenie (dezaktywację) użytkowników zamiast ich usuwania, ponieważ usunięcie jest nieodwracalne. Aby uzyskać więcej informacji, zobacz [Inspekcja użytkowników usługi Yammer w sieciach połączonych z usługą Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) i [Usuwanie użytkowników](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Konfigurując usługę Yammer przy użyciu tych kroków, możesz również skonfigurować sieć Yammer dla trybu macierzystego dla usługi Microsoft 365. Aby uzyskać więcej informacji, zobacz [Konfigurowanie sieci Usługi Yammer w trybie macierzystym dla usługi Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).