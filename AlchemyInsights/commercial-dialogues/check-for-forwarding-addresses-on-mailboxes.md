---
title: Sprawdzanie, czy adresy w skrzynkach pocztowych nie są przesyłane dalej
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482778"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="fd89b-102">Sprawdzanie, czy adresy w skrzynkach pocztowych nie są przesyłane dalej</span><span class="sxs-lookup"><span data-stu-id="fd89b-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="fd89b-103">Czasami hakerzy przesyłają dalej wiadomości e-mail użytkowników do siebie, dlatego najpierw sprawdzamy, czy adresy i reguły w skrzynce pocztowej nie są przesyłane dalej.</span><span class="sxs-lookup"><span data-stu-id="fd89b-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="fd89b-104">Następnie sprawdzimy dzienniki inspekcji.</span><span class="sxs-lookup"><span data-stu-id="fd89b-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="fd89b-105">Oto jak sprawdzić, czy adresy są przekazywane dalej:</span><span class="sxs-lookup"><span data-stu-id="fd89b-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="fd89b-106">Wybierz **pozycję**  >  **Aktywni użytkownicy.**</span><span class="sxs-lookup"><span data-stu-id="fd89b-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="fd89b-107">Wybierz użytkownika, którego konto zostało naruszone.</span><span class="sxs-lookup"><span data-stu-id="fd89b-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="fd89b-108">W wyświetlonym wysuwaniu rozwiń pozycję **Ustawienia** poczty, a następnie kliknij pozycję **Edytuj** dla przesyłania **dalej wiadomości e-mail.**</span><span class="sxs-lookup"><span data-stu-id="fd89b-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="fd89b-109">Usuń wszystkie adresy przesyłania dalej, których nie rozpoznajesz.</span><span class="sxs-lookup"><span data-stu-id="fd89b-109">Remove any forwarding addresses you don't recognize.</span></span>