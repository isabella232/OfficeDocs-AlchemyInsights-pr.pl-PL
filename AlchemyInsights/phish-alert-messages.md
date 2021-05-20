---
title: 2491 Alert o wiadomościach e-mail z zasad "Dostarczono informacje o wiadomościach phish z powodu zastąpienia dzierżawy lub użytkownika"
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
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544588"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="8077b-102">Alert w wiadomościach e-mail z zasad "Dostarczono informacje na temat informacji o wiadomościach na temat wiadomości e-mail z powodu zastąpienia dzierżawy lub użytkownika"</span><span class="sxs-lookup"><span data-stu-id="8077b-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="8077b-103">W dzierżawach usługi Microsoft Defender dla komputerów Office 365 P1 i P2 w dzierżawie zostały włączone domyślne zasady alertów o nazwie "Dostarczono phish z powodu zastąpienia dzierżawy"</span><span class="sxs-lookup"><span data-stu-id="8077b-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="8077b-104">Jeśli otrzymano ten alert, należy zbadać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="8077b-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="8077b-105">W komunikacie alertu kliknij pozycję **Wyświetl alert,** aby przejść do strony **Alerty** w Centrum & zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="8077b-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="8077b-106">Wybierz alert, aby wyświetlić opcję Wyświetl **listę wiadomości lub** Wyświetl wiadomości w **Eksploratorze**.</span><span class="sxs-lookup"><span data-stu-id="8077b-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="8077b-107">W obu tych opcjach znajdują się szczegóły wiadomości, w tym identyfikator wiadomości.</span><span class="sxs-lookup"><span data-stu-id="8077b-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="8077b-108">Link Eksplorator zagrożeń automatycznie filtruje wiadomości zgodne z kryteriami alertu.</span><span class="sxs-lookup"><span data-stu-id="8077b-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="8077b-109">Może być konieczne dostosowanie filtru daty w Eksploratorze zagrożeń.</span><span class="sxs-lookup"><span data-stu-id="8077b-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="8077b-110">Wiadomość wyłudzająca informacje została dostarczona z powodu ręcznie skonfigurowanego zastąpienia:</span><span class="sxs-lookup"><span data-stu-id="8077b-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="8077b-111">Dozwolony nadawca lub domena ustawione przez użytkownika.</span><span class="sxs-lookup"><span data-stu-id="8077b-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="8077b-112">Dozwolony nadawca lub domena określone przez administratora w zasadach ochrony przed spamem.</span><span class="sxs-lookup"><span data-stu-id="8077b-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="8077b-113">Dozwolony adres IP w zasadach filtru połączenia.</span><span class="sxs-lookup"><span data-stu-id="8077b-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="8077b-114">Reguła przepływu poczty e-mail (znana również jako reguła transportu), która jest skonfigurowana do zezwalania na przychodzące wiadomości.</span><span class="sxs-lookup"><span data-stu-id="8077b-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="8077b-115">Jeśli uważasz, że wiadomość została niepoprawnie oznaczona jako phish, użyj dodatku Outlook [Report Message](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) (Wiadomość raportu) w celu przesłania przykładowych wiadomości do firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8077b-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
