---
title: S/MIME w aplikacji Outlook w sieci Web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511518"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="9da6b-102">Szyfrowanie wiadomości e-mail w programie Outlook</span><span class="sxs-lookup"><span data-stu-id="9da6b-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="9da6b-103">Szyfrowanie wiadomości usługi Microsoft 365 jest oparte na usłudze Microsoft Azure Rights Management (Azure RMS), która jest częścią usługi Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="9da6b-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="9da6b-104">Jeśli subskrypcja obejmuje usługę Azure Rights Management lub usługę Azure Information Protection, **nie trzeba podejmować żadnych działań w celu ręcznego włączenia lub aktywowania** usługi zarządzania prawami.</span><span class="sxs-lookup"><span data-stu-id="9da6b-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="9da6b-105">Na podstawie opinii klientów nie będziemy już domyślnie włączać reguł przepływu poczty programu Exchange do automatycznego szyfrowania wychodzących wiadomości e-mail zawierających określony typ poufnych informacji w dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="9da6b-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="9da6b-106">Zamiast tego dostarczamy szczegółowe instrukcje, w jaki sposób możecie to zrobić sami.</span><span class="sxs-lookup"><span data-stu-id="9da6b-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="9da6b-107">Aby uzyskać dodatkowe informacje dotyczące tworzenia reguły transportu w celu szyfrowania poufnych informacji, zobacz [ten artykuł](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="9da6b-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="9da6b-108">Jeśli korzystasz z aplikacji Outlook w sieci Web (dawniej **OWA):** Podczas redagowania wiadomości e-mail po prostu kliknij przycisk **Chroń** w programie OWA.</span><span class="sxs-lookup"><span data-stu-id="9da6b-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="9da6b-109">Będzie to dotyczyć uprawnienia "Nie przesyłaj dalej".</span><span class="sxs-lookup"><span data-stu-id="9da6b-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="9da6b-110">Kliknij **pozycję Zmień uprawnienie** i wybierz pozycję **Szyfruj,** aby zaszyfrować tylko wiadomość.</span><span class="sxs-lookup"><span data-stu-id="9da6b-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="9da6b-111">Jeśli używasz **klienta programu Outlook:** Aby wysłać zaszyfrowaną wiadomość z programu Outlook 2013 lub 2016 lub programu Outlook 2016 dla komputerów Mac, wybierz pozycję Uprawnienia **opcji**, a następnie  >  **Permissions**wybierz potrzebną opcję ochrony.</span><span class="sxs-lookup"><span data-stu-id="9da6b-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="9da6b-112">Aby **automatycznie zaszyfrować wszystkie wiadomości e-mail** wysyłane do określonych adresatów lub zewnętrznych organizacji partnerskich, należy utworzyć regułę transportu przepływu poczty w Centrum administracyjnym programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="9da6b-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="9da6b-113">Szczegółowe instrukcje znajdują się w [tym artykule pomocy technicznej](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="9da6b-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

