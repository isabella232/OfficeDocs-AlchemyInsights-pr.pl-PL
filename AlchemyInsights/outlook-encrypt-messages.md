---
title: S/MIME w aplikacji Outlook w sieci Web
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
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772308"
---
# <a name="encrypt-email-messages-in-outlook"></a>Szyfrowanie wiadomości e-mail w programie Outlook

Szyfrowanie wiadomości programu Microsoft 365 jest oparte na usłudze Microsoft Azure Rights Management (Azure RMS), która jest częścią funkcji Azure Information Protection. Jeśli Twój abonament obejmuje usługę Azure Rights Management lub ochrona informacji o platformie Azure, **nie musisz podejmować żadnych działań w celu ręcznego włączenia lub aktywowania** usługi zarządzania prawami.

Na podstawie opinii klientów nie będzie już można włączać reguł przepływu poczty e-mail programu Exchange w celu automatycznego szyfrowania poczty e-mail, w której domyślnie jest określony rodzaj poufnych informacji. Zamiast tego udostępniamy szczegółowe instrukcje, jak to zrobić yourselves. Aby uzyskać dodatkowe informacje na temat tworzenia reguły transportu w celu zaszyfrowania poufnych informacji, zobacz [ten artykuł](https://aka.ms/OmeEtr).

- Jeśli korzystasz z aplikacji Outlook w sieci Web (dawniej **owa**): podczas redagowania wiadomości e-mail wystarczy kliknąć pozycję **Chroń** w programie OWA. To będzie miało zastosowanie uprawnienie "nie przekazuj". Kliknij pozycję **Zmień uprawnienie** i wybierz pozycję **Szyfruj** , aby tylko zaszyfrować wiadomość.

- Jeśli używasz **klienta programu Outlook**: aby wysłać zaszyfrowaną wiadomość z programu Outlook 2013 lub 2016 lub Outlook 2016 dla komputerów Mac, wybierz pozycję **Opcje**  >  **uprawnień**, a następnie wybierz odpowiednią opcję ochrony.

- Aby **automatycznie szyfrować wszystkie wiadomości e-mail** wysyłane do określonych adresatów lub zewnętrznych organizacji partnerów, należy utworzyć regułę transportu przepływu poczty w centrum administracyjnym programu Exchange. Szczegółowe instrukcje znajdują się w [tym artykule pomocy technicznej](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

