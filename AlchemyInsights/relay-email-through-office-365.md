---
title: Przekazywanie wiadomości e-mail przez platformę Microsoft 365
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 56936541c52e56d7aa9b0f5dad7b9a359c5b6185
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809665"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="1a2e7-102">Konfiguracja urządzenia wielofunkcyjnego lub aplikacji do wysyłania wiadomości e-mail</span><span class="sxs-lookup"><span data-stu-id="1a2e7-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="1a2e7-103">Aby poznać dostępne opcje i instrukcje, zobacz [Jak skonfigurować urządzenie wielofunkcyjne lub aplikację do wysyłania wiadomości e-mail przy użyciu platformy Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="1a2e7-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="1a2e7-104">**Uwaga:** Jeśli Twoje urządzenie lub aplikacja ostatnio przestały działać, informujemy, że zgodnie z planem rozpoczęliśmy [wyłączanie szyfrowania 3DES](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="1a2e7-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="1a2e7-105">Aby wyświetlić urządzenia, na których występuje problem, przejdź do [raportu Klienci uwierzytelniania SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="1a2e7-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="1a2e7-106">Typowe błędy mogą wyglądać tak, jak te: Błąd uwierzytelniania, Błąd TLS, Błąd algorytmu szyfrowania, Niedopasowanie algorytmów lub Przerwane połączenie.</span><span class="sxs-lookup"><span data-stu-id="1a2e7-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="1a2e7-107">Aby rozwiązać problem:</span><span class="sxs-lookup"><span data-stu-id="1a2e7-107">To resolve the issue:</span></span>

 - <span data-ttu-id="1a2e7-108">**Windows Server 2003 IIS SMTP nie będzie już dłużej działać. Wymagana jest nowsza wersja systemu Windows.**</span><span class="sxs-lookup"><span data-stu-id="1a2e7-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="1a2e7-109">Sprawdź w aplikacji lub u dostawcy urządzenia, czy obsługiwany jest nowoczesny mechanizm szyfrowania lub czy jest dostępna aktualizacja.</span><span class="sxs-lookup"><span data-stu-id="1a2e7-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
