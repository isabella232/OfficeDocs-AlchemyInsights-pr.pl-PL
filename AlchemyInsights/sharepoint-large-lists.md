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
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Praca z dużymi listami i bibliotekami w programie SharePoint

Listy i biblioteki programu SharePoint mogą zawierać nawet 30 000 000 elementów, ale jeśli mają więcej niż 5 000 elementy, podczas próby współpracy z nimi może zostać wyświetlony błąd progu widoku listy. Zadaniem tego progu jest utrzymanie wydajności usługi. Nie można go zmienić. Aby uniknąć wymuszania tego progu:

**Użyj nowoczesnego**

Widoki przedstawiające wiele elementów działają najlepiej w nowoczesnych doświadczeniach. [Korzystaj z nowoczesnego środowiska,](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) aby uniknąć błędów, które mogą pojawić się w klasycznym środowisku.

**Dodawanie indeksów**

Podczas filtrowania lub sortowania według kolumny, która nie ma indeksu, może zostać wyświetlony komunikat o błędzie. Ręcznie [Dodaj indeks](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) z obszaru **Ustawienia listy** w menu Ustawienia, a następnie pozycję **indeksowane kolumny**.

**Edytowanie widoku listy**

Jeśli podczas pracy z dużą listą wystąpi błąd, [Edytuj widok listy](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).

Poniższe cztery zmiany spowodują usunięcie błędów progu widoku listy. Wprowadź wszystkie cztery zmiany, aby usunąć wszystkie błędy. Jeśli nadal pojawiają się błędy, sprawdź, czy jest polecenie [Zarządzaj dużymi listami i bibliotekami](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).

1. Wybierz pozycję **Brak** z obu **pierwszych Sortuj według kolumny** , a **następnie Sortuj według kolumny**.
2. Wybierz pozycję **Brak** z **pierwszej grupy według kolumny** , a **następnie Grupuj według kolumny**.
3. Wybierz pozycję **Brak** dla wszystkich kolumn w sekcji **sumy** .
4. Usuń zaznaczenie opcji wszystkie oprócz jednej kolumny do wyświetlenia w sekcji **kolumny** .

