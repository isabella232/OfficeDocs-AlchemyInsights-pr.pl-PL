---
title: Problemy z zarządzaniem użytkownikami
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037515"
---
# <a name="user-management-issues"></a>Problemy z zarządzaniem użytkownikami

**Co się stanie z bieżącymi przypisanymi użytkownikami do aplikacji, jeśli wyłączę właściwość "Wymagane przypisanie użytkownika" (ustawię tę właściwość na Nie)?**

Wyłączenie **wymaganego przypisywania użytkownika** NIE ma wpływu na obecnie przypisanych użytkowników. Wyłączenie tej właściwości spowoduje, że tylko wszyscy użytkownicy będą mieć dostęp do aplikacji. Wszyscy użytkownicy z listy i użytkownicy przypisani do grup w aplikacji nadal będą prawidłowymi.

- Aby ograniczyć aplikację do określonego zestawu użytkowników, zobacz — Ograniczanie aplikacji Azure AD do zestawu użytkowników — Platforma tożsamości firmy Microsoft — [| Dokumenty Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Aby przypisać użytkowników i grupy do aplikacji w przedsiębiorstwie w usłudze Azure Active Directory (Azure AD), z poziomu portalu Azure Portal lub przy użyciu programu PowerShell, zobacz Zarządzanie przypisaniem użytkowników do aplikacji w [usłudze Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)
- Aby delegować uprawnienia tworzenia aplikacji i zarządzania nimi, zobacz Delegowanie uprawnień administratora zarządzania aplikacją [— usługa Azure AD | Dokumenty Microsoft](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Ukrywanie określonych aplikacji przedsiębiorstwa przed użytkownikami —** aby ukryć wszystkie aplikacje platformy Microsoft 365 na panelu **Moje aplikacje,** skorzystaj z poniższych kroków. Aplikacje nadal będą widoczne w portalu usługi Office 365.

 1. Zaloguj się do portalu Azure Portal jako administrator globalny swojego katalogu. 
 2. Wybierz **pozycję Azure Active Directory.** 
 3. Wybierz **pozycję Użytkownicy.** 
 4. Wybierz **pozycję Ustawienia użytkownika.** 
 5. W **obszarze Aplikacje dla przedsiębiorstw** kliknij pozycję Zarządzaj uruchamianiem i wyświetlaniem aplikacji przez użytkowników **końcowych.** 
 6. W przypadku Użytkowników aplikacje usługi Office 365 są dostępne tylko w portalu usługi **Office 365, kliknij** pozycję **Tak.** 
 7. Kliknij przycisk **Zapisz**. 
 8. Aby uzyskać więcej szczegółowych informacji, zobacz Ukrywanie aplikacji przedsiębiorstwa w witrynie [usługi Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Jeśli oferujesz aplikację Software as a Service (SaaS) dla wielu organizacji, możesz tak skonfigurować aplikację, aby akceptowała logowania z dowolnej dzierżawy usługi Azure Active Directory (Azure AD). Ta konfiguracja jest nazywana "tworzeniem aplikacji jako wielodostępu". Użytkownicy w dowolnej dzierżawie usługi Azure AD będą mogli zalogować się do Twojej aplikacji po zgodzie na używanie swojego konta w Twojej aplikacji. Aby uzyskać więcej informacji, zobacz Tworzenie aplikacji, które logują się do [użytkowników usługi Azure AD — platforma tożsamości firmy Microsoft | Dokumenty Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Jak użytkownik końcowy może uzyskać dostęp do aplikacji po przypisaniu go do aplikacji?**

Każda aplikacja w programie Enterprise zawiera link, za pomocą których użytkownicy końcowi mogą uzyskać do nich dostęp. Użytkownicy mogą też w łatwy sposób uzyskać dostęp do aplikacji za pośrednictwem portalu **Myapps.**

- **Chcesz wiedzieć, które aplikacje i typy aplikacji są używane przez użytkowników?**

Raporty logowania za ostatnie 30 dni można pobierać z usługi portal.azure.com > Azure Active Directory i> **i pobierać raporty**> usługi Azure Active Directory.

- Dowiedz się, jak [udzielić](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) zgody administratora dla całej dzierżawy aplikacji i Jak skonfigurować sposób zgody użytkowników [końcowych na aplikacje.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)

- Dowiedz [się, jak działa zgoda](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) [i Zarządzaj zgodą na aplikacje.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)


