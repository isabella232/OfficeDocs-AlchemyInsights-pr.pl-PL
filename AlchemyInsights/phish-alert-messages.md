---
title: Alert (2491) wiadomości e-mail z poziomu "phishing dostarczany z powodu zasad przesłonięcia dzierżawy lub użytkownika"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728621"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="ca4ef-102">Alarmowanie wiadomości e-mail z poziomu "phishing dostarczany z powodu zasad przesłonięcia dzierżawy lub użytkownika"</span><span class="sxs-lookup"><span data-stu-id="ca4ef-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="ca4ef-103">Domyślna zasada alertów o nazwie "wyłudzanie informacji została dostarczona z powodu przesłonięcia dzierżawy lub zastąpienia użytkownika" została przekazana do dzierżawców za pomocą licencji na usługi Office 365 ATP i P2.</span><span class="sxs-lookup"><span data-stu-id="ca4ef-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="ca4ef-104">Jeśli otrzymałeś ten alert, możesz sprawdzić następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="ca4ef-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="ca4ef-105">W oknie komunikatu alertu kliknij pozycję **Wyświetl alert** , aby przejść do strony **alerty** w centrum zabezpieczeń & zgodności.</span><span class="sxs-lookup"><span data-stu-id="ca4ef-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="ca4ef-106">Wybierz Alert, aby zobaczyć opcję **wyświetlania listy wiadomości** lub **wyświetlania wiadomości w Eksploratorze**.</span><span class="sxs-lookup"><span data-stu-id="ca4ef-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="ca4ef-107">W obu tych opcjach przedstawiono szczegóły wiadomości zawierającej identyfikator wiadomości.</span><span class="sxs-lookup"><span data-stu-id="ca4ef-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="ca4ef-108">Pamiętaj, że link w Eksploratorze zagrożeń będzie automatycznie filtrować wiadomości zgodne z kryteriami alertów.</span><span class="sxs-lookup"><span data-stu-id="ca4ef-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="ca4ef-109">Być może trzeba dostosować filtr daty w Eksploratorze zagrożeń.</span><span class="sxs-lookup"><span data-stu-id="ca4ef-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="ca4ef-110">Wiadomość wyłudzająca informacje została dostarczona z powodu ręcznej konfiguracji przesłonięcia:</span><span class="sxs-lookup"><span data-stu-id="ca4ef-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="ca4ef-111">Dozwolony nadawca lub domena ustawiona przez użytkownika.</span><span class="sxs-lookup"><span data-stu-id="ca4ef-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="ca4ef-112">Dozwolony nadawca lub domena ustawiona przez administratora w zasadach ochrony przed spamem.</span><span class="sxs-lookup"><span data-stu-id="ca4ef-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="ca4ef-113">Dozwolony adres IP w zasadach filtru połączeń.</span><span class="sxs-lookup"><span data-stu-id="ca4ef-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="ca4ef-114">Reguła przepływu poczty (nazywana też regułą transportu), która jest skonfigurowana do zezwalania na wiadomości.</span><span class="sxs-lookup"><span data-stu-id="ca4ef-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="ca4ef-115">Jeśli uważasz, że wiadomość została niepoprawnie oznaczona jako wyłudzanie informacji, użyj [dodatku wiadomości raportu](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) programu Outlook, aby przesłać próbki wiadomości do firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ca4ef-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
