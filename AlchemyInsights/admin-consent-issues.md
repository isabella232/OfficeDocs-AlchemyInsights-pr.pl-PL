---
title: Problemy ze zgodą administratora
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952583"
---
# <a name="admin-consent-issues"></a>Problemy ze zgodą administratora

1. Włącz przepływ [pracy zgody administratora,](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) aby umożliwić użytkownikom żądanie zatwierdzenia administratora bezpośrednio z ekranu zgody.

1. Jeśli w trakcie procesu wyrażania zgody Ty lub użytkownicy Twojej aplikacji widzisz nieoczekiwane błędy, zobacz ten artykuł, aby uzyskać informacje na temat rozwiązywania problemów: Nieoczekiwany błąd podczas wykonywania zgody [na aplikację.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)

1. Dowiedz się więcej [o zgodzie](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)administratora na [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) Platforma tożsamości Microsoft, jak działa monit o zgodę, oraz jak oceniać żądanie zgody [administratora dla całej dzierżawy.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. Aplikacje integrują się z Platforma tożsamości Microsoft modelem autoryzacji, który zapewnia użytkownikom i administratorom kontrolę nad dostępem do danych. Implementacja modelu autoryzacji została zaktualizowana w punkcie Platforma tożsamości Microsoft końcowego i zmienia sposób interakcji aplikacji z Platforma tożsamości Microsoft. Zobacz [Uprawnienia i zgody w punkcie Platforma tożsamości Microsoft,](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) aby uzyskać omówienie tego modelu autoryzacji, w tym zakresów, uprawnień i zgody.