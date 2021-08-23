---
title: Moja aplikacja nie jest pokazywana w zarządzaniu aplikacją
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454995"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Moja aplikacja nie jest pokazywana w zarządzaniu aplikacją

Jeśli twoja aplikacja nie jest wyświetlona w programie Zarządzanie aplikacją, sprawdź następujące kwestie:

1. Przejdź do [usługi Azure AD](https://aad.portal.azure.com/) i znajdź identyfikator aplikacji, wyszukując nazwę aplikacji na górnym pasku na stronie Omówienie.

1. Uzyskaj Graph i wyszukaj identyfikator aplikacji w ramach podmiotu zabezpieczeń usługi, używając tego zapytania i zastępując nim odpowiedni identyfikator <appId> aplikacji: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Jeśli nie zostaną zwrócone żadne wyniki, wyszukaj identyfikator aplikacji w aplikacji, używając tego zapytania i zastępując nim odpowiedni identyfikator <appId> aplikacji: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Jeśli wystąpią problemy z zapytaniem, zobacz [Uzyskiwanie pomocy technicznej.](https://docs.microsoft.com/microsoft-365/business-video/get-help-support) 

Aby uzyskać więcej informacji lub uzyskać więcej informacji na temat aplikacji w zarządzaniu aplikacjami, zobacz Więcej informacji na temat [widoczności i szczegółowych informacji.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Aby uzyskać więcej informacji na temat wyświetlania aplikacji, [zobacz Wyświetlanie aplikacji.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)
