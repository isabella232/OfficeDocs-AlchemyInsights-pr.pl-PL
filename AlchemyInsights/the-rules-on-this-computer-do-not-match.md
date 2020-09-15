---
title: 'Błąd: reguły na tym komputerze nie pasują do siebie.'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690973"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="0d193-102">Błąd: reguły na tym komputerze nie pasują do siebie.</span><span class="sxs-lookup"><span data-stu-id="0d193-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="0d193-103">Aby wyświetlić zaktualizowany stan tego znanego problemu, zobacz [reguły na tym komputerze są niezgodne z regułami w programie Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="0d193-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="0d193-104">Zespół programu Outlook zaimplementował poprawkę w kompilacji 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="0d193-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="0d193-105">Poprawka jest już w Niejawnym programie testów i będzie przełączana do kanału miesięcznego po późnych 2020 czerwca.</span><span class="sxs-lookup"><span data-stu-id="0d193-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="0d193-106">Po utworzeniu stałej kompilacji możesz wyświetlić monit "które reguły chcesz zachować" po raz ostatni.</span><span class="sxs-lookup"><span data-stu-id="0d193-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="0d193-107">Wybierz pozycję serwer po wyświetleniu monitu, a następnie wróć do programu Outlook i ponownie Włącz wszystkie reguły, które zostały wyłączone.</span><span class="sxs-lookup"><span data-stu-id="0d193-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="0d193-108">Dopóki poprawka nie będzie dostępna, użyj następującego obejścia:</span><span class="sxs-lookup"><span data-stu-id="0d193-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="0d193-109">**Obejście**: w przypadku ostatnich raportów wystąpił problem dotyczący utworzonych tylko reguł klientów w aplikacji klasycznej Outlook.</span><span class="sxs-lookup"><span data-stu-id="0d193-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="0d193-110">Jeśli problem nadal występuje, warto usunąć reguły, a następnie utworzyć i edytować reguły tylko w aplikacji OWA (Outlook Web App) do momentu rozwiązania problemu.</span><span class="sxs-lookup"><span data-stu-id="0d193-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="0d193-111">Jeśli nie można usunąć reguł ręcznie, możesz uruchomić polecenie programu Outlook po uruchomieniu programu Outlook, uruchamiając Outlook.exe/cleanrules.</span><span class="sxs-lookup"><span data-stu-id="0d193-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="0d193-112">Spowoduje to usunięcie zarówno reguł klienta, jak i serwera.</span><span class="sxs-lookup"><span data-stu-id="0d193-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="0d193-113">Spowoduje to usunięcie wszystkich reguł dla wszystkich kont w profilu programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="0d193-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="0d193-114">To polecenie jest dokładniej opisane w artykule przełączniki wiersza polecenia.</span><span class="sxs-lookup"><span data-stu-id="0d193-114">This command is further documented in the Command-line switches article.</span></span>

