---
title: 'Błąd: reguły na tym komputerze nie są zgodne'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664256"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="d5710-102">Błąd: reguły na tym komputerze nie są zgodne</span><span class="sxs-lookup"><span data-stu-id="d5710-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="d5710-103">Aby zobaczyć zaktualizowany stan tego znanego problemu, zobacz [Reguły na tym komputerze nie są zgodne z regułami programu Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="d5710-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="d5710-104">Zespół programu Outlook zaimplementował poprawkę w kompilacji 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="d5710-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="d5710-105">Poprawka jest już w Insider Fast i trafi do Miesięcznego Kanału pod koniec czerwca 2020.</span><span class="sxs-lookup"><span data-stu-id="d5710-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="d5710-106">Po uzyskaniu stałej kompilacji możesz po raz ostatni otrzymać monit "Które reguły chcesz zachować".</span><span class="sxs-lookup"><span data-stu-id="d5710-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="d5710-107">Wybierz pozycję Serwer po wyświetleniu monitu, a następnie wróć do programu Outlook i ponownie włącz wszystkie wyłączone reguły.</span><span class="sxs-lookup"><span data-stu-id="d5710-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="d5710-108">Dopóki poprawka nie będzie dostępna, użyj następującego obejścia:</span><span class="sxs-lookup"><span data-stu-id="d5710-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="d5710-109">**Obejście**: W ostatnich raportach wystąpił problem dla tych, którzy utworzyli tylko reguły klienta na pulpicie programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="d5710-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="d5710-110">Jeśli nadal występuje problem, należy rozważyć usunięcie reguł, a następnie utworzyć i edytować reguły tylko w programie OWA (Outlook Web App) do momentu rozwiązania problemu.</span><span class="sxs-lookup"><span data-stu-id="d5710-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="d5710-111">Jeśli nie można usunąć reguł ręcznie, możesz uruchomić polecenie programu Outlook po uruchomieniu programu Outlook, uruchamiając program Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="d5710-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="d5710-112">Spowoduje to usunięcie reguł klienta i serwera.</span><span class="sxs-lookup"><span data-stu-id="d5710-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="d5710-113">Spowoduje to usunięcie wszystkich reguł dla wszystkich kont w profilu programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="d5710-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="d5710-114">To polecenie jest dodatkowo udokumentowane w artykule Przełączniki wiersza polecenia.</span><span class="sxs-lookup"><span data-stu-id="d5710-114">This command is further documented in the Command-line switches article.</span></span>

