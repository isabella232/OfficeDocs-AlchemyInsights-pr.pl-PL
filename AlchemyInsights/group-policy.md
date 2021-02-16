---
title: Zasady grupy
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256783"
---
# <a name="group-policy"></a>Zasady grupy

Ustawieniami obiektów użytkowników i komputerów w usłudze Azure Usługi domenowe w usłudze Active Directory (Azure AD DS) często zarządza się przy użyciu obiektów zasady grupy (GPO). Usługa Azure AD DS zawiera wbudowane urządzenia GPO dla kontenerów Użytkowników usługi AADDC i komputerów usługi AADDC. Te wbudowane zasady grupy można dostosowywać w celu skonfigurowania zasad grupy zgodnie z potrzebami środowiska. Członkowie grupy administratorów centrum administracyjnego usługi Azure AD mają uprawnienia do administrowania zasadami grupy w domenie usługi Azure AD DS, a także mogą tworzyć niestandardowe grupy gpos i jednostki organizacyjne. Aby uzyskać więcej informacji na temat zasad grupy i ich działania, zobacz [zasady grupy omówienie.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

W środowisku hybrydowym zasady grupy skonfigurowane w lokalnym środowisku AD DS nie są synchronizowane z usługą Azure AD DS. Aby zdefiniować ustawienia konfiguracji dla użytkowników lub komputerów w usłudze Azure AD DS, edytuj jedno z domyślnych zasad grupy lub utwórz niestandardowy obiektów zasad grupy.

W tym [artykule zasady grupy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) przedstawiono sposób instalowania narzędzi do zarządzania zasady grupy, edytowania wbudowanych zasad grupy oraz tworzenia niestandardowych zasad grupy.



