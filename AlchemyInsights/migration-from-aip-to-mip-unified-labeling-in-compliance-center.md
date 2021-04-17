---
title: Migracja z usługi AIP do rozwiązania MIP/unified Labeling w Centrum zgodności
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825381"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migracja z usługi AIP do rozwiązania MIP/unified Labeling w Centrum zgodności

Aby przeprowadzić migrację etykiet AIP do funkcji Unified Labeling w Centrum zabezpieczeń i zgodności, wykonaj następujące czynności:

**Aktywowanie ochrony z portalu Azure Portal**

1. Jeśli jeszcze tego nie zrobiono, otwórz nowe okno przeglądarki i [zaloguj się do portalu Azure Portal.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal) Przejdź do **bladej usługi Azure Information Protection.** Na przykład w menu Centrum kliknij pozycję **Wszystkie** usługi i zacznij wpisywać **informacje** w polu Filtruj. Wybierz **pozycję Azure Information Protection**. Jeśli do tej pory nie uzyskiwano dostępu do grota usługi Azure Information Protection, zapoznaj się z dodatkowymi czynnościami w celu dodania tego grota do portalu. [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) Aby otworzyć blok danych usługi Azure Information Protection, musisz mieć [plan Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) lub plan usługi Office 365, który obejmuje zarządzanie prawami. Jeśli masz jedną z tych subskrypcji, ale jest wyświetlany komunikat informujący, że nie można odnaleźć ważnej subskrypcji, skontaktuj się z pomocą techniczną firmy [Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) lub skorzystaj ze standardowych kanałów pomocy technicznej.

2. Znajdź opcje menu **Zarządzaj** i wybierz pozycję **Aktywacja ochrony.** Kliknij **przycisk** Aktywuj , a następnie potwierdź swoje działanie. Po zakończeniu aktywacji na pasku informacji zostanie wyświetlony **komunikat Pomyślnie ukończono aktywację.**

**Migrowanie etykiet usługi Azure Information Protection do Centrum zabezpieczeń & Office 365**

1. Upewnij się, że zalogowano się jako użytkownik z uprawnieniami administratora globalnego.

2. Przejdź do **bladej usługi Azure Information Protection.**

3. Z menu **Zarządzaj** wybierz pozycję **Ujednolicone etykiety**.

4. Na stronie **Azure Information Protection — ujednolicone pole etykiet** kliknij przycisk **Aktywuj** i postępuj zgodnie z instrukcjami online.

**Uwaga:** przed aktywowaniem migracji Centrum zgodności w centrum zabezpieczeń & upewnij się, że masz odpowiednie uprawnienia. Aby uzyskać więcej informacji, zobacz następujące artykuły:

1. [Czy musisz być administratorem globalnym, aby skonfigurować usługę Azure Information Protection, czy mogę delegować innych administratorów?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Ważne informacje o rolach administracyjnych po migracji do Centrum & zabezpieczeń.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Aby uzyskać więcej informacji na temat migracji Z usługi AIP do usługi Unified Labeling do Centrum zabezpieczeń i zgodności, zobacz [Migrowanie etykiet.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)
