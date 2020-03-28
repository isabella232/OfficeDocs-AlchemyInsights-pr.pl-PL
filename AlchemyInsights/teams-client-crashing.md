---
title: Awarie klienta usługi Teams?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030678"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="7baa4-102">Awarie klienta usługi Teams?</span><span class="sxs-lookup"><span data-stu-id="7baa4-102">Teams client crashing?</span></span>

<span data-ttu-id="7baa4-103">Jeśli masz problem z awariami klienta usługi Teams, spróbuj poniższych rozwiązań:</span><span class="sxs-lookup"><span data-stu-id="7baa4-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="7baa4-104">Jeśli używasz aplikacji klasycznej Teams, [upewnij się, że aplikacja jest w pełni zaktualizowana](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="7baa4-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="7baa4-105">Upewnij się, że wszystkie [ zakresy adresów URL i adresy URL pakietu Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) są dostępne.</span><span class="sxs-lookup"><span data-stu-id="7baa4-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="7baa4-106">Zaloguj się do konta administratora usługi i sprawdź na [pulpicie nawigacyjnym kondycji usługi](https://docs.microsoft.com/office365/enterprise/view-service-health), czy nie ma awarii ani obniżenia wydajności usługi.</span><span class="sxs-lookup"><span data-stu-id="7baa4-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="7baa4-107">Na koniec możesz spróbować wyczyścić pamięć podręczną klienta usługi Teams:</span><span class="sxs-lookup"><span data-stu-id="7baa4-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="7baa4-108">Całkowicie zamknij klienta stacjonarnego usługi Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7baa4-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="7baa4-109">Kliknij prawym przyciskiem myszy **Teams** na pasku ikon i kliknij **Zamknij** albo otwórz Menedżer zadań i całkowicie zakończ proces.</span><span class="sxs-lookup"><span data-stu-id="7baa4-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="7baa4-110">Przejdź do Eksploratora plików i wpisz %appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="7baa4-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="7baa4-111">Po otwarciu katalogu będą widoczne następujące foldery:</span><span class="sxs-lookup"><span data-stu-id="7baa4-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="7baa4-112">W folderze **Application Cache** otwórz folder Cache i usuń wszystkie znajdujące się w nim pliki:  %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="7baa4-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="7baa4-113">W folderze **Blob_storage** usuń wszystkie pliki: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="7baa4-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="7baa4-114">W folderze **Cache**, usuń wszystkie pliki: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="7baa4-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="7baa4-115">W folderze **databases** usuń wszystkie pliki: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="7baa4-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="7baa4-116">W folderze **GPUCache** usuń wszystkie pliki: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="7baa4-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="7baa4-117">W folderze **IndexedDB** usuń plik .db: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="7baa4-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="7baa4-118">W folderze **Local Storage** usuń wszystkie pliki: %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="7baa4-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="7baa4-119">Na koniec w folerze **tmp** usuń wszystkie pliki: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="7baa4-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="7baa4-120">Ponownie otwórz klienta usługi Teams.</span><span class="sxs-lookup"><span data-stu-id="7baa4-120">Restart your Teams client.</span></span>
