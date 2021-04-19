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
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="4e69b-102">Rozwiązywanie problemów z uwierzytelnianiem SMTP</span><span class="sxs-lookup"><span data-stu-id="4e69b-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="4e69b-103">Jeśli podczas próby wysłania wiadomości e-mail SMTP i uwierzytelnienia w kliencie lub aplikacji występują błędy 5.7.57 lub 5.7.3, należy sprawdzić kilka czynności:</span><span class="sxs-lookup"><span data-stu-id="4e69b-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="4e69b-104">Uwierzytelnione przesyłanie SMTP może być wyłączone w dzierżawie lub w skrzynce pocztowej, z których próbujesz korzystać (sprawdź oba ustawienia).</span><span class="sxs-lookup"><span data-stu-id="4e69b-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="4e69b-105">Aby dowiedzieć się więcej, [zobacz Włączanie lub wyłączanie przesyłania SMTP uwierzytelnionego klienta.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)</span><span class="sxs-lookup"><span data-stu-id="4e69b-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="4e69b-106">Sprawdzanie, [czy dla dzierżawy](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) włączono ustawienia domyślne zabezpieczeń platformy Azure; Jeśli ta funkcja jest włączona, uwierzytelnianie SMTP przy użyciu uwierzytelniania podstawowego (znanego także jako starsze; spowoduje to użycie nazwy użytkownika i hasła) nie powiedzie się.</span><span class="sxs-lookup"><span data-stu-id="4e69b-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
