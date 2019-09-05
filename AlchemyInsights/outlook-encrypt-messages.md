---
title: S/MIME w programie Outlook w sieci Web
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752870"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="f3576-102">Szyfruj wiadomości e-mail w Outlooku</span><span class="sxs-lookup"><span data-stu-id="f3576-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="f3576-103">Szyfrowanie wiadomości pakietu Office 365 jest zbudowany na Microsoft Azure Rights Management (Azure RMS), który jest częścią usługi Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="f3576-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="f3576-104">Jeśli subskrypcja obejmuje usługę Azure Rights Management lub usługę Azure Information Protection, **nie trzeba podejmować żadnych działań, aby ręcznie włączyć lub aktywować** usługę zarządzania prawami dostępu.</span><span class="sxs-lookup"><span data-stu-id="f3576-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="f3576-105">Na podstawie opinii klientów nie będzie już włączania reguł przepływu poczty programu Exchange do automatycznego szyfrowania wychodzących wiadomości e-mail zawierających określony typ poufnych informacji w dzierżawie domyślnie.</span><span class="sxs-lookup"><span data-stu-id="f3576-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="f3576-106">Zamiast tego, zapewniamy szczegółowe instrukcje, jak można to zrobić sami.</span><span class="sxs-lookup"><span data-stu-id="f3576-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="f3576-107">Aby uzyskać dodatkowe informacje dotyczące sposobu tworzenia reguły transportu do szyfrowania poufnych informacji, zobacz w [tym artykule](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="f3576-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="f3576-108">Jeśli korzystasz z programu Outlook w sieci Web (dawniej **owa**): podczas tworzenia wiadomości e-mail, po prostu kliknij przycisk **Chroń** w programie OWA.</span><span class="sxs-lookup"><span data-stu-id="f3576-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="f3576-109">Spowoduje to zastosowanie uprawnienia "nie przesyłam dalej".</span><span class="sxs-lookup"><span data-stu-id="f3576-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="f3576-110">Kliknij opcję **Zmień uprawnienie** i \*\*\*\* wybierz opcję Szyfruj, aby zaszyfrować tylko wiadomość.</span><span class="sxs-lookup"><span data-stu-id="f3576-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="f3576-111">W przypadku korzystania z **klienta programu Outlook**: aby wysłać zaszyfrowaną wiadomość z programu Outlook 2013 lub 2016 lub Outlook 2016 dla komputerów Macintosh **, wybierz opcję** > **uprawnienia**, a następnie wybierz opcję ochrony, której potrzebujesz.</span><span class="sxs-lookup"><span data-stu-id="f3576-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="f3576-112">Aby **automatycznie szyfrować wszystkie wiadomości e-mail** wysłane do określonych adresatów lub zewnętrznych organizacji partnerskich, należy utworzyć regułę transportu przepływu poczty w centrum administracyjnego programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="f3576-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="f3576-113">Szczegółowe instrukcje podano w [tym artykule pomocy technicznej](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="f3576-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

