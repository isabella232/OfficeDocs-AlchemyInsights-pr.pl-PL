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
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059825"
---
# <a name="troubleshooting-pst-import-issues"></a>Rozwiązywanie problemów z importowaniem pliku PST

- Jeśli importujesz dane w obrębie samego klienta programu Outlook, zobacz Rozwiązywanie problemów z importowaniem pliku [pst programu Outlook.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)

- Jeśli korzystasz z usługi importowania i problem się zablokował, pamiętaj, że każdy plik PST, który przekażemy do lokalizacji magazynu platformy Azure, nie powinien być większy niż 20 GB. Pliki PST o rozmiarze większym niż 20 GB mogą mieć wpływ na wydajność procesu importowania pliku PST. Aby uzyskać więcej informacji dotyczących rozwiązywania problemów z zadaniami, które utknęły, zobacz [Problemy dotyczące zadań importu plików PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

- Jeśli chcesz sprawdzić stan określonego zadania importu, użyj [get-MailboxImportRequest -batchname.](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)

- Aby uzyskać szczegółowe informacje na temat usługi importowania, zobacz Omówienie importowania plików [PST organizacji.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
