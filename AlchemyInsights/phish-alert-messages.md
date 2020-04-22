---
title: 2491 Alert wiadomości e-mail z "Phish dostarczone z powodu dzierżawy lub zastąpienia użytkownika" zasady
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758939"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="7a8ca-102">Alert wiadomości e-mail z "Phish dostarczone z powodu dzierżawy lub zastąpienia użytkownika" zasady</span><span class="sxs-lookup"><span data-stu-id="7a8ca-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="7a8ca-103">Domyślna zasada alertów o nazwie "Phish delivered due to tenant or user override" została wdrożona dla dzierżaw z licencjami Office 365 ATP P1 i P2.</span><span class="sxs-lookup"><span data-stu-id="7a8ca-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="7a8ca-104">Jeśli ten alert został odebrany, oto kroki, które należy zbadać:</span><span class="sxs-lookup"><span data-stu-id="7a8ca-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="7a8ca-105">W komunikacie alertu kliknij pozycję **Wyświetl alert,** aby przejść do strony **Alerty** w Centrum zgodności & zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="7a8ca-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="7a8ca-106">Wybierz alert, aby wyświetlić opcję **Wyświetl listę wiadomości** lub Wyświetl wiadomości w **Eksploratorze**.</span><span class="sxs-lookup"><span data-stu-id="7a8ca-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="7a8ca-107">Obie te opcje przejmują cię do szczegółów wiadomości, która zawiera identyfikator wiadomości.</span><span class="sxs-lookup"><span data-stu-id="7a8ca-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="7a8ca-108">Należy zauważyć, że łącze Eksploratora zagrożeń będzie automatycznie filtrować wiadomości zgodne z kryteriami alertu.</span><span class="sxs-lookup"><span data-stu-id="7a8ca-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="7a8ca-109">Może być konieczne dostosowanie filtru daty w Eksploratorze zagrożeń.</span><span class="sxs-lookup"><span data-stu-id="7a8ca-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="7a8ca-110">Wiadomość wyłudzająca informacje została dostarczona z powodu ręcznie skonfigurowanego zastąpienia:</span><span class="sxs-lookup"><span data-stu-id="7a8ca-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="7a8ca-111">Dozwolony nadawca lub domena ustawiona przez użytkownika.</span><span class="sxs-lookup"><span data-stu-id="7a8ca-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="7a8ca-112">Dozwolony nadawca lub domena ustawiona przez administratora w zasadach antyspamowych.</span><span class="sxs-lookup"><span data-stu-id="7a8ca-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="7a8ca-113">Dozwolony adres IP w zasadach filtrowania połączeń.</span><span class="sxs-lookup"><span data-stu-id="7a8ca-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="7a8ca-114">Reguła przepływu poczty (znana również jako reguła transportu), która jest skonfigurowana tak, aby zezwalać na wysyłanie wiadomości.</span><span class="sxs-lookup"><span data-stu-id="7a8ca-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="7a8ca-115">Jeśli uważasz, że wiadomość została niepoprawnie oznaczona jako phish, użyj [dodatku Wiadomości raportu](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) programu Outlook, aby przesłać przykłady wiadomości do firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7a8ca-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
