---
title: Wdrażanie zasad grupy
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
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427564"
---
# <a name="gpo-deployment"></a>Wdrażanie zasad grupy

Ustawieniami obiektów użytkowników i komputerów w usłudze Azure Usługi domenowe w usłudze Active Directory (Azure AD DS) często zarządza się przy użyciu obiektów zasady grupy (GPO). Usługa Azure AD DS zawiera wbudowane urządzenia GPO dla kontenerów Użytkowników usługi AADDC i komputerów usługi AADDC. Te wbudowane zasady grupy można dostosowywać w celu skonfigurowania zasad grupy zgodnie z potrzebami środowiska. Członkowie grupy administratorów centrum administracyjnego usługi Azure AD mają uprawnienia do administrowania zasadami grupy w domenie usługi Azure AD DS, a także mogą tworzyć niestandardowe grupy gpos i jednostki organizacyjne. Aby uzyskać więcej informacji na temat zasad grupy i ich działania, zobacz [zasady grupy Omówienie.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

W środowisku hybrydowym zasady grupy skonfigurowane w lokalnym środowisku AD DS nie są synchronizowane z usługą Azure AD DS. Aby zdefiniować ustawienia konfiguracji dla użytkowników lub komputerów w usłudze Azure AD DS, edytuj jedno z domyślnych zasad grupy lub utwórz niestandardowy obiektów zasad grupy.

W tym [artykule zasady grupy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) przedstawiono sposób instalowania narzędzi do zarządzania zasady grupy, edytowania wbudowanych zasad grupy oraz tworzenia niestandardowych zasad grupy.
