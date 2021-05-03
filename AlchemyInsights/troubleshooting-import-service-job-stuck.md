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
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="36264-102">Rozwiązywanie problemów z zadaniem usługi importowania nie rozwiązało problemu</span><span class="sxs-lookup"><span data-stu-id="36264-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="36264-103">Jeśli występują problemy z importowaniem zadań usługi utknęły lub się nie powiedają, sprawdź i wypróbuj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="36264-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="36264-104">Sprawdź rozmiar pliku PST.</span><span class="sxs-lookup"><span data-stu-id="36264-104">Review the size of of the PST file.</span></span> <span data-ttu-id="36264-105">Maksymalny rozmiar pliku PST zalecany w przypadku importowania wynosi 20 GB.</span><span class="sxs-lookup"><span data-stu-id="36264-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="36264-106">Jeśli podejrzewasz, że pominięte elementy są pomijane z powodu uszkodzenia, uruchom Scanpst.exe, aby zdiagnozować i naprawić błędy w plikach PST.</span><span class="sxs-lookup"><span data-stu-id="36264-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="36264-107">Jeśli podczas importowania zostanie wyświetlony błąd "MapiExceptionShutoffQuotaExceeded", upewnij się, że docelowa skrzynka pocztowa ma wystarczająco dużo pojemności, aby zaimportować odpowiednie pliki PST.</span><span class="sxs-lookup"><span data-stu-id="36264-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="36264-108">Aby uzyskać więcej informacji na temat rozwiązywania problemów z zadaniami importu plików PST, zobacz [Rozwiązywanie problemów z zadaniami importu pliku PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="36264-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="36264-109">Aby uzyskać informacje o tym, jak rozwiązać problemy podczas importowania plików PST do programu Outlook, zobacz Rozwiązywanie problemów z importowaniem pliku [pst programu Outlook (microsoft.com).](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)</span><span class="sxs-lookup"><span data-stu-id="36264-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>