---
title: Wiele obiektów ma ten sam adres e-mail co tożsamość
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439715"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Wiele obiektów ma ten sam adres e-mail co tożsamość

**Wiele obiektów**

Jedną z typowych przyczyn tego błędu jest nie jest możliwe do routowania żądania programu Outlook Web Access poprawnie w obecności wielu obiektów o tym samym adresie e-mail jako tożsamości. Aby znaleźć te obiekty, uruchom następujące polecenia:

· Odbiorca pobierz<email address>

· Pobierz użytkownika<email address>

· Get-User <email address> -SoftDeletedUżytnik

· Kontakt z użytkownikami<email address>

· Get-Mailbox <email address> -PublicFolder

· Get-Skrzynka pocztowa <email address> -IncludeSoftDeletedMailbox

· Get-Skrzynka pocztowa <email address> -Nieaktywna skrzynka pocztowaTylko

Aby rozwiązać ten problem, usuń wiele obiektów o tej samej tożsamości poczty e-mail i upewnij się, że istnieje pojedynczy obiekt o określonej tożsamości wiadomości e-mail i że jego typem adresata jest UserMailbox.

**Ten sam adres jest używany w skrzynkach pocztowych firm i konsumentów**

Inną przyczyną jest, gdy ten sam adres jest używany dla skrzynek pocztowych firmy i konsumentów. W takim przypadku użytkownik musi zmienić swój podstawowy alias konsumenta, dopóki Cafe obsługuje ten scenariusz. Jest to trwały błąd, który nie zniknie bez interwencji.

Aby uzyskać szczegółowe informacje, zobacz [Zmienianie adresu e-mail lub numeru telefonu konta Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).