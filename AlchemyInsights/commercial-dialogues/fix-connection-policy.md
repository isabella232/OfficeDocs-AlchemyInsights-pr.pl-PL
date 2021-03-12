---
title: Naprawianie zasad połączenia
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750605"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="dc4b6-102">Naprawianie zasad połączenia</span><span class="sxs-lookup"><span data-stu-id="dc4b6-102">Fix connection policy</span></span>

<span data-ttu-id="dc4b6-103">Wiadomość e-mail została oznaczona jako bezpieczna i dostarczona do skrzynki odbiorczej użytkownika, ponieważ wysyłający adres IP został oznaczony jako bezpieczny w zasadach Filtr połączenia.</span><span class="sxs-lookup"><span data-stu-id="dc4b6-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="dc4b6-104">Aby przejrzeć zasady, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="dc4b6-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="dc4b6-105">Przejdź do Centrum zabezpieczeń [usługi Office 365 &](https://go.microsoft.com/fwlink/p/?linkid=2077143) zgodności , a następnie przejdź do strony Ochrona przed spamem przy zasadach zarządzania  >    >  [zagrożeniami.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="dc4b6-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="dc4b6-106">Na karcie **Niestandardowe** wybierz zasady **filtru połączenia**, a następnie wybierz pozycję **Edytuj zasady**.</span><span class="sxs-lookup"><span data-stu-id="dc4b6-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="dc4b6-107">Przejrzyj listę **adresów IP Allow (Zezwalaj).**</span><span class="sxs-lookup"><span data-stu-id="dc4b6-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="dc4b6-108">Sprawdź, czy **jest włączona lista** bezpiecznych adresów.</span><span class="sxs-lookup"><span data-stu-id="dc4b6-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="dc4b6-109">Firma Microsoft subskrybuje zewnętrzne źródła zaufanych nadawców.</span><span class="sxs-lookup"><span data-stu-id="dc4b6-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="dc4b6-110">Jeśli **jest włączona** lista Bezpieczne, zaufani nadawcy nie są omyłnie oznaczani jako spam.</span><span class="sxs-lookup"><span data-stu-id="dc4b6-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="dc4b6-111">Zalecam zaznaczenie tej opcji, ponieważ spowoduje to zmniejszenie liczby odbieranych wyników fałszywie dodatnich (good mail, które są klasyfikowane jako spam).</span><span class="sxs-lookup"><span data-stu-id="dc4b6-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
