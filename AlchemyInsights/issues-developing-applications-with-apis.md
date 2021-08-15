---
title: Problemy podczas opracowywania aplikacji z interfejsami API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013470"
---
# <a name="issues-developing-applications-with-apis"></a>Problemy podczas opracowywania aplikacji z interfejsami API

Aby rozpocząć korzystanie z interfejsu API Azure Active Directory Graph, zobacz przewodnik Szybki start interfejsu API usługi [Azure AD Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) lub zapoznaj się z interakcyjną dokumentacją interfejsu API usługi Azure AD [Graph.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Zakończenie świadczenia pomocy technicznej dla biblioteki ADAL (Azure Active Directory Authentication Library) i interfejsu API azure AD Graph (AAD Graph)**

**Począwszy od 30 czerwca 2020** r. nie będziemy już dodawać żadnych nowych funkcji do usługi ADAL ani Azure AD Graph. Będziemy nadal zapewniać pomoc techniczną i aktualizacje zabezpieczeń, natomiast nie będziemy dłużej dostarczać aktualizacji funkcji.

**Począwszy od 30 czerwca 2022 r.,** zakończymy świadczenie pomocy technicznej dla usługi ADAL i Azure AD Graph i nie będziemy już zapewniać pomocy technicznej ani aktualizacji zabezpieczeń.

Aplikacje używające biblioteki ADAL w istniejących wersjach systemu operacyjnego nadal będą działać po tej dacie, lecz nie będą uzyskiwać żadnej pomocy technicznej lub aktualizacji zabezpieczeń.

Aplikacje korzystające z usługi Azure AD Graph tym czasie mogą już nie odbierać odpowiedzi z punktu końcowego usługi Azure AD Graph sieci Web.

**Migracja ADAL**

Zalecamy zaktualizowanie do [Biblioteki uwierzytelniania Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), która oferuje najnowsze aktualizacje funkcji i zabezpieczeń.

Jeśli korzystasz z aplikacji firmy Microsoft, migruj aplikacje do programu MSAL do terminu zakończenia świadczenia pomocy technicznej, upewniając się, że będą one korzystać z bieżących ulepszeń zabezpieczeń i funkcji programu MSAL.

1. [Przeczytaj często zadawane pytania dotyczące ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Dowiedz się, jak migrować aplikacje na platformie.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Jeśli potrzebujesz pomocy w zrozumieniu, które z Twoich aplikacji korzystają z pliku ADAL, zalecamy zapoznanie się ze wszystkimi kodami źródłowymi aplikacji i, jeśli to konieczne, spływaj do wszystkich usługodawców internetowych (ISV) lub dostawców aplikacji. Pomoc techniczna firmy Microsoft może również dostarczyć listę aplikacji ADAL innych firm w Twojej dzierżawie.

**Migracja usługi AAD Graph**

W przypadku aplikacji korzystających z usługi Azure AD Graph skorzystaj z naszych wskazówek dotyczących migrowania aplikacji usługi [Azure AD Graph do usługi Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [Nasz lista kontrolna dotycząca migracji stanowi punkt umożliwiający rozpoczęcie](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Portal rejestracji aplikacji Azure pokazuje, jakie aplikacje używają usługi AAD Graph. Zalecamy przejrzenie kodu źródłowego wszystkich Twoich aplikacji i, w razie potrzeby, skontaktowanie się z dowolnym dostawcą ISV lub dostawcą aplikacji. Pomoc techniczna firmy Microsoft może także udostępnić listę wszystkich funkcji AAD Graph użycia w Twojej dzierżawie.
1. Aby Twoja aplikacja uzyskać dostęp do danych w aplikacji Microsoft Graph, użytkownik lub administrator musi udzielić im właściwych uprawnień w ramach procesu zgody. Odwołanie [do Graph firmy Microsoft](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) zawiera listę uprawnień skojarzonych z każdym głównym zestawem interfejsów API usługi Microsoft Graph API. Zawiera również wskazówki dotyczące korzystania z tych uprawnień.
