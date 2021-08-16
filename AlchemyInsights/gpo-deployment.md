---
title: Wdrożenie zasad grupy
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067850"
---
# <a name="gpo-deployment"></a>Wdrożenie zasad grupy

Ustawienia obiekty użytkowników i komputerów w usługach domenowych Azure Active Directory domenowych (Azure AD DS) są często zarządzane przy użyciu obiektów zasady grupy (GPOs). Usługa Azure AD DS zawiera wbudowane urządzenia GPOs dla kontenerów Użytkownicy usługi AADDC i Komputery AADDC. Te wbudowane urządzenia gpOs można dostosować w celu skonfigurowania zasad grupy zgodnie z potrzebami środowiska. Członkowie grupy administratorów centrum administracyjnego centrum administracyjnego usługi Azure AD mają uprawnienia do administrowania zasadami grupy w domenie usługi Azure AD DS oraz mogą również tworzyć niestandardowe gpos i jednostki organizacyjne. Aby uzyskać więcej informacji na temat zasad grupy i ich działania, zobacz Omówienie zasady grupy [grupy.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

W środowisku hybrydowym zasady grupy skonfigurowane w lokalnym środowisku AD DS nie są synchronizowane z usługą Azure AD DS. Aby zdefiniować ustawienia konfiguracji dla użytkowników lub komputerów w usłudze Azure AD DS, edytuj jedno z domyślnych obiektów GPOS lub utwórz niestandardowy magazyn zasad grupy.

W tym [artykule zasady grupy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) opisano sposób instalowania narzędzi do zarządzania zasady grupy, edytowania wbudowanych obiektów GPOs i tworzenia niestandardowych obiektów GPOs.
