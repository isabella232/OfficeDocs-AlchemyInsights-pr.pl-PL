---
title: Rozwiązywanie problemów z ładowaniem obrazów w usłudze Yammer
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
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148294"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="53b25-102">Rozwiązywanie problemów z ładowaniem obrazów w usłudze Yammer</span><span class="sxs-lookup"><span data-stu-id="53b25-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="53b25-103">W przypadku wystąpienia problemów ze zdjęciami i podglądami plików w usłudze Yammer należy rozwiązać problem, sprawdzając, czy problem występuje dla wszystkich użytkowników, czy występuje na urządzeniach przenośnych i czy jest odtwarzalny podczas przekazywania załącznika.</span><span class="sxs-lookup"><span data-stu-id="53b25-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="53b25-104">**Problemy ze zdjęciem w profilu**</span><span class="sxs-lookup"><span data-stu-id="53b25-104">**Profile photo issues**</span></span>  

<span data-ttu-id="53b25-105">Jeśli użytkownicy końcowi logują się do usługi Yammer za pośrednictwem usługi Microsoft 365, muszą zmienić swój profil, w tym zdjęcie profilowe.</span><span class="sxs-lookup"><span data-stu-id="53b25-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="53b25-106">Jeśli użytkownicy nie mogą dokonywać aktualizacji profilu, administrator może dokonać aktualizacji dla użytkownika.</span><span class="sxs-lookup"><span data-stu-id="53b25-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="53b25-107">Aby uzyskać więcej informacji, zobacz [Wyświetlanie i aktualizowanie profilu w aplikacji Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="53b25-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="53b25-108">Aby uzyskać informacje o edycji profilu, w tym zdjęcia profilowe, zobacz [Zmienianie profilu i ustawień usługi Yammer](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="53b25-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="53b25-109">Zaktualizowane zdjęcia profilowe są synchronizowane inaczej niż atrybuty profilu.</span><span class="sxs-lookup"><span data-stu-id="53b25-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="53b25-110">Użytkownicy muszą się zalogować, aby zainicjować synchronizację swojego zdjęcia profilowego.</span><span class="sxs-lookup"><span data-stu-id="53b25-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="53b25-111">Aby uzyskać więcej informacji, zobacz [są zdjęcia profilowe użytkowników zaktualizowane z usługi Office 365 do usługi Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="53b25-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="53b25-112">Aby uzyskać informacje o cyklu życia użytkownika usługi Yammer, zobacz [Zarządzanie użytkownikami usługi Yammer w całym cyklu życia z usługi Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="53b25-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="53b25-113">Aby uzyskać szczegółowe informacje na temat działania synchronizacji zdjęć profilowych w usłudze Microsoft 365, zobacz [Informacje o synchronizacji obrazów profilowych w usłudze Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="53b25-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="53b25-114">**Podglądy dokumentów i problemy z miniaturami obrazów**</span><span class="sxs-lookup"><span data-stu-id="53b25-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="53b25-115">Gdy pliki lub obrazy są publikowane w usłudze Yammer, podglądy mogą nie być wyświetlane, ponieważ:</span><span class="sxs-lookup"><span data-stu-id="53b25-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="53b25-116">Plik jest uszkodzony i nie można go przetworzyć.</span><span class="sxs-lookup"><span data-stu-id="53b25-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="53b25-117">Plik nie został niedawno przekazany do usługi SharePoint Online lub usługa Yammer ma nieprawidłowe metadane z innych powodów.</span><span class="sxs-lookup"><span data-stu-id="53b25-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="53b25-118">Adresy URL wymagane do ładowania obrazów podglądu są blokowane.</span><span class="sxs-lookup"><span data-stu-id="53b25-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="53b25-119">Podgląd pliku został usunięty przez użytkownika przed opublikowaniem.</span><span class="sxs-lookup"><span data-stu-id="53b25-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="53b25-120">Problem z usługą uniemożliwił wygenerowanie podglądu.</span><span class="sxs-lookup"><span data-stu-id="53b25-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="53b25-121">**Uwaga** Podglądy łączy i przekazywania plików mogą zachowywać się inaczej.</span><span class="sxs-lookup"><span data-stu-id="53b25-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="53b25-122">Łącza do plików w Internecie lub łącza wymagające dodatkowego uwierzytelniania mogą nie być wyświetlane poprawnie.</span><span class="sxs-lookup"><span data-stu-id="53b25-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="53b25-123">Aby uzyskać więcej informacji, zobacz [Dołączanie pliku lub obrazu do wiadomości usługi Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="53b25-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 