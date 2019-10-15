---
title: Duże listy programu SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488527"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="688f7-102">Praca z dużymi list i bibliotek w programie SharePoint</span><span class="sxs-lookup"><span data-stu-id="688f7-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="688f7-103">Listy programu SharePoint i bibliotek może zawierać maksymalnie 30 000 000 elementów, ale gdy mają więcej niż 5 000 elementów, może zostać wyświetlony próg widoku listy błąd podczas próby pracy z nimi.</span><span class="sxs-lookup"><span data-stu-id="688f7-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="688f7-104">Próg ten jest w miejscu, aby utrzymać wydajność usługi.</span><span class="sxs-lookup"><span data-stu-id="688f7-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="688f7-105">Nie można go zmienić.</span><span class="sxs-lookup"><span data-stu-id="688f7-105">It can't be changed.</span></span> <span data-ttu-id="688f7-106">Aby uniknąć uderzenia w ten próg:</span><span class="sxs-lookup"><span data-stu-id="688f7-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="688f7-107">**Korzystaj z nowoczesnych**</span><span class="sxs-lookup"><span data-stu-id="688f7-107">**Use modern**</span></span>

<span data-ttu-id="688f7-108">Widoki przedstawiające wiele elementów działają najlepiej w nowoczesnym doświadczeniu.</span><span class="sxs-lookup"><span data-stu-id="688f7-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="688f7-109">[Korzystaj z nowoczesnych doświadczeń](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) , aby uniknąć błędów, które mogą być widoczne w klasycznym doświadczeniu.</span><span class="sxs-lookup"><span data-stu-id="688f7-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="688f7-110">**Dodawanie indeksów**</span><span class="sxs-lookup"><span data-stu-id="688f7-110">**Add indexes**</span></span>

<span data-ttu-id="688f7-111">Podczas filtrowania lub sortowania według kolumny, która nie ma indeksu, może zostać wyświetlony komunikat o błędzie.</span><span class="sxs-lookup"><span data-stu-id="688f7-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="688f7-112">[Dodaj indeks](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) ręcznie z **Ustawienia listy** w menu ustawień, a następnie **kolumny indeksowane**.</span><span class="sxs-lookup"><span data-stu-id="688f7-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="688f7-113">**Edycja widoku listy**</span><span class="sxs-lookup"><span data-stu-id="688f7-113">**Edit the list view**</span></span>

<span data-ttu-id="688f7-114">Jeśli wystąpi błąd podczas pracy z dużą listą, [Edytuj widok listy](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="688f7-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="688f7-115">Następujące cztery zmiany usunie błędy próg widoku listy.</span><span class="sxs-lookup"><span data-stu-id="688f7-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="688f7-116">Dokonaj wszystkich czterech zmian, aby usunąć wszystkie błędy.</span><span class="sxs-lookup"><span data-stu-id="688f7-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="688f7-117">Jeśli nadal otrzymujesz błędy, sprawdź [Zarządzaj dużymi listami i bibliotekami](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="688f7-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="688f7-118">Wybierz opcję **Brak** z obu **pierwszego sortowania według kolumny** , a **następnie Sortuj według kolumny**.</span><span class="sxs-lookup"><span data-stu-id="688f7-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="688f7-119">Wybierz **Brak** z obu **pierwszej grupy przez kolumnę** , a **następnie Grupuj według kolumny**.</span><span class="sxs-lookup"><span data-stu-id="688f7-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="688f7-120">Wybierz opcję **Brak** dla wszystkich kolumn w sekcji **sumy** .</span><span class="sxs-lookup"><span data-stu-id="688f7-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="688f7-121">Odznacz wszystkie oprócz jednej kolumny do wyświetlenia w sekcji **kolumny** .</span><span class="sxs-lookup"><span data-stu-id="688f7-121">Deselect all but one column for display from the **Columns** section.</span></span>

