---
title: MC210173 — wycofanie nowej niestandardowej funkcji formularza programu SharePoint Designer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 185e8fc94345b240667490b1ffc63af8459d8daf
ms.sourcegitcommit: a9e6b2fcce8bd12fd079ed967f426b67d5c6d239
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/28/2020
ms.locfileid: "43928537"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="bb1d8-102">MC210173 — wycofanie nowej niestandardowej funkcji formularza programu SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="bb1d8-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="bb1d8-103">Zidentyfikowaliśmy problem wpływającym na funkcjonalność programu SharePoint Designer dla [tworzenia formularzy niestandardowych](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) w usłudze SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="bb1d8-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="bb1d8-104">Po przeprowadzeniu starannej analizy stwierdziliśmy, że nie ma znanych poprawek dla tego problemu i postanowiliśmy wyłączyć funkcję tworzenia formularzy niestandardowych o godzinie 3:00 (czasu UTC) w sobotę 25 kwietnia 2020 r.</span><span class="sxs-lookup"><span data-stu-id="bb1d8-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="bb1d8-105">Ta zmiana nie ma wpływu na możliwość edytowania wcześniej utworzonych formularzy ani innych istniejących funkcji w usłudze SharePoint Online Designer.</span><span class="sxs-lookup"><span data-stu-id="bb1d8-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="bb1d8-106">Po wprowadzeniu tej zmiany użytkownicy mogli otrzymać błąd: „Nie można zapisać zmian na liście na serwerze” podczas tworzenia nowych formularzy.</span><span class="sxs-lookup"><span data-stu-id="bb1d8-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="bb1d8-107">Użytkownicy, którzy wcześniej korzystali z programu SharePoint Designer do tworzenia formularzy niestandardowych, mogą użyć do tego celu usługi [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form).</span><span class="sxs-lookup"><span data-stu-id="bb1d8-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="bb1d8-108">Usługa PowerApps to łatwe w użyciu zaawansowane narzędzie pozwalające użytkownikom pracującym w środowisku SharePoint Online Modern tworzyć i edytować niestandardowe formularze dla list programu SharePoint i bibliotek dokumentów bezpośrednio z okna przeglądarki.</span><span class="sxs-lookup"><span data-stu-id="bb1d8-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="bb1d8-109">Usługa PowerApps nie wymaga znajomości tradycyjnego kodowania ani pobierania żadnych dodatkowych aplikacji, takich jak program InfoPath.</span><span class="sxs-lookup"><span data-stu-id="bb1d8-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="bb1d8-110">**Uwaga**: użytkownicy usługi SharePoint Online Classic będą musieli chwilowo przełączać się do nowoczesnego środowiska, aby uzyskać dostęp do usługi PowerApps i korzystać z niej. Chociaż wszystkie formularze niestandardowe utworzone w usłudze PowerApps są dostępne dla doświadczonych użytkowników usługi SharePoint Online w wersji klasycznej.</span><span class="sxs-lookup"><span data-stu-id="bb1d8-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
