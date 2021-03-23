---
title: Ochrona przed atakami backscatterów
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037185"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="b21bf-102">Ochrona przed atakami backscatterów</span><span class="sxs-lookup"><span data-stu-id="b21bf-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="b21bf-103">Wiadomość typu backscatter to raporty o niedo dostarczeniu (nazywane również raportami o niedo dostarczenia lub wiadomościami zwrotnych) o wiadomościach, które nie zostały wysłane przez Ciebie.</span><span class="sxs-lookup"><span data-stu-id="b21bf-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="b21bf-104">Spamerzy podszywają  się (fałszują) adresy od swoich wiadomości i często używają prawdziwych adresów e-mail do wiarygodności swoich wiadomości.</span><span class="sxs-lookup"><span data-stu-id="b21bf-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="b21bf-105">Dlatego w przypadku, gdy spamerzy trudno wysłać wiadomości do nieistniejących adresatów, docelowy serwer poczty e-mail w zasadzie ma mieć  kłopoty z zwróceniem nie można dostarczyć wiadomości w wiadomości o niedostarczeniu do nadawcy rozmytego w adresie Od.</span><span class="sxs-lookup"><span data-stu-id="b21bf-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="b21bf-106">Dodatkowe informacje można znaleźć w wiadomości [Backscatter w uciekaszem usługi EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)</span><span class="sxs-lookup"><span data-stu-id="b21bf-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="b21bf-107">**Włączanie ochrony backscatterów**</span><span class="sxs-lookup"><span data-stu-id="b21bf-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="b21bf-108">Aby włączyć ochronę backscatterów, postępuj zgodnie z instrukcjami poniżej.</span><span class="sxs-lookup"><span data-stu-id="b21bf-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="b21bf-109">**protection.office.com > zarządzanie zagrożeniami > > ochrony przed spamem > Wybierz właściwości Zasad filtru spamu i Edytuj zasady > Spam > Oznacz jako spam > wiadomość typu backscatter > Ustaw jako "Wł."**</span><span class="sxs-lookup"><span data-stu-id="b21bf-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="b21bf-110">Jeśli uważasz, że ktoś włamania na konto został naruszony, zobacz następujące informacje:</span><span class="sxs-lookup"><span data-stu-id="b21bf-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="b21bf-111">Odpowiadanie na naruszone konto e-mail</span><span class="sxs-lookup"><span data-stu-id="b21bf-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="b21bf-112">Usuwanie zablokowanych użytkowników z portalu Użytkownicy z ograniczeniami w usłudze Office 365</span><span class="sxs-lookup"><span data-stu-id="b21bf-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



