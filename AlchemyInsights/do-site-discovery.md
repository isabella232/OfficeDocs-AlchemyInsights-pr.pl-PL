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
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694562"
---
# <a name="do-site-discovery"></a>Odnajdowanie witryn

Jeśli Twoja organizacja nadal używa starszych aplikacji sieci Web i planuje korzystać z trybu programu Internet Explorer (co robi większość klientów), należy wykonać dodatkowe odnajdowanie witryn.

**Wdrożono już starszą wersję przeglądarki Microsoft Edge**

Jeśli lista witryn przedsiębiorstwa została już skonfigurowana do działania w starszej wersji przeglądarki Microsoft Edge, odnajdowanie witryn jest prawie gotowe. Jedną z rzeczy, które może być konieczne, jest dodanie witryn neutralnych.

Witryny neutralne to zazwyczaj witryny, które zapewniają logowanie jednokrotne. Jeśli przejdź do witryny neutralnej z programu Microsoft Edge, chcesz pozostać w programie Microsoft Edge w celu uwierzytelnienia. Jeśli przejdźsz do witryny neutralnej w trybie programu Internet Explorer, chcesz pozostać w trybie programu Internet Explorer w celu uwierzytelnienia.

Zidentyfikuj wszelkie logowania jednokrotne lub inne witryny neutralne, z których korzystasz, i dodaj je do listy witryn przedsiębiorstwa.

**Program Internet Explorer jest domyślną przeglądarką**

Jeśli teraz korzystasz tylko z programu Internet Explorer, być może nie wiesz, które witryny uaktualniły się do nowoczesnych standardów sieci Web, a które nadal wymagają programu Internet Explorer. Warto znaleźć te witryny i dodać je do listy witryn przedsiębiorstwa, aby można było używać trybu programu Internet Explorer tylko dla tych witryn.

> [!NOTE]
> [Odnajdowanie witryn przedsiębiorstwa](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) wykrywa witryny, które mogą wymagać trybu programu Internet Explorer. Może zbierać dane na komputerach z systemem Windows Internet Explorer 8 za pośrednictwem programu Internet Explorer 11 w systemie Windows 10, Windows 8.1 lub Windows 7.

**Analizowanie danych**

Po zebraniu danych witryny zalecamy, aby w celu ich przeanalizowania był następujący proces czteroetapowy:
1. Sortuj dane według domeny, a następnie według adresu URL.
2. Zdefiniuj granice aplikacji, aby skonfigurować tryb programu Internet Explorer. Chcesz uwzględnić wszystkie witryny i kontrolki sieci Web definiujące aplikację, ale nie chcesz uwzględniać dodatkowych witryn i kontrolek. Niektóre witryny mogą być tak proste, jak *https://contoso.com/app1* inne mogą wymagać zdefiniowania wielu witryn i stron.
3. Przetestuj aplikację, aby sprawdzić, czy nie działa natywnie. Wiele witryn oferuje nowoczesną zawartość po wykryciu nowoczesnej przeglądarki i oferuje starszą zawartość tylko wtedy, gdy wykryje program Internet Explorer.
4. Dodaj aplikację do listy witryn przedsiębiorstwa, jeśli testy nie powiedzie się.

> [!NOTE]
> Najlepszym rozwiązaniem jest pogrupowanie wszystkich witryn składających się na aplikację. Dzięki temu podczas uaktualniania aplikacji łatwiej będzie usunąć całą witrynę z trybu programu Internet Explorer i rozpocząć korzystanie z nowoczesnej przeglądarki dla tej aplikacji.

Po zakończeniu odnajdowania witryn i przeanalizowaniu danych możesz zacząć analizować strategię kanału.

