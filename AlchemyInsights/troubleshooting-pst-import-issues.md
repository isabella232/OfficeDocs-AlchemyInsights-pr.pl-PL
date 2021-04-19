---
title: Rozwiązywanie problemów z importowaniem pliku PST
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826173"
---
# <a name="troubleshooting-pst-import-issues"></a>Rozwiązywanie problemów z importowaniem pliku PST

- Jeśli importujesz bezpośrednio w kliencie programu Outlook, zobacz [Rozwiązywanie problemów z importowaniem pliku pst programu Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Jeśli używasz usługi importowania i usługa ta zatrzymuje się, pamiętaj, że rozmiar każdego pliku PST przekazywanego do lokalizacji usługi Azure Storage nie powinien być większy niż 20 GB. Pliki PST, których rozmiar jest większy niż 20 GB mogą wpływać na poprawność działania procesu importowania pliku PST.

- Jeśli chcesz sprawdzić stan określonego zadania importu, możesz użyć [Get-MailboxImportRequest-batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Aby uzyskać szczegółowe informacje o usłudze importowania, zobacz [Omówienie importowania plików PST organizacji](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
