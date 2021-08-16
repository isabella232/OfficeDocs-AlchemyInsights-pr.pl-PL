---
title: S/MIME w programie Outlook w sieci Web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010734"
---
# <a name="encrypt-email-messages-in-outlook"></a>Szyfrowanie wiadomości e-mail w Outlook

Microsoft 365 Szyfrowanie wiadomości jest zbudowane na usłudze Microsoft Azure zarządzania prawami dostępu (Azure RMS), która jest częścią usługi Azure Information Protection. Jeśli Twoja subskrypcja obejmuje usługę Azure Rights Management lub Azure Information **Protection,** nie musisz nic robić, aby ręcznie włączyć lub aktywować usługę zarządzania prawami.

Zgodnie z opiniami klientów nie będziemy już włączać reguł przepływu poczty Exchange automatycznie szyfrować wychodzące wiadomości e-mail zawierające określony typ informacji poufnych w dzierżawie. Zamiast tego udostępniamy szczegółowe instrukcje dotyczące sposobu, w jaki możesz to zrobić samodzielnie. Aby uzyskać dodatkowe informacje na temat tworzenia reguły transportu w celu szyfrowania informacji poufnych, zobacz [ten artykuł.](https://aka.ms/OmeEtr)

- Jeśli używasz Outlook sieci Web (dawniej **OWA):** podczas redagowania wiadomości e-mail po prostu kliknij **pozycję Chroń w** aplikacji OWA. Spowoduje to zastosowanie uprawnienia "Nie przesyłaj dalej". Kliknij **pozycję Zmień uprawnienie** i wybierz pozycję **Zaszyfruj,** aby zaszyfrować tylko wiadomość.

- Jeśli używasz **Outlook klienta:** Aby wysłać zaszyfrowaną wiadomość z programu Outlook 2013 lub 2016 albo Outlook 2016 dla komputerów Mac, wybierz pozycję Uprawnienia opcji , a następnie wybierz potrzebną opcję   >  ochrony.

- Aby **automatycznie szyfrować wszystkie** wiadomości e-mail wysyłane do określonych adresatów lub zewnętrznych organizacji partnerskich, musisz utworzyć regułę transportu poczty e-mail w centrum Exchange administracyjnym. Szczegółowe instrukcje znajdują się [w tym artykule pomocy technicznej.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

