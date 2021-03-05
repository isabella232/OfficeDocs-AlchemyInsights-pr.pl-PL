---
title: Synchronizacja haseł
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482041"
---
# <a name="password-synchronization"></a><span data-ttu-id="85978-102">Synchronizacja haseł</span><span class="sxs-lookup"><span data-stu-id="85978-102">Password synchronization</span></span>

<span data-ttu-id="85978-103">**Synchronizacja skrótów haseł w ogóle nie działa**</span><span class="sxs-lookup"><span data-stu-id="85978-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="85978-104">Niektóre typowe problemy napotykane przez klientów, gdy synchronizacja skrótów haseł nie działa:</span><span class="sxs-lookup"><span data-stu-id="85978-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="85978-105">Konto usługi Active Directory używane przez usługę Azure AD Connect  do komunikowania się z lokalną usługą Active Directory nie jest udzielane uprawnień Do replikowania zmian w katalogu i replikowania zmian katalogu **Wszystkie** uprawnienia, które są wymagane do synchronizacji haseł — należy rozwiązać ten problem, udzielając tych uprawnień kontu usługi Active Directory.</span><span class="sxs-lookup"><span data-stu-id="85978-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="85978-106">Synchronizacja skrótów haseł jest wyłączona po zmianie  przez administratora metody user Sign-In z synchronizacji haseł na inną opcję, taką jak  federacja z usługami **AD FS** w kreatorze Azure AD Connect — ten problem można rozwiązać, ponownie włączając funkcję synchronizacji skrótów haseł w kreatorze Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="85978-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="85978-107">Problem z łącznością z lokalną usługą Active Directory.</span><span class="sxs-lookup"><span data-stu-id="85978-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="85978-108">Na przykład niektóre kontrolery domeny nie są dostępne [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) przez usługę Azure AD Connect lub wymagane porty są blokowane przez zaporę — należy rozwiązać ten problem, upewniając się, że łączność między serwerem Azure AD Connect a lokalną usługą Active Directory działa prawidłowo.</span><span class="sxs-lookup"><span data-stu-id="85978-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="85978-109">Serwer Azure AD Connect jest obecnie w trybie tymczasowego, co spowoduje, że serwer nie będzie mógł uzyskać skrótów haseł — Aby rozwiązać ten problem, wykonaj czynności opisane w sekcji Rozwiązywanie problemów z synchronizacją haseł z synchronizacją programu [Azure AD Connect —](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)nie są synchronizowane żadne hasła.</span><span class="sxs-lookup"><span data-stu-id="85978-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="85978-110">**Synchronizacja skrótów haseł nie działa w przypadku niektórych użytkowników**</span><span class="sxs-lookup"><span data-stu-id="85978-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="85978-111">Jeśli zauważysz, że skrót haseł nie jest synchronizowany  dla użytkownika, użyj zadania rozwiązywania problemów w programie Azure AD Connect, aby zbadać i rozwiązać ten problem.</span><span class="sxs-lookup"><span data-stu-id="85978-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="85978-112">Wykonaj następujące zadania:</span><span class="sxs-lookup"><span data-stu-id="85978-112">Perform the following tasks:</span></span>

    <span data-ttu-id="85978-113">a.</span><span class="sxs-lookup"><span data-stu-id="85978-113">a.</span></span> [<span data-ttu-id="85978-114">Uruchamianie zadania rozwiązywania problemów w kreatorze</span><span class="sxs-lookup"><span data-stu-id="85978-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="85978-115">b.</span><span class="sxs-lookup"><span data-stu-id="85978-115">b.</span></span> [<span data-ttu-id="85978-116">Używanie polecenia cmdlet do rozwiązywania problemów w celu zbadania problemu z synchronizacją skrótów haseł dla określonego użycia</span><span class="sxs-lookup"><span data-stu-id="85978-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="85978-117">Dla obiektu użytkownika lokalnej usługi Active Directory jest włączona opcja Użytkownik musi zmienić hasło **przy następnej** opcji logowania.</span><span class="sxs-lookup"><span data-stu-id="85978-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="85978-118">Gdy ta opcja jest włączona, użytkownikowi jest przypisywane hasło tymczasowe i zostanie wyświetlony monit o zmianę hasła przy następnym loganiu.</span><span class="sxs-lookup"><span data-stu-id="85978-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="85978-119">Program Azure AD Connect nie synchronizuje haseł tymczasowych z usługą Azure AD.</span><span class="sxs-lookup"><span data-stu-id="85978-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="85978-120">Aby rozwiązać powyższy problem, wykonaj jedną z następujących czynności:</span><span class="sxs-lookup"><span data-stu-id="85978-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="85978-121">Poproś użytkownika o zalogowanie się do aplikacji lokalnej (na przykład aplikacji klasycznej systemu Windows) i zmianę hasła.</span><span class="sxs-lookup"><span data-stu-id="85978-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="85978-122">Nowe hasło zostanie zsynchronizowane z usługą Azure AD.</span><span class="sxs-lookup"><span data-stu-id="85978-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="85978-123">Niech administrator zaktualizuje hasło użytkownika bez włączania opcji Użytkownik musi zmienić hasło podczas następnego logowania **i** udostępnić nowe hasło użytkownikowi.</span><span class="sxs-lookup"><span data-stu-id="85978-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="85978-124">Obiekt użytkownika lokalnej usługi Active Directory **nie** jest poprawnie skonfigurowany do synchronizacji obiektów lub synchronizacji haseł.</span><span class="sxs-lookup"><span data-stu-id="85978-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="85978-125">Aby rozwiązać ten problem, wykonaj czynności opisane w tece Rozwiązywanie problemów z synchronizacją skrótów haseł za [pomocą synchronizacji programu Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="85978-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







