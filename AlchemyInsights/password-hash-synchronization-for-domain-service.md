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
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="a384a-102">Synchronizacja skrótów haseł dla usługi domeny</span><span class="sxs-lookup"><span data-stu-id="a384a-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="a384a-103">**Jeśli Twoje wystąpienie usługi Azure AD DS wyświetla monit o włączenie synchronizacji skrótów haseł**</span><span class="sxs-lookup"><span data-stu-id="a384a-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="a384a-104">Możesz napotkać scenariusz, w którym używasz środowiska hybrydowego z użytkownikami synchronizując je z lokalnego środowiska usługi Azure Usługi domenowe w usłudze Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="a384a-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="a384a-105">Ten scenariusz występuje mimo tego, że masz synchronizację skrótów haseł z lokalnej AD DS do dzierżawy usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a384a-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="a384a-106">**Przyczyna**</span><span class="sxs-lookup"><span data-stu-id="a384a-106">**Cause**</span></span>

<span data-ttu-id="a384a-107">Dzieje się tak, ponieważ program Azure AD Connect domyślnie nie synchronizuje starszych skrótów haseł NTLM (New Technology LAN Manager) i Kerberos, które są wymagane dla usługi Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="a384a-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="a384a-108">**Obejście problemu**</span><span class="sxs-lookup"><span data-stu-id="a384a-108">**Workaround**</span></span> 

<span data-ttu-id="a384a-109">Konieczne będzie skonfigurowanie programu Azure AD Connect w celu zsynchronizowania tych skrótów haseł wymaganych do uwierzytelniania NTLM i Kerberos.</span><span class="sxs-lookup"><span data-stu-id="a384a-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="a384a-110">Po skonfigurowaniu programu Azure AD Connect lokalne zdarzenie tworzenia konta lub zmiany hasła również synchronizuje starsze skróty haseł z usługą Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a384a-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="a384a-111">Zobacz [tutaj, aby](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) uzyskać więcej informacji na ten temat oraz wskazówki dotyczące włączania synchronizacji haseł w środowisku hybrydowym usługi Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="a384a-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>