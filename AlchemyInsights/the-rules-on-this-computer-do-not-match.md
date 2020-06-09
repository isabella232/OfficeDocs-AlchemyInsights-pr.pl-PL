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
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/09/2020
ms.locfileid: "44618023"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="3be38-102">Błąd: reguły na tym komputerze nie są zgodne</span><span class="sxs-lookup"><span data-stu-id="3be38-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="3be38-103">Aby zobaczyć zaktualizowany stan tego znanego problemu, zobacz [Reguły na tym komputerze nie są zgodne z regułami programu Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="3be38-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="3be38-104">Zespół programu Outlook zaimplementował poprawkę w kompilacji 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="3be38-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="3be38-105">Poprawka jest już w Insider Fast i trafi do Miesięcznego Kanału pod koniec czerwca 2020.</span><span class="sxs-lookup"><span data-stu-id="3be38-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="3be38-106">Po uzyskaniu stałej kompilacji możesz po raz ostatni otrzymać monit "Które reguły chcesz zachować".</span><span class="sxs-lookup"><span data-stu-id="3be38-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="3be38-107">Wybierz pozycję Serwer po wyświetleniu monitu, a następnie wróć do programu Outlook i ponownie włącz wszystkie wyłączone reguły.</span><span class="sxs-lookup"><span data-stu-id="3be38-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="3be38-108">Dopóki poprawka nie będzie dostępna, użyj następującego obejścia:</span><span class="sxs-lookup"><span data-stu-id="3be38-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="3be38-109">**Obejście**: W ostatnich raportach wystąpił problem dla tych, którzy utworzyli tylko reguły klienta na pulpicie programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="3be38-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="3be38-110">Jeśli nadal występuje problem, należy rozważyć usunięcie reguł, a następnie utworzyć i edytować reguły tylko w programie OWA (Outlook Web App) do momentu rozwiązania problemu.</span><span class="sxs-lookup"><span data-stu-id="3be38-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="3be38-111">Jeśli nie można usunąć reguł ręcznie, możesz uruchomić polecenie programu Outlook po uruchomieniu programu Outlook, uruchamiając program Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="3be38-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="3be38-112">Spowoduje to usunięcie reguł klienta i serwera.</span><span class="sxs-lookup"><span data-stu-id="3be38-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="3be38-113">Spowoduje to usunięcie wszystkich reguł dla wszystkich kont w profilu programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="3be38-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="3be38-114">To polecenie jest dodatkowo udokumentowane w artykule Przełączniki wiersza polecenia.</span><span class="sxs-lookup"><span data-stu-id="3be38-114">This command is further documented in the Command-line switches  article.</span></span>