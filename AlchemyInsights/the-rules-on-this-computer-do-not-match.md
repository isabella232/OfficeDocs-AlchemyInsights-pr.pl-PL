---
title: 'Błąd: Reguły na tym komputerze nie są zgodne'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782962"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="e75b4-102">Błąd: Reguły na tym komputerze nie są zgodne</span><span class="sxs-lookup"><span data-stu-id="e75b4-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="e75b4-103">Aby wyświetlić zaktualizowany stan tego znanego problemu, zobacz Reguły na tym komputerze nie są zgodne z [regułami w programie Microsoft Exchange.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="e75b4-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="e75b4-104">Zespół programu Outlook zaimplementował poprawkę w kompilacji 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="e75b4-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="e75b4-105">Poprawka jest już dostępna w niejawnym programie testów w szybkich wersjach i trafi do kanału miesięcznego pod koniec czerwca 2020 r.</span><span class="sxs-lookup"><span data-stu-id="e75b4-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="e75b4-106">Po naprawieniu kompilacji może ostatni raz zostać wyświetlony monit "Które reguły chcesz zachować".</span><span class="sxs-lookup"><span data-stu-id="e75b4-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="e75b4-107">Po wyświetleniu monitu wybierz pozycję Serwer, a następnie wróć do programu Outlook i ponownie włącz reguły, które zostały wyłączone.</span><span class="sxs-lookup"><span data-stu-id="e75b4-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="e75b4-108">Do czasu, aż poprawka będzie dostępna, użyj następującego obejścia:</span><span class="sxs-lookup"><span data-stu-id="e75b4-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="e75b4-109">**Obejście:** W ostatnich raportach problem pojawił się u tych osób, które tylko tworzyły reguły klienta w klasycznej wersji programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="e75b4-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="e75b4-110">Jeśli problem nadal występuje, rozważ usunięcie reguł, a następnie utworzenie i edytowanie reguł tylko w aplikacji OWA (Outlook Web App), dopóki problem nie zostanie rozwiązany.</span><span class="sxs-lookup"><span data-stu-id="e75b4-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="e75b4-111">Jeśli nie możesz ręcznie usunąć reguł, możesz uruchomić polecenie programu Outlook podczas uruchamiania programu Outlook, uruchamiając polecenie Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="e75b4-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="e75b4-112">Spowoduje to usunięcie zarówno reguł klienta, jak i reguł serwera.</span><span class="sxs-lookup"><span data-stu-id="e75b4-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="e75b4-113">Spowoduje to usunięcie wszystkich reguł dla wszystkich kont w profilu programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="e75b4-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="e75b4-114">To polecenie jest dodatkowo udokumentowane w artykule Przełączniki wiersza polecenia.</span><span class="sxs-lookup"><span data-stu-id="e75b4-114">This command is further documented in the Command-line switches article.</span></span>

