---
title: Rozwiązywanie problemów z zadaniem usługi importowania nie rozwiązało problemu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125489"
---
# <a name="troubleshooting-import-service-job-stuck"></a>Rozwiązywanie problemów z zadaniem usługi importowania nie rozwiązało problemu

Jeśli występują problemy z importowaniem zadań usługi utknęły lub się nie powiedają, sprawdź i wypróbuj następujące czynności:

- Sprawdź rozmiar pliku PST. Maksymalny rozmiar pliku PST zalecany w przypadku importowania wynosi 20 GB.

- Jeśli podejrzewasz, że pominięte elementy są pomijane z powodu uszkodzenia, uruchom Scanpst.exe, aby zdiagnozować i naprawić błędy w plikach PST.

- Jeśli podczas importowania zostanie wyświetlony błąd "MapiExceptionShutoffQuotaExceeded", upewnij się, że docelowa skrzynka pocztowa ma wystarczająco dużo pojemności, aby zaimportować odpowiednie pliki PST.

Aby uzyskać więcej informacji na temat rozwiązywania problemów z zadaniami importu plików PST, zobacz [Rozwiązywanie problemów z zadaniami importu pliku PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

Aby uzyskać informacje o tym, jak rozwiązać problemy podczas importowania plików PST do programu Outlook, zobacz Rozwiązywanie problemów z importowaniem pliku [pst programu Outlook (microsoft.com).](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)