---
title: Problem z otwieraniem lub pobieraniem plików w usłudze Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148336"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Problem z otwieraniem lub pobieraniem plików w usłudze Yammer

Usługa Classic Yammer obsługuje wiele opcji przekazywania plików do wiadomości i grup. W zależności od konfiguracji sieci pliki domyślnie mają miejsce przechowywania w programie SharePoint.

Selektor plików w nowym usłudze Yammer nie obsługuje jeszcze wszystkich opcji dostępnych w klasycznym usłudze Yammer. Przyszła aktualizacja doda dodatkowe funkcje. Aby uzyskać więcej informacji, zobacz [Dołączanie pliku lub obrazu do posta konwersacji usługi Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Nie można otworzyć lub pobrać pliku**  

Plik może zostać przekazany do usługi Yammer, ale także łączyć się z plikiem w usłudze SharePoint Online. Aby rozwiązać problem, należy najpierw określić lokalizację pliku. Jeśli plik został przekazany do usługi Yammer, będzie miał *.yammer.com adres URL. Upewnij się, że wymagane adresy URL i adresy IP są odblokowane. Aby uzyskać więcej informacji, zobacz wpis w blogu [Używanie zakodowanych na czas adresów IP usługi Yammer nie jest zalecane.](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)

Sprawdź, czy użytkownik, który jest również administratorem globalnym, może pobrać plik. Jeśli plik jest prywatny, może być trzeba użyć trybu zawartości prywatnej. Aby uzyskać więcej informacji, zobacz następnie [monitorowanie zawartości prywatnej w usłudze Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Goście i pliki na poziomie sieci Yammer w usłudze SharePoint Online**  

[Goście na poziomie sieci w usłudze Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) nie korzystają z usługi Azure AD B2B i są wewnętrzni usługi Yammer, więc nie mogą uzyskać dostępu do plików usługi Yammer przechowywanych w programie SharePoint. Utwórz zewnętrznego użytkownika usługi AAD B2B, który może uzyskiwać dostęp do bibliotek dokumentów w usłudze SharePoint Online przy użyciu tej tożsamości. Aby uzyskać informacje na temat przyszłej obsługi gości usługi Azure AD B2B w usłudze Yammer, zobacz [Obsługa gościa między przedsiębiorstwami (B2B) w usłudze Yammer Preview — warunki dla klientów i często zadawane pytania](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).