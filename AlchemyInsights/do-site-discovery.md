---
title: Odnajdowanie witryn
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: 4653fdef7e9226f05809d56e9a445cd1da35b0578c088bea72252a281d4527d2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030768"
---
# <a name="do-site-discovery"></a>Odnajdowanie witryn

Jeśli Twoja organizacja nadal używa starszych aplikacji i planów sieci Web korzystających z trybu programu Internet Explorer (co robi większość klientów), musisz wykonać dodatkowe odnajdowanie witryn.

**Wcześniej wdrożono starszą wersję pakietu Microsoft Edge**

Jeśli masz już skonfigurowaną listę witryn Enterprise do działania dla starszej wersji programu Microsoft Edge, odnajdowanie witryn jest prawie gotowe. Jedną z rzeczy, które może być konieczne, jest dodanie witryn neutralnych.

Witryny neutralne to zazwyczaj witryny, które zapewniają logowanie jednokrotne. Jeśli przejdźsz do witryny neutralnej z Microsoft Edge, chcesz pozostać w Microsoft Edge uwierzytelnienia. Jeśli w trybie programu Internet Explorer przejdźsz do witryny neutralnej, chcesz pozostać w trybie programu Internet Explorer, aby uwierzytelnić.

Zidentyfikuj wszelkie logowania jednokrotne lub inne witryny neutralne, z których korzystasz, i dodaj je Enterprise do listy witryn.

**Program Internet Explorer jest domyślną przeglądarką**

Jeśli teraz używasz tylko programu Internet Explorer, być może nie wiesz, które witryny zostały uaktualnione do nowoczesnych standardów sieci Web, a które nadal wymagają programu Internet Explorer. Trzeba znaleźć te witryny i dodać je do listy witryn programu Enterprise, aby można było używać trybu programu Internet Explorer tylko dla tych witryn.

> [!NOTE]
> [Enterprise odnajdowania](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) witryn wykrywa witryny, które mogą wymagać trybu programu Internet Explorer. Może zbierać dane na komputerach z systemem Windows Internet Explorer od 8 do Internet Explorer 11 na komputerze z systemem Windows 10, Windows 8.1 lub Windows 7.

**Analizowanie danych**

Po zebraniu danych dotyczących witryny zalecamy skorzystanie z czterech kroków procesu analizy danych:
1. Dane można sortować według domeny, a następnie według adresu URL.
2. Definiowanie granic aplikacji w celu skonfigurowania trybu programu Internet Explorer. Chcesz uwzględnić wszystkie witryny i kontrolki sieci Web definiujące aplikację, ale nie chcesz uwzględniać dodatkowych witryn i kontrolek. Niektóre witryny mogą być tak proste, jak inne mogą *https://contoso.com/app1* wymagać zdefiniowania wielu witryn i stron.
3. Przetestuj aplikację, aby sprawdzić, czy nie działa natywnie. Wiele witryn oferuje nowoczesną zawartość, gdy wykryje nowoczesną przeglądarkę, i będzie oferować starszą zawartość tylko wtedy, gdy wykryje program Internet Explorer.
4. Dodaj aplikację do listy witryn Enterprise w przypadku niepowodzenia testowania.

> [!NOTE]
> Najlepszym rozwiązaniem jest pogrupowanie wszystkich witryn składających się na aplikację. Dzięki temu podczas uaktualniania aplikacji łatwiej jest usunąć całą witrynę z trybu programu Internet Explorer i zacząć korzystać z nowoczesnej przeglądarki dla tej aplikacji.

Po zakończeniu odnajdowania witryny i przeanalizowaniu danych możesz zacząć szukać strategii dotyczącej kanału.

