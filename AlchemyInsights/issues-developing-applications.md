---
title: Problemy związane z tworzeniem aplikacji
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013434"
---
# <a name="issues-developing-applications"></a>Problemy związane z tworzeniem aplikacji

Aby rozwiązać najbardziej typowe problemy podczas tworzenia aplikacji usługi Azure Active Directory (AD), zobacz następujące artykuły:

- [Widzę problemy z logowaniem się do aplikacji tylko przy użyciu przeglądarki Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Nie wiem, jak zmienić domyślne wartości domyślne okresu istnienia tokenu dla mojej aplikacji](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Nie wiem, jak działa zgoda aplikacji](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Nie wiem, jak udzielić uprawnień do mojej aplikacji](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Nie rozumiem różnicy między uprawnieniami delegowanymi a uprawnieniami aplikacji](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Zakończenie świadczenia pomocy technicznej dla biblioteki ADAL (Azure Active Directory Authentication Library) i interfejsu API azure AD Graph (AAD Graph)***

- Począwszy od 30 czerwca 2020 r. nie będziemy już dłużej dodawać żądnych nowych funkcji do biblioteki Azure Active Directory Authentication Library (ADAL) oraz interfejsu API usługi AD Graph (AAD Graph). Będziemy nadal zapewniać pomoc techniczną i aktualizacje zabezpieczeń, natomiast nie będziemy dłużej dostarczać aktualizacji funkcji.

- Począwszy od 30 czerwca 2022 r. zakończymy świadczenie pomocy technicznej dla biblioteki ADAL i usługi AAD Graph, a także nie będziemy dłużej zapewniać pomocy technicznej lub aktualizacji zabezpieczeń. Z powodu tego warunku następujące skutki są następujące:

    - Aplikacje używające biblioteki ADAL w istniejących wersjach systemu operacyjnego nadal będą działać po tej dacie, lecz nie będą uzyskiwać żadnej pomocy technicznej lub aktualizacji zabezpieczeń.

    - Aplikacje korzystające z Graph AAD po tym czasie mogą już nie otrzymywać odpowiedzi z punktu Graph AAD

**Migracja ADAL**

Jeśli korzystasz z aplikacji firmy Microsoft, zalecamy aktualizację do biblioteki Microsoft Authentication Library (MSAL), która zawiera najnowsze funkcje i aktualizacje zabezpieczeń. To zalecenie znajduje się w kontekście inicjowania przez firmę Microsoft procesu migrowania jej aplikacji do programu MSAL do terminu zakończenia wsparcia technicznego. 

Migracja aplikacji firmy Microsoft do programu MSAL gwarantuje, że aplikacje będą korzystać z bieżących ulepszeń zabezpieczeń i funkcji pakietu MSAL.

1. [Przeczytaj sekcję ADAL — często zadawane pytania](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Dowiedz się na temat sposobu migracji aplikacji zależnie od platformy](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Jeśli potrzebujesz pomocy w zrozumieniu, które z Twoich aplikacji korzystają z pliku ADAL, zalecamy zapoznanie się ze wszystkimi kodami źródłowymi aplikacji i, jeśli to konieczne, s strzyganie się z dowolnymi niezależnymi dostawcami oprogramowania (ISV) lub dostawcami aplikacji. Pomoc techniczna firmy Microsoft może również dostarczyć listę aplikacji ADAL innych firm w Twojej dzierżawie.

**Migracja usługi AAD Graph**

W przypadku aplikacji korzystających z usługi AAD Graph migruj aplikacje AAD do usługi Microsoft Graph do usługi Microsoft Graph:

1. [Nasz lista kontrolna dotycząca migracji stanowi punkt umożliwiający rozpoczęcie](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Portal rejestracji aplikacji Azure pokazuje, jakie aplikacje używają usługi AAD Graph. Zalecamy zapoznanie się ze wszystkimi kodami źródłowymi aplikacji i, jeśli to zastosowanie, strzyganie się z dowolnymi niezależnymi dostawcami oprogramowania (ISV) lub dostawcami aplikacji. Pomoc techniczna firmy Microsoft może również udostępnić Ci informacje na temat użycia Graph AAD w Twojej dzierżawie.







