---
title: Program Project Online jest w stanie tylko do odczytu
ms.author: pebaum
author: pebaum
manager: pamg
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1776"
- "9000205"
ms.openlocfilehash: ad2a9f95bf30708772edb166945f3f42e0f1f503
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801662"
---
# <a name="project-online-is-in-a-read-only-state"></a><span data-ttu-id="e539e-102">Program Project Online jest w stanie tylko do odczytu</span><span class="sxs-lookup"><span data-stu-id="e539e-102">Project Online is in a read-only state</span></span>

<span data-ttu-id="e539e-103">Istnieją trzy typowe powody, dla których program Project Online może uzyskać stan tylko do odczytu:</span><span class="sxs-lookup"><span data-stu-id="e539e-103">There are three common reasons why Project Online may reach a read-only state:</span></span>

1. <span data-ttu-id="e539e-104">Organizacje mają tylko licencje usługi Project Online Essentials.</span><span class="sxs-lookup"><span data-stu-id="e539e-104">Organizations have a Project Online Essentials license(s) only.</span></span> <span data-ttu-id="e539e-105">To nie wystarczy, aby utrzymać stan aktywności witryny, a po pewnym czasie zostanie zainicjowana obsługa administracyjna.</span><span class="sxs-lookup"><span data-stu-id="e539e-105">This isn't enough to keep the site alive and it will eventually get de-provisioned.</span></span><span data-ttu-id="e539e-106">Witryna jest umieszczana w stanie tylko do odczytu, aby administratorzy wiedzieli, że coś jest niewłaściwa i może uzyskać prawidłowe licencje.</span><span class="sxs-lookup"><span data-stu-id="e539e-106"> We place the site in a read-only state so that Admins know something is wrong and can acquire the correct licenses.</span></span> <span data-ttu-id="e539e-107">Administratorzy będą musieli dodać licencję usługi Project Online Professional i/lub Premium.</span><span class="sxs-lookup"><span data-stu-id="e539e-107">Admins will need to add a Project Online Professional and/or Premium license.</span></span> <span data-ttu-id="e539e-108">W tym momencie witryna znajdzie się w trybie tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="e539e-108">The site will come out of read-only at that point.</span></span> <span data-ttu-id="e539e-109">Aby uzyskać więcej informacji, zobacz [porównanie rozwiązań zarządzania projektami](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span><span class="sxs-lookup"><span data-stu-id="e539e-109">For more info, see [Compare Project Management Solutions](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span></span>
2. <span data-ttu-id="e539e-110">Osiągnięto przypisany przydział.</span><span class="sxs-lookup"><span data-stu-id="e539e-110">Assigned quota has been reached.</span></span> <span data-ttu-id="e539e-111">Aby uzyskać więcej informacji, zobacz [przydział aplikacji Project Web App](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span><span class="sxs-lookup"><span data-stu-id="e539e-111">For more info, see [Project Web App Quota](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span></span> <span data-ttu-id="e539e-112">Zaznacz pole wyboru [Konfiguruj zbiorcze dane raportowania danych w usłudze Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) , aby zobaczyć, jak ziarnistość raportowania może wpływać na użycie przydziału.</span><span class="sxs-lookup"><span data-stu-id="e539e-112">Check [Configure rollup of timephased reporting data in Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) to see how reporting granularity may impact quota usage.</span></span>
3. <span data-ttu-id="e539e-113">Stan tylko do odczytu może być bardzo tymczasowym warunkiem, który może wystąpić podczas konserwacji.</span><span class="sxs-lookup"><span data-stu-id="e539e-113">Read-only can be a very temporary condition that can occur during maintenance.</span></span> <span data-ttu-id="e539e-114">Większość obsługi nie jest jeszcze zauważalna przez naszych klientów i nie jest to często widoczne, ale istnieją czasy, w których wystąpią krótkie okresy tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="e539e-114">Most maintenance is not even noticed by our customers and you will not often see this, but there are times when short periods of read-only are experienced.</span></span>
