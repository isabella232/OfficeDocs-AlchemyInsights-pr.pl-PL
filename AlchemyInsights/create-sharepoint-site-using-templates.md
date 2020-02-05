---
title: Tworzenie witryny w usłudze SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770433"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="12d7d-102">Tworzenie witryn programu SharePoint przy użyciu szablonów</span><span class="sxs-lookup"><span data-stu-id="12d7d-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="12d7d-103">Możliwość zapisywania witryny jako szablonu nie jest obsługiwana w nowoczesnych witrynach komunikacyjnych lub zespołowych.</span><span class="sxs-lookup"><span data-stu-id="12d7d-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="12d7d-104">Aby uzyskać więcej informacji na temat używania szablonów, zobacz [Zapisywanie, pobieranie i przekazywanie witryny programu SharePoint jako szablonu](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="12d7d-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="12d7d-105">Oto kilka typowych problemów/rozwiązań dotyczących zapisywania witryny lub listy jako szablonu w usłudze Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="12d7d-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="12d7d-106">**Przycisk Zapisz szablon witryny/listy nie jest dostępny lub brakuje przycisku**</span><span class="sxs-lookup"><span data-stu-id="12d7d-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="12d7d-107">Administratorzy będą musieli zezwolić na skrypt niestandardowy, aby włączyć funkcje szablonu.</span><span class="sxs-lookup"><span data-stu-id="12d7d-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="12d7d-108">Szczegółowe kroki, przykłady i zagadnienia można znaleźć</span><span class="sxs-lookup"><span data-stu-id="12d7d-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="12d7d-109">Zezwalanie na skrypt niestandardowy lub zapobieganie mu</span><span class="sxs-lookup"><span data-stu-id="12d7d-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="12d7d-110">Polecenie Zapisz witrynę jako szablon nie jest obsługiwane i może powodować problemy w witrynach korzystających z infrastruktury publikowania programu SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="12d7d-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="12d7d-111">**Nie można utworzyć szablonu witryny lub nie działa poprawnie**</span><span class="sxs-lookup"><span data-stu-id="12d7d-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="12d7d-112">W szablonie może brakować [funkcji](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i nie zostanie uruchomiony.</span><span class="sxs-lookup"><span data-stu-id="12d7d-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="12d7d-113">Jeśli funkcja nie jest dostępna do aktywacji w bieżącym zbiorze witryn, nie można użyć szablonu witryny do utworzenia witryny.</span><span class="sxs-lookup"><span data-stu-id="12d7d-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="12d7d-114">Sprawdź, czy jakiekolwiek listy lub biblioteki przekraczają [próg limitu widoku listy](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 elementów, ponieważ może to blokować tworzenie szablonu witryny.</span><span class="sxs-lookup"><span data-stu-id="12d7d-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="12d7d-115">Lokacja może używać zbyt wielu zasobów i dlatego szablon witryny przekracza limit 50 MB.</span><span class="sxs-lookup"><span data-stu-id="12d7d-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="12d7d-116">Występują problemy z wyświetlaniem danych z listy, która używa kolumny odlotowej.</span><span class="sxs-lookup"><span data-stu-id="12d7d-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="12d7d-117">Aby uzyskać więcej informacji, zobacz [Lista wygenerowana przez szablon nie wyświetla danych z poprawnej listy odstawień w usłudze SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="12d7d-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="12d7d-118">Aby uzyskać bardziej szczegółowe informacje na temat typowych problemów i rozwiązań, zapoznaj się z [temattworzenia i używania szablonów witryn](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="12d7d-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



