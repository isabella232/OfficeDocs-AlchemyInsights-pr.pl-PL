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
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="4d6ad-102">Rozwiązywanie problemów z importowaniem pliku PST</span><span class="sxs-lookup"><span data-stu-id="4d6ad-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="4d6ad-103">Jeśli importujesz dane w obrębie samego klienta programu Outlook, zobacz Rozwiązywanie problemów z importowaniem pliku [pst programu Outlook.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)</span><span class="sxs-lookup"><span data-stu-id="4d6ad-103">If you are importing within the Outlook client itself, see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="4d6ad-104">Jeśli korzystasz z usługi importowania i problem się zablokował, pamiętaj, że każdy plik PST, który przekażemy do lokalizacji magazynu platformy Azure, nie powinien być większy niż 20 GB.</span><span class="sxs-lookup"><span data-stu-id="4d6ad-104">If you are using Import Service and it's stuck, note that each PST file that you upload to the Azure Storage location should be no larger than 20GB.</span></span> <span data-ttu-id="4d6ad-105">Pliki PST o rozmiarze większym niż 20 GB mogą mieć wpływ na wydajność procesu importowania pliku PST.</span><span class="sxs-lookup"><span data-stu-id="4d6ad-105">PST files larger than 20GB may impact the performance of the PST import process.</span></span> <span data-ttu-id="4d6ad-106">Aby uzyskać więcej informacji dotyczących rozwiązywania problemów z zadaniami, które utknęły, zobacz [Problemy dotyczące zadań importu plików PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="4d6ad-106">For more information troubleshooting stuck jobs, see [Issues that affect PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

- <span data-ttu-id="4d6ad-107">Jeśli chcesz sprawdzić stan określonego zadania importu, użyj [get-MailboxImportRequest -batchname.](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)</span><span class="sxs-lookup"><span data-stu-id="4d6ad-107">If you want to verify the status of a specific Import job, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="4d6ad-108">Aby uzyskać szczegółowe informacje na temat usługi importowania, zobacz Omówienie importowania plików [PST organizacji.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="4d6ad-108">For full details on the import service, see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
