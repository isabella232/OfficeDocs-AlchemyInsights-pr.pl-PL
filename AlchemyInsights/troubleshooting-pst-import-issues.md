---
title: Rozwiązywanie problemów z importowaniem pliku PST
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 58fdd509fae5e87bf5ae72db5d8926c4367cdd64
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991375"
---
# <a name="troubleshooting-pst-import-issues"></a>Rozwiązywanie problemów z importowaniem pliku PST

- Jeśli importujesz bezpośrednio w kliencie programu Outlook, zobacz [Rozwiązywanie problemów z importowaniem pliku pst programu Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Jeśli używasz usługi importowania i usługa ta zatrzymuje się, pamiętaj, że rozmiar każdego pliku PST przekazywanego do lokalizacji usługi Azure Storage nie powinien być większy niż 20 GB. Pliki PST, których rozmiar jest większy niż 20 GB mogą wpływać na poprawność działania procesu importowania pliku PST.

- Jeśli chcesz sprawdzić stan określonego zadania importu, możesz użyć [Get-MailboxImportRequest-batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Aby uzyskać szczegółowe informacje o usłudze importowania, zobacz [Omówienie importowania plików PST organizacji](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
