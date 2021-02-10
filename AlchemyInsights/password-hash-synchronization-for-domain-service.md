---
title: Synchronizacja skrótów haseł dla usługi domeny
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177626"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Synchronizacja skrótów haseł dla usługi domeny

**Jeśli Twoje wystąpienie usługi Azure AD DS wyświetla monit o włączenie synchronizacji skrótów haseł**

Możesz napotkać scenariusz, w którym używasz środowiska hybrydowego z użytkownikami synchronizując je z lokalnego środowiska usługi Azure Usługi domenowe w usłudze Active Directory (AD DS). Ten scenariusz występuje mimo tego, że masz synchronizację skrótów haseł z lokalnej AD DS do dzierżawy usługi Azure AD.

**Przyczyna**

Dzieje się tak, ponieważ program Azure AD Connect domyślnie nie synchronizuje starszych skrótów haseł NTLM (New Technology LAN Manager) i Kerberos, które są wymagane dla usługi Azure AD DS.

**Obejście problemu** 

Konieczne będzie skonfigurowanie programu Azure AD Connect w celu zsynchronizowania tych skrótów haseł wymaganych do uwierzytelniania NTLM i Kerberos.

Po skonfigurowaniu programu Azure AD Connect lokalne zdarzenie tworzenia konta lub zmiany hasła również synchronizuje starsze skróty haseł z usługą Azure AD. Zobacz [tutaj, aby](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) uzyskać więcej informacji na ten temat oraz wskazówki dotyczące włączania synchronizacji haseł w środowisku hybrydowym usługi Azure AD DS.