---
title: Rozwiązywanie problemów z uwierzytelnianiem SMTP
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
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826425"
---
# <a name="solving-smtp-authentication-issues"></a>Rozwiązywanie problemów z uwierzytelnianiem SMTP

Jeśli podczas próby wysłania wiadomości e-mail SMTP i uwierzytelnienia w kliencie lub aplikacji występują błędy 5.7.57 lub 5.7.3, należy sprawdzić kilka czynności:

- Uwierzytelnione przesyłanie SMTP może być wyłączone w dzierżawie lub w skrzynce pocztowej, z których próbujesz korzystać (sprawdź oba ustawienia). Aby dowiedzieć się więcej, [zobacz Włączanie lub wyłączanie przesyłania SMTP uwierzytelnionego klienta.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)

- Sprawdzanie, [czy dla dzierżawy](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) włączono ustawienia domyślne zabezpieczeń platformy Azure; Jeśli ta funkcja jest włączona, uwierzytelnianie SMTP przy użyciu uwierzytelniania podstawowego (znanego także jako starsze; spowoduje to użycie nazwy użytkownika i hasła) nie powiedzie się.
