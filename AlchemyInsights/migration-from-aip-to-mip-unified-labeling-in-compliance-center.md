---
title: Migracja z centrali Środkowej do MCI/ujednolicona etykietowanie w centrum zgodności
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674336"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migracja z centrali Środkowej do MCI/ujednolicona etykietowanie w centrum zgodności

Aby przeprowadzić migrację z etykiet centralnych do ujednoliconych etykiet w centrum zabezpieczeń i zgodności, wykonaj następujące czynności:

**Aktywowanie ochrony w portalu Azure**

1. Jeśli jeszcze tego nie zrobiono, Otwórz nowe okno przeglądarki i [Zaloguj się w witrynie Azure Portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Przejdź do bloku **Ochrona informacji platformy Azure** . Na przykład w menu centrum kliknij pozycję **wszystkie usługi** i zacznij wpisywać **informacje** w polu Filtr. Wybierz pozycję **Ochrona informacji platformy Azure**. Jeśli nie uzyskano dostępu do bloku usługi Azure Information Protection, zobacz [dodatkowe czynności](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) , które umożliwiają dodanie tego bloku do portalu. Aby otworzyć blok usługi Azure Information Protection, musisz mieć [Plan Premium (Azure Information Protection](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) ) lub plan Office 365, który zawiera Zarządzanie prawami. Jeśli masz już taką subskrypcję, ale widzisz komunikat, że nie można znaleźć prawidłowego abonamentu, [skontaktuj się z pomocą techniczną firmy Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) lub skorzystaj ze standardowych kanałów pomocy technicznej.

2. Znajdź opcje menu **Zarządzaj** , a następnie wybierz pozycję **Aktywacja ochrony**. Kliknij pozycję **Aktywuj**, a następnie Potwierdź działanie. Po zakończeniu aktywacji na pasku informacji jest wyświetlana informacja, że **Aktywacja została pomyślnie zakończona**.

**Migrowanie etykiet ochrony informacji platformy Azure do usługi Office 365 Security & Centrum zgodności**

1. Upewnij się, że zalogowano się jako użytkownik z uprawnieniami administratora globalnego.

2. Przejdź do bloku **Ochrona informacji platformy Azure** .

3. W menu **Zarządzaj** wybierz opcję **ujednolicone etykietowanie**.

4. Na **wbudowanym bloku etykiet na platformie Azure Information Protection** kliknij pozycję **Aktywuj** i postępuj zgodnie z instrukcjami online.

**Uwaga**: Sprawdź, czy masz odpowiednie uprawnienia, zanim uaktywnisz migrację centrum zabezpieczeń & zgodności. Aby uzyskać więcej informacji, zobacz następujące artykuły:

1. [Czy musisz być administratorem globalnym w celu skonfigurowania usługi Azure Information Protection lub można delegować do innych administratorów?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Ważne informacje dotyczące ról administracyjnych po przeprowadzeniu migracji do centrum zgodności z zabezpieczeniami &.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Aby uzyskać więcej informacji na temat podwyższania poziomu migracji etykiet do centrum zabezpieczeń i zgodności, zobacz [Migrowanie etykiet](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
