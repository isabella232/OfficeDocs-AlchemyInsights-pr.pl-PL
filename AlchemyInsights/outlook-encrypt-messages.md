---
title: S/MIME w programie Outlook w sieci Web
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752870"
---
# <a name="encrypt-email-messages-in-outlook"></a>Szyfruj wiadomości e-mail w Outlooku

Szyfrowanie wiadomości pakietu Office 365 jest zbudowany na Microsoft Azure Rights Management (Azure RMS), który jest częścią usługi Azure Information Protection. Jeśli subskrypcja obejmuje usługę Azure Rights Management lub usługę Azure Information Protection, **nie trzeba podejmować żadnych działań, aby ręcznie włączyć lub aktywować** usługę zarządzania prawami dostępu.

Na podstawie opinii klientów nie będzie już włączania reguł przepływu poczty programu Exchange do automatycznego szyfrowania wychodzących wiadomości e-mail zawierających określony typ poufnych informacji w dzierżawie domyślnie. Zamiast tego, zapewniamy szczegółowe instrukcje, jak można to zrobić sami. Aby uzyskać dodatkowe informacje dotyczące sposobu tworzenia reguły transportu do szyfrowania poufnych informacji, zobacz w [tym artykule](https://aka.ms/OmeEtr).

- Jeśli korzystasz z programu Outlook w sieci Web (dawniej **owa**): podczas tworzenia wiadomości e-mail, po prostu kliknij przycisk **Chroń** w programie OWA. Spowoduje to zastosowanie uprawnienia "nie przesyłam dalej". Kliknij opcję **Zmień uprawnienie** i **** wybierz opcję Szyfruj, aby zaszyfrować tylko wiadomość.

- W przypadku korzystania z **klienta programu Outlook**: aby wysłać zaszyfrowaną wiadomość z programu Outlook 2013 lub 2016 lub Outlook 2016 dla komputerów Macintosh **, wybierz opcję** > **uprawnienia**, a następnie wybierz opcję ochrony, której potrzebujesz.

- Aby **automatycznie szyfrować wszystkie wiadomości e-mail** wysłane do określonych adresatów lub zewnętrznych organizacji partnerskich, należy utworzyć regułę transportu przepływu poczty w centrum administracyjnego programu Exchange. Szczegółowe instrukcje podano w [tym artykule pomocy technicznej](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

