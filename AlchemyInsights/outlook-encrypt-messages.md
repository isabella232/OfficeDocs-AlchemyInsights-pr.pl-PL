---
title: S/MIME w aplikacji Outlook w sieci Web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511518"
---
# <a name="encrypt-email-messages-in-outlook"></a>Szyfrowanie wiadomości e-mail w programie Outlook

Szyfrowanie wiadomości usługi Microsoft 365 jest oparte na usłudze Microsoft Azure Rights Management (Azure RMS), która jest częścią usługi Azure Information Protection. Jeśli subskrypcja obejmuje usługę Azure Rights Management lub usługę Azure Information Protection, **nie trzeba podejmować żadnych działań w celu ręcznego włączenia lub aktywowania** usługi zarządzania prawami.

Na podstawie opinii klientów nie będziemy już domyślnie włączać reguł przepływu poczty programu Exchange do automatycznego szyfrowania wychodzących wiadomości e-mail zawierających określony typ poufnych informacji w dzierżawie. Zamiast tego dostarczamy szczegółowe instrukcje, w jaki sposób możecie to zrobić sami. Aby uzyskać dodatkowe informacje dotyczące tworzenia reguły transportu w celu szyfrowania poufnych informacji, zobacz [ten artykuł](https://aka.ms/OmeEtr).

- Jeśli korzystasz z aplikacji Outlook w sieci Web (dawniej **OWA):** Podczas redagowania wiadomości e-mail po prostu kliknij przycisk **Chroń** w programie OWA. Będzie to dotyczyć uprawnienia "Nie przesyłaj dalej". Kliknij **pozycję Zmień uprawnienie** i wybierz pozycję **Szyfruj,** aby zaszyfrować tylko wiadomość.

- Jeśli używasz **klienta programu Outlook:** Aby wysłać zaszyfrowaną wiadomość z programu Outlook 2013 lub 2016 lub programu Outlook 2016 dla komputerów Mac, wybierz pozycję Uprawnienia **opcji**, a następnie  >  **Permissions**wybierz potrzebną opcję ochrony.

- Aby **automatycznie zaszyfrować wszystkie wiadomości e-mail** wysyłane do określonych adresatów lub zewnętrznych organizacji partnerskich, należy utworzyć regułę transportu przepływu poczty w Centrum administracyjnym programu Exchange. Szczegółowe instrukcje znajdują się w [tym artykule pomocy technicznej](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

