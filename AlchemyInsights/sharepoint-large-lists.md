---
title: Duże listy programu SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720143"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="c9570-102">Praca z dużymi listami i bibliotekami w programie SharePoint</span><span class="sxs-lookup"><span data-stu-id="c9570-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="c9570-103">Listy i biblioteki programu SharePoint mogą zawierać nawet 30 000 000 elementów, ale jeśli mają więcej niż 5 000 elementy, podczas próby współpracy z nimi może zostać wyświetlony błąd progu widoku listy.</span><span class="sxs-lookup"><span data-stu-id="c9570-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="c9570-104">Zadaniem tego progu jest utrzymanie wydajności usługi.</span><span class="sxs-lookup"><span data-stu-id="c9570-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="c9570-105">Nie można go zmienić.</span><span class="sxs-lookup"><span data-stu-id="c9570-105">It can't be changed.</span></span> <span data-ttu-id="c9570-106">Aby uniknąć wymuszania tego progu:</span><span class="sxs-lookup"><span data-stu-id="c9570-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="c9570-107">**Użyj nowoczesnego**</span><span class="sxs-lookup"><span data-stu-id="c9570-107">**Use modern**</span></span>

<span data-ttu-id="c9570-108">Widoki przedstawiające wiele elementów działają najlepiej w nowoczesnych doświadczeniach.</span><span class="sxs-lookup"><span data-stu-id="c9570-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="c9570-109">[Korzystaj z nowoczesnego środowiska,](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) aby uniknąć błędów, które mogą pojawić się w klasycznym środowisku.</span><span class="sxs-lookup"><span data-stu-id="c9570-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="c9570-110">**Dodawanie indeksów**</span><span class="sxs-lookup"><span data-stu-id="c9570-110">**Add indexes**</span></span>

<span data-ttu-id="c9570-111">Podczas filtrowania lub sortowania według kolumny, która nie ma indeksu, może zostać wyświetlony komunikat o błędzie.</span><span class="sxs-lookup"><span data-stu-id="c9570-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="c9570-112">Ręcznie [Dodaj indeks](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) z obszaru **Ustawienia listy** w menu Ustawienia, a następnie pozycję **indeksowane kolumny**.</span><span class="sxs-lookup"><span data-stu-id="c9570-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="c9570-113">**Edytowanie widoku listy**</span><span class="sxs-lookup"><span data-stu-id="c9570-113">**Edit the list view**</span></span>

<span data-ttu-id="c9570-114">Jeśli podczas pracy z dużą listą wystąpi błąd, [Edytuj widok listy](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="c9570-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="c9570-115">Poniższe cztery zmiany spowodują usunięcie błędów progu widoku listy.</span><span class="sxs-lookup"><span data-stu-id="c9570-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="c9570-116">Wprowadź wszystkie cztery zmiany, aby usunąć wszystkie błędy.</span><span class="sxs-lookup"><span data-stu-id="c9570-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="c9570-117">Jeśli nadal pojawiają się błędy, sprawdź, czy jest polecenie [Zarządzaj dużymi listami i bibliotekami](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="c9570-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="c9570-118">Wybierz pozycję **Brak** z obu **pierwszych Sortuj według kolumny** , a **następnie Sortuj według kolumny**.</span><span class="sxs-lookup"><span data-stu-id="c9570-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="c9570-119">Wybierz pozycję **Brak** z **pierwszej grupy według kolumny** , a **następnie Grupuj według kolumny**.</span><span class="sxs-lookup"><span data-stu-id="c9570-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="c9570-120">Wybierz pozycję **Brak** dla wszystkich kolumn w sekcji **sumy** .</span><span class="sxs-lookup"><span data-stu-id="c9570-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="c9570-121">Usuń zaznaczenie opcji wszystkie oprócz jednej kolumny do wyświetlenia w sekcji **kolumny** .</span><span class="sxs-lookup"><span data-stu-id="c9570-121">Deselect all but one column for display from the **Columns** section.</span></span>

