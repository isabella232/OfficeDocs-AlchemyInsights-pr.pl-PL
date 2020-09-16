---
title: S/MIME w aplikacji Outlook w sieci Web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772308"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="ec051-102">Szyfrowanie wiadomości e-mail w programie Outlook</span><span class="sxs-lookup"><span data-stu-id="ec051-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="ec051-103">Szyfrowanie wiadomości programu Microsoft 365 jest oparte na usłudze Microsoft Azure Rights Management (Azure RMS), która jest częścią funkcji Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="ec051-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="ec051-104">Jeśli Twój abonament obejmuje usługę Azure Rights Management lub ochrona informacji o platformie Azure, **nie musisz podejmować żadnych działań w celu ręcznego włączenia lub aktywowania** usługi zarządzania prawami.</span><span class="sxs-lookup"><span data-stu-id="ec051-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="ec051-105">Na podstawie opinii klientów nie będzie już można włączać reguł przepływu poczty e-mail programu Exchange w celu automatycznego szyfrowania poczty e-mail, w której domyślnie jest określony rodzaj poufnych informacji.</span><span class="sxs-lookup"><span data-stu-id="ec051-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="ec051-106">Zamiast tego udostępniamy szczegółowe instrukcje, jak to zrobić yourselves.</span><span class="sxs-lookup"><span data-stu-id="ec051-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="ec051-107">Aby uzyskać dodatkowe informacje na temat tworzenia reguły transportu w celu zaszyfrowania poufnych informacji, zobacz [ten artykuł](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="ec051-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="ec051-108">Jeśli korzystasz z aplikacji Outlook w sieci Web (dawniej **owa**): podczas redagowania wiadomości e-mail wystarczy kliknąć pozycję **Chroń** w programie OWA.</span><span class="sxs-lookup"><span data-stu-id="ec051-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="ec051-109">To będzie miało zastosowanie uprawnienie "nie przekazuj".</span><span class="sxs-lookup"><span data-stu-id="ec051-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="ec051-110">Kliknij pozycję **Zmień uprawnienie** i wybierz pozycję **Szyfruj** , aby tylko zaszyfrować wiadomość.</span><span class="sxs-lookup"><span data-stu-id="ec051-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="ec051-111">Jeśli używasz **klienta programu Outlook**: aby wysłać zaszyfrowaną wiadomość z programu Outlook 2013 lub 2016 lub Outlook 2016 dla komputerów Mac, wybierz pozycję **Opcje**  >  **uprawnień**, a następnie wybierz odpowiednią opcję ochrony.</span><span class="sxs-lookup"><span data-stu-id="ec051-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="ec051-112">Aby **automatycznie szyfrować wszystkie wiadomości e-mail** wysyłane do określonych adresatów lub zewnętrznych organizacji partnerów, należy utworzyć regułę transportu przepływu poczty w centrum administracyjnym programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec051-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="ec051-113">Szczegółowe instrukcje znajdują się w [tym artykule pomocy technicznej](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="ec051-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

