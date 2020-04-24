---
title: Przekazywanie wiadomości e-mail przez platformę Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 4b36caf1841c5292d269812f4ab5ca16a46fbc81
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785205"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="79207-102">Konfiguracja urządzenia wielofunkcyjnego lub aplikacji do wysyłania wiadomości e-mail</span><span class="sxs-lookup"><span data-stu-id="79207-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="79207-103">Aby poznać dostępne opcje i instrukcje, zobacz [Jak skonfigurować urządzenie wielofunkcyjne lub aplikację do wysyłania wiadomości e-mail przy użyciu platformy Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span><span class="sxs-lookup"><span data-stu-id="79207-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span></span>
  
<span data-ttu-id="79207-104">**Uwaga:** Jeśli Twoje urządzenie lub aplikacja ostatnio przestały działać, informujemy, że zgodnie z planem rozpoczęliśmy [wyłączanie szyfrowania 3DES](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="79207-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="79207-105">Aby wyświetlić urządzenia, na których występuje problem, przejdź do [raportu Klienci uwierzytelniania SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="79207-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="79207-106">Typowe błędy mogą wyglądać tak, jak te: Błąd uwierzytelniania, Błąd TLS, Błąd algorytmu szyfrowania, Niedopasowanie algorytmów lub Przerwane połączenie.</span><span class="sxs-lookup"><span data-stu-id="79207-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="79207-107">Aby rozwiązać problem:</span><span class="sxs-lookup"><span data-stu-id="79207-107">To resolve the issue:</span></span>
 - <span data-ttu-id="79207-108">**Windows Server 2003 IIS SMTP nie będzie już dłużej działać. Wymagana jest nowsza wersja systemu Windows.**</span><span class="sxs-lookup"><span data-stu-id="79207-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="79207-109">Sprawdź w aplikacji lub u dostawcy urządzenia, czy obsługiwany jest nowoczesny mechanizm szyfrowania lub czy jest dostępna aktualizacja.</span><span class="sxs-lookup"><span data-stu-id="79207-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
