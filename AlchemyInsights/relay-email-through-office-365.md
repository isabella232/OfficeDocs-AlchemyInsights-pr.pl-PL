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
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117993"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="62f15-102">Konfiguracja urządzenia wielofunkcyjnego lub aplikacji do wysyłania wiadomości e-mail</span><span class="sxs-lookup"><span data-stu-id="62f15-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="62f15-103">Aby poznać dostępne opcje i instrukcje, zobacz [Jak skonfigurować urządzenie wielofunkcyjne lub aplikację do wysyłania wiadomości e-mail przy użyciu platformy Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="62f15-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="62f15-104">Jeśli masz urządzenie lub aplikację, która ostatnio przestała działać, najczęstszymi problemami są:</span><span class="sxs-lookup"><span data-stu-id="62f15-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="62f15-105">**Błędy związane z uwierzytelnianiem podczas korzystania z przesyłania klienta uwierzytelniania SMTP** Ostatnio wpisano pewne zmiany dotyczące działania uwierzytelniania SMTP.</span><span class="sxs-lookup"><span data-stu-id="62f15-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="62f15-106">Aby uzyskać więcej informacji na temat rozwiązywania problemów, zobacz sekcję rozwiązywanie problemów z uwierzytelnianiem za pomocą drukarki, skanerów i aplikacji biznesowych, które wysyłają wiadomości e-mail za pomocą programu Microsoft 365 lub [Office 365.](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)</span><span class="sxs-lookup"><span data-stu-id="62f15-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="62f15-107">Podczas bezpiecznego połączenia z internetem akceptujemy tylko wersję **TLS 1.2 Office 365** Jeśli korzystasz z bezpiecznego połączenia (TLS), upewnij się, że urządzenie aplikacji obsługuje TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="62f15-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="62f15-108">Aby uzyskać więcej informacji, zobacz Przygotowywanie się do [1.2 TLS](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)w programie Office 365 i Office 365 GCC.</span><span class="sxs-lookup"><span data-stu-id="62f15-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="62f15-109">Aby uzyskać informacje na temat innych problemów i ich rozwiązań, zobacz Rozwiązywanie problemów z drukarkami, skanerami i aplikacjami LOB, które wysyłają wiadomości [e-mail](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)przy użyciu Microsoft 365 lub Office 365.</span><span class="sxs-lookup"><span data-stu-id="62f15-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="62f15-110">Aby wyświetlić urządzenia, na których występuje problem, przejdź do [raportu Klienci uwierzytelniania SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="62f15-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="62f15-111">**Uwaga:** Exchange Online scenariuszy z wysyłką zbiorczą.</span><span class="sxs-lookup"><span data-stu-id="62f15-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="62f15-112">Aby wysyłać masową komercyjną pocztę e-mail (na przykład biuletyny klientów), należy używać innych dostawców oferowanych w tych usługach.</span><span class="sxs-lookup"><span data-stu-id="62f15-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
