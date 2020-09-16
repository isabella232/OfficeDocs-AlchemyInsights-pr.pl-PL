---
title: Zapisywanie witryny lub listy jako szablonu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727541"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="6c271-102">Zapisywanie witryny lub listy jako szablonu</span><span class="sxs-lookup"><span data-stu-id="6c271-102">Save site or list as a template</span></span>

<span data-ttu-id="6c271-103">Szablony witryn programu SharePoint są wstępnie zbudowanymi definicjami zaprojektowanymi wokół konkretnych potrzeb biznesowych.</span><span class="sxs-lookup"><span data-stu-id="6c271-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="6c271-104">Aby uzyskać więcej informacji, zobacz [Tworzenie różnych rodzajów witryn programu SharePoint za pomocą szablonów](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="6c271-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="6c271-105">Poniżej przedstawiono kilka typowych problemów i rozwiązań dotyczących zapisywania witryny lub listy jako szablonu w usłudze SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="6c271-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="6c271-106">**Przycisk Zapisz szablon witryny/listy nie jest dostępny lub brakuje**go.</span><span class="sxs-lookup"><span data-stu-id="6c271-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="6c271-107">Aby umożliwić administratorom niestandardowym Włączanie funkcji szablonu, Administratorzy muszą zezwolić na używanie skryptu niestandardowego.</span><span class="sxs-lookup"><span data-stu-id="6c271-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="6c271-108">Aby uzyskać szczegółowe instrukcje, przykłady i zagadnienia, zobacz [Zezwalanie lub zapobieganie skryptowi niestandardowemu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="6c271-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="6c271-109">Polecenie Zapisz witrynę jako szablon nie jest obsługiwane i może powodować problemy z witrynami korzystającymi z infrastruktury publikowania w programie SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="6c271-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="6c271-110">**Nie można utworzyć szablonu witryny lub nie działa on poprawnie**</span><span class="sxs-lookup"><span data-stu-id="6c271-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="6c271-111">W szablonie może brakować [funkcji](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i nie można jej aktywować.</span><span class="sxs-lookup"><span data-stu-id="6c271-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="6c271-112">Jeśli ta funkcja nie jest dostępna do aktywacji w bieżącym zbiorze witryn, nie można utworzyć witryny przy użyciu szablonu witryny.</span><span class="sxs-lookup"><span data-stu-id="6c271-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="6c271-113">Sprawdź, czy jakieś listy lub biblioteki nie przekraczają [progu limitów widoku listy](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) dla 5000 elementów, ponieważ może blokować Tworzenie szablonu witryny.</span><span class="sxs-lookup"><span data-stu-id="6c271-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="6c271-114">Witryna może używać zbyt wielu zasobów, więc szablon witryny przekracza limit 50 megabajtów (MB).</span><span class="sxs-lookup"><span data-stu-id="6c271-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="6c271-115">Występują problemy z wyświetlaniem danych z listy używającej kolumny odnośnika.</span><span class="sxs-lookup"><span data-stu-id="6c271-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="6c271-116">Aby uzyskać więcej informacji, zobacz [Lista wygenerowana przez szablony nie wyświetla danych z odpowiedniej listy odnośników w usłudze SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="6c271-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="6c271-117">Aby uzyskać bardziej szczegółowe informacje o typowych problemach i rozwiązaniach, zobacz [Tworzenie i używanie szablonów witryn](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="6c271-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

