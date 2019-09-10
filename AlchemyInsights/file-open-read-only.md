---
title: Plik otwarty tylko do odczytu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: eddd427b159a782abf53adda934de8b15a02ed00
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822244"
---
# <a name="file-open-read-only"></a><span data-ttu-id="473d6-102">Plik otwarty tylko do odczytu</span><span class="sxs-lookup"><span data-stu-id="473d6-102">File open read-only</span></span>

<span data-ttu-id="473d6-103">Może się okazać, że podczas otwierania plików, otwierają się jako tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="473d6-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="473d6-104">W niektórych przypadkach jest to dla dodatkowych zabezpieczeń, takich jak podczas otwierania plików z Internetu, a inne czasy, może być ze względu na ustawienie, które mogą być zmieniane.</span><span class="sxs-lookup"><span data-stu-id="473d6-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="473d6-105">Oto kilka scenariuszy, w których plik otwiera tylko do odczytu i niektóre kroki można podjąć, aby zmienić.</span><span class="sxs-lookup"><span data-stu-id="473d6-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="473d6-106">**Mój program antywirusowy powoduje otwarcie tylko do odczytu**</span><span class="sxs-lookup"><span data-stu-id="473d6-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="473d6-107">Niektóre programy antywirusowe mogą chronić Cię przed potencjalnie niebezpiecznymi plikami, otwierając je tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="473d6-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="473d6-108">Aby dowiedzieć się, jak dostosować te ustawienia, konieczne może być sprawdzenie u dostawcy oprogramowania antywirusowego.</span><span class="sxs-lookup"><span data-stu-id="473d6-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="473d6-109">Na przykład BitDefender zawiera treści dotyczące dodawania wykluczeń aplikacji tutaj: [jak dodać wykluczenia aplikacji lub procesu w BitDefender Control Center](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="473d6-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="473d6-110">**Czy właściwości pliku są ustawione na tylko do odczytu?**</span><span class="sxs-lookup"><span data-stu-id="473d6-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="473d6-111">Właściwości pliku można sprawdzić, klikając prawym przyciskiem myszy plik i wybierając polecenie Właściwości.</span><span class="sxs-lookup"><span data-stu-id="473d6-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="473d6-112">Jeśli atrybut tylko do odczytu jest zaznaczony, można odznaczyć go i kliknij przycisk OK.</span><span class="sxs-lookup"><span data-stu-id="473d6-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="473d6-113">**Zawartość jest w widoku chronionym**</span><span class="sxs-lookup"><span data-stu-id="473d6-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="473d6-114">Pliki z Internetu i z innych potencjalnie niebezpiecznych lokalizacji mogą zawierać wirusy, robaki lub inne rodzaje złośliwego oprogramowania, które może uszkodzić komputer.</span><span class="sxs-lookup"><span data-stu-id="473d6-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="473d6-115">Jest to również często w przypadku załączników e-mail lub pobranych plików.</span><span class="sxs-lookup"><span data-stu-id="473d6-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="473d6-116">Aby ułatwić ochronę komputera, pliki z tych potencjalnie niebezpiecznych lokalizacji są otwierane w widoku chronionym.</span><span class="sxs-lookup"><span data-stu-id="473d6-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="473d6-117">Za pomocą widoku chronionego można odczytać plik i wyświetlić jego zawartość, jednocześnie zmniejszając ryzyko.</span><span class="sxs-lookup"><span data-stu-id="473d6-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="473d6-118">Aby uzyskać więcej informacji o widoku chronionym i sposobie zmieniania ustawień, zobacz ten artykuł: [co to jest Widok chroniony?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="473d6-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="473d6-119">**Czy usługa OneDrive jest pełna?**</span><span class="sxs-lookup"><span data-stu-id="473d6-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="473d6-120">Jeśli plik jest przechowywany w usłudze OneDrive, a przestrzeń dyskowa usługi OneDrive jest zapełcona, nie będzie można zapisać dokumentu, dopóki nie znajdujesz się pod wyznaczonym miejscem.</span><span class="sxs-lookup"><span data-stu-id="473d6-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="473d6-121">Możesz sprawdzić swoje wolne miejsce w OneDrive, klikając ikonę OneDrive w centrum powiadomień i wybierając Zarządzaj magazynem, lub możesz przejść do [http://onedrive.live.com](http://onedrive.live.com), zaloguj się i Zanotuj ilość używanego miejsca w lewym dolnym rogu ekranu.</span><span class="sxs-lookup"><span data-stu-id="473d6-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="473d6-122">**Czy pakiet Office jest aktywowany?**</span><span class="sxs-lookup"><span data-stu-id="473d6-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="473d6-123">Jeśli pakiet Office nie jest aktywowany lub subskrypcja wygasła, może być w trybie ograniczonej funkcjonalności tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="473d6-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="473d6-124">Aby uzyskać informacje dotyczące sposobu aktywowania pakietu Office, zobacz: [nielicencjonowane produkty i błędy aktywacji w pakiecie Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="473d6-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="473d6-125">**Jeśli wszystko inne zawiedzie...**</span><span class="sxs-lookup"><span data-stu-id="473d6-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="473d6-126">Spróbuj ponownie uruchomić komputer</span><span class="sxs-lookup"><span data-stu-id="473d6-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="473d6-127">Instalowanie aktualizacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="473d6-127">Install Office updates</span></span>
    
- <span data-ttu-id="473d6-128">Przeprowadź naprawę online pakietu Office</span><span class="sxs-lookup"><span data-stu-id="473d6-128">Perform an Online repair of Office</span></span>
    

