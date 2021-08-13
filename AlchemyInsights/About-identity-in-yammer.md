---
title: Informacje o tożsamości w programie Yammer
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
ms.openlocfilehash: 57e7e6328747fc05b89799d631b2c6d7e0056547253aa3d75cdecb38cea3ad7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918947"
---
# <a name="about-identity-in-yammer"></a>Informacje o tożsamości w programie Yammer

Zaleca się, aby wszystkie sieci chłoną się w ten sposób, aby uniknąć problemów związanych z tożsamością:

1. Wymusz Office 365 po Microsoft 365 kontach użytkowników w usłudze Azure AD, aby zapewnić, że wszyscy użytkownicy logują się przy użyciu ich podstawowych kont Microsoft 365 konta. Aby uzyskać więcej informacji, zobacz [Wymuszanie Office 365 tożsamości dla Yammer użytkowników.](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)
2. Konsolidowanie wielu Yammer sieci. Starsze Yammer umożliwiają Yammer wielu sieciach połączonych z jedną dzierżawą. Aby uzyskać więcej informacji, zobacz [Migracja sieci — konsolidowanie wielu Yammer sieci.](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)
3. Opcjonalnie wymusz licencjonowanie Yammer celu zablokowania Yammer użytkowników, którzy nie mają licencji. Aby uzyskać więcej informacji, zobacz [Zarządzanie Yammer użytkownikami w aplikacji Office 365.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)
4. Na koniec przejmij inspekcję listy użytkowników dla starszych Yammer sieci i zawieś starszych użytkowników. Zaleca się zawieszanie (dezaktywowanie) użytkowników zamiast ich usuwania, ponieważ usuwanie jest nieodwracalne. Aby uzyskać więcej informacji, zobacz [Inspekcja Yammer użytkowników w sieciach połączonych](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) Office 365 [i Usuwanie użytkowników.](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)

Konfigurując Yammer przy użyciu tych kroków, możesz również skonfigurować sieć w Yammer natywny dla Microsoft 365. Aby uzyskać więcej informacji, [zobacz Konfigurowanie Yammer sieci na Microsoft 365.](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)