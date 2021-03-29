---
title: Sprawdzanie, czy adresy w skrzynkach pocztowych nie są przesyłane dalej
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403321"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="eb820-102">Sprawdzanie, czy adresy w skrzynkach pocztowych nie są przesyłane dalej</span><span class="sxs-lookup"><span data-stu-id="eb820-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="eb820-103">Czasami hakerzy przesyłają dalej wiadomości e-mail użytkowników do siebie, dlatego najpierw sprawdzimy, czy adresy i reguły nie są przekazywane w skrzynce pocztowej.</span><span class="sxs-lookup"><span data-stu-id="eb820-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="eb820-104">Następnie sprawdzimy dzienniki inspekcji.</span><span class="sxs-lookup"><span data-stu-id="eb820-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="eb820-105">Oto jak sprawdzić, czy adresy są przekazywane dalej:</span><span class="sxs-lookup"><span data-stu-id="eb820-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="eb820-106">Wybierz **pozycję Użytkownicy**  >  **Aktywni użytkownicy.**</span><span class="sxs-lookup"><span data-stu-id="eb820-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="eb820-107">Wybierz użytkownika, którego konto zostało naruszone.</span><span class="sxs-lookup"><span data-stu-id="eb820-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="eb820-108">W wyświetlonym wysuwaniu **rozwiń** pozycję Ustawienia poczty , a następnie kliknij **pozycję Edytuj dla** ustawienia Przesyłanie dalej wiadomości **e-mail.**</span><span class="sxs-lookup"><span data-stu-id="eb820-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="eb820-109">Usuń wszystkie adresy, których nie rozpoznajesz.</span><span class="sxs-lookup"><span data-stu-id="eb820-109">Remove any forwarding addresses you don't recognize.</span></span>