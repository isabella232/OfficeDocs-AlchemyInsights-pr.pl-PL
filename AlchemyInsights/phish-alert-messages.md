---
title: Wiadomości e-mail alertu 2491 od wykrywanie witryn wyłudzających wydana z powodu dzierżawcę lub użytkownika zastępują zasady
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391436"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="7e990-102">Wiadomości e-mail alertu z wykrywanie witryn wyłudzających wydana z powodu dzierżawcę lub użytkownika zastępują zasady</span><span class="sxs-lookup"><span data-stu-id="7e990-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="7e990-103">Domyślna zasada alert o nazwie "Wykrywanie witryn wyłudzających dostarczone ze względu na zastąpienie dzierżawcę lub użytkownika" była dostępna dla najemców z licencjami Office 365 ATP P1 i P2.</span><span class="sxs-lookup"><span data-stu-id="7e990-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="7e990-104">Jeśli otrzymasz ten komunikat, Oto kroki, aby zbadać:</span><span class="sxs-lookup"><span data-stu-id="7e990-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="7e990-105">Z komunikatu alertu kliknij przycisk **Wyświetl Alert** , aby przejść do strony **alerty** zabezpieczeń & Centrum zgodności.</span><span class="sxs-lookup"><span data-stu-id="7e990-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="7e990-106">Wybierz ten alert, aby wyświetlić opcję na **liście wiadomości w widoku** lub **Wyświetlanie wiadomości w Eksploratorze**.</span><span class="sxs-lookup"><span data-stu-id="7e990-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="7e990-107">Obie te opcje przejście do szczegółów wiadomości, która zawiera identyfikator wiadomości.</span><span class="sxs-lookup"><span data-stu-id="7e990-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="7e990-108">Uwaga: łącze zagrożenie Explorer automatycznie przefiltruje wiadomości, które spełniają kryteria alertu.</span><span class="sxs-lookup"><span data-stu-id="7e990-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="7e990-109">Konieczne może być dostosowanie filtr daty w Eksploratorze zagrożenie.</span><span class="sxs-lookup"><span data-stu-id="7e990-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="7e990-110">Wiadomość wyłudzająca informacje została dostarczona z powodu override ręcznie skonfigurowane:</span><span class="sxs-lookup"><span data-stu-id="7e990-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="7e990-111">Dozwolone nadawcy lub domeny ustawiona przez użytkownika.</span><span class="sxs-lookup"><span data-stu-id="7e990-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="7e990-112">Dozwolonych nadawców lub domeny ustawiona przez administratora w zasadzie zwalczania spamu.</span><span class="sxs-lookup"><span data-stu-id="7e990-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="7e990-113">Dozwolony adres IP w zasadzie filtr połączeń.</span><span class="sxs-lookup"><span data-stu-id="7e990-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="7e990-114">Reguły przepływu poczty (znany również jako regułę transportu), która jest skonfigurowana do obsługi wiadomości w.</span><span class="sxs-lookup"><span data-stu-id="7e990-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="7e990-115">Jeśli uważasz, że wiadomość została niepoprawnie oznaczona jako pozyskiwać, użyj programu Outlook [dodatek wiadomość raportu](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) przedłożenia próbek wiadomości do firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7e990-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
