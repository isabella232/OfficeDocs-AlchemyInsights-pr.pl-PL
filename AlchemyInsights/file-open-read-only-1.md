---
title: Otwieranie pliku tylko do odczytu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 69705825-723a-4c1e-ae85-d16b5051d2fe
ms.openlocfilehash: 06c052383a6462288270d2e062930352883a199a
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525725"
---
# <a name="file-open-read-only"></a><span data-ttu-id="41d52-102">Otwieranie pliku tylko do odczytu</span><span class="sxs-lookup"><span data-stu-id="41d52-102">File open read-only</span></span>

<span data-ttu-id="41d52-103">Może się okazać, że otwierając pliki, otworzyć jako tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="41d52-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="41d52-104">W niektórych przypadkach to aby zwiększyć bezpieczeństwo, takie jak otwierając pliki z Internetu, a innym razem, mogą występować z powodu ustawienia, które mogą być zmieniane.</span><span class="sxs-lookup"><span data-stu-id="41d52-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="41d52-105">Poniżej przedstawiono kilka scenariuszy, w którym plik zostanie otwarty tylko do odczytu i czynności, jakie można podjąć, aby to zmienić.</span><span class="sxs-lookup"><span data-stu-id="41d52-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="41d52-106">**Mój program antywirusowy jest przyczyną je otworzyć tylko do odczytu**</span><span class="sxs-lookup"><span data-stu-id="41d52-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="41d52-107">Niektóre programy antywirusowe mogą chronić potencjalnie niebezpiecznych plików przez otwarcie ich jako tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="41d52-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="41d52-108">Należy skontaktować się z dostawcą oprogramowania antywirusowego, aby dowiedzieć się, jak dostosować te ustawienia.</span><span class="sxs-lookup"><span data-stu-id="41d52-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="41d52-109">BitDefender, na przykład ma zawartość na dodanie wykluczeń aplikacji tutaj: [jak dodać aplikację lub wykluczenia procesu w centrum sterowania Bitdefender](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span><span class="sxs-lookup"><span data-stu-id="41d52-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="41d52-110">**Właściwości pliku ustawiono atrybut tylko do odczytu?**</span><span class="sxs-lookup"><span data-stu-id="41d52-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="41d52-111">Można sprawdzić właściwości pliku prawym przyciskiem myszy plik i wybierz polecenie Właściwości.</span><span class="sxs-lookup"><span data-stu-id="41d52-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="41d52-112">Jeśli atrybut tylko do odczytu jest zaznaczone, można usunąć jego zaznaczenie i kliknij OK.</span><span class="sxs-lookup"><span data-stu-id="41d52-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="41d52-113">**Zawartość jest w widoku chronionym**</span><span class="sxs-lookup"><span data-stu-id="41d52-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="41d52-114">Pliki z Internetu i innych potencjalnie niebezpiecznych lokalizacjach mogą zawierać wirusy, robaki lub inne rodzaje złośliwego oprogramowania, które mogą uszkodzić komputer.</span><span class="sxs-lookup"><span data-stu-id="41d52-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="41d52-115">Jest to również często z załączników wiadomości e-mail lub pliki pobrane.</span><span class="sxs-lookup"><span data-stu-id="41d52-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="41d52-116">Aby pomóc w ochronie tego komputera, pliki z lokalizacji tych potencjalnie niebezpieczne są otwierane w widoku chronionym.</span><span class="sxs-lookup"><span data-stu-id="41d52-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="41d52-117">Za pomocą widoku chronionego, można czytać pliku i wyświetlić jego zawartość przy jednoczesnym zmniejszeniu ryzyka.</span><span class="sxs-lookup"><span data-stu-id="41d52-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="41d52-118">Aby uzyskać więcej informacji w widoku chronionym i sposobu zmieniania ustawień, w tym artykule: [Co to jest widok chroniony?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="41d52-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="41d52-119">**OneDrive jest zapełniony?**</span><span class="sxs-lookup"><span data-stu-id="41d52-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="41d52-120">Jeśli plik jest przechowywany na OneDrive i z przestrzeni magazynowania jest pełny, nie można zapisać dokumentu, dopóki nie są pod przydzielonego miejsca.</span><span class="sxs-lookup"><span data-stu-id="41d52-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="41d52-121">Wolne miejsce na dysku OneDrive można sprawdzić, klikając ikonę OneDrive w Centrum powiadomień i wybierając polecenie Zarządzanie magazynem, lub możesz przejść do [http://onedrive.live.com](http://onedrive.live.com), zaloguj się i zanotuj ilość zajętego miejsca w dolnym lewym rogu ekranu.</span><span class="sxs-lookup"><span data-stu-id="41d52-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="41d52-122">**Urząd jest aktywowany?**</span><span class="sxs-lookup"><span data-stu-id="41d52-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="41d52-123">Jeśli pakietu Office nie jest aktywowany lub jeśli Twoja subskrypcja wygasła, może być w trybie tylko do odczytu trybie zmniejszonej funkcjonalności.</span><span class="sxs-lookup"><span data-stu-id="41d52-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="41d52-124">Szczegółowe informacje na temat aktywacji pakietu Office: [produkt bez licencji i błędów aktywacji pakietu Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="41d52-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="41d52-125">**Jeśli wszystkie inne źródła zawiodą...**</span><span class="sxs-lookup"><span data-stu-id="41d52-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="41d52-126">Spróbuj ponownie uruchomić komputer</span><span class="sxs-lookup"><span data-stu-id="41d52-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="41d52-127">Zainstaluj aktualizacje pakietu Office</span><span class="sxs-lookup"><span data-stu-id="41d52-127">Install Office updates</span></span>
    
- <span data-ttu-id="41d52-128">Wykonać naprawy w trybie Online pakietu Office</span><span class="sxs-lookup"><span data-stu-id="41d52-128">Perform an Online repair of Office</span></span>
    

