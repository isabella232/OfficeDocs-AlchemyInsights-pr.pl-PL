---
title: Plik tylko do odczytu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: c045188af15fcec0f868eb0e5b399bd1fb42a09a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702784"
---
# <a name="file-open-read-only"></a><span data-ttu-id="1b5d2-102">Plik tylko do odczytu</span><span class="sxs-lookup"><span data-stu-id="1b5d2-102">File open read-only</span></span>

<span data-ttu-id="1b5d2-103">Może się okazać, że podczas otwierania plików otwierają się one jako tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="1b5d2-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="1b5d2-104">W niektórych przypadkach jest to dla zwiększenia bezpieczeństwa, na przykład podczas otwierania plików z Internetu, a innym razem może to być spowodowane ustawieniem, które można zmienić.</span><span class="sxs-lookup"><span data-stu-id="1b5d2-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="1b5d2-105">Oto kilka scenariuszy, w których plik otwiera tylko do odczytu i kilka kroków, które można wykonać, aby to zmienić.</span><span class="sxs-lookup"><span data-stu-id="1b5d2-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="1b5d2-106">**Mój program antywirusowy powoduje, że otwierają się tylko do odczytu**</span><span class="sxs-lookup"><span data-stu-id="1b5d2-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="1b5d2-107">Niektóre programy antywirusowe mogą chronić przed potencjalnie niebezpiecznymi plikami, otwierając je tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="1b5d2-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="1b5d2-108">Może być konieczne skontaktowanie się z dostawcą oprogramowania antywirusowego, aby dowiedzieć się, jak dostosować te ustawienia.</span><span class="sxs-lookup"><span data-stu-id="1b5d2-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="1b5d2-109">BitDefender, na przykład, ma zawartość na dodawanie wykluczeń aplikacji tutaj: [Jak dodać wykluczenia aplikacji lub procesu w Centrum sterowania Bitdefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="1b5d2-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="1b5d2-110">**Czy właściwości pliku są ustawione na tylko do odczytu?**</span><span class="sxs-lookup"><span data-stu-id="1b5d2-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="1b5d2-111">Właściwości pliku można sprawdzić, klikając prawym przyciskiem myszy plik i wybierając polecenie Właściwości.</span><span class="sxs-lookup"><span data-stu-id="1b5d2-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="1b5d2-112">Jeśli atrybut Tylko do odczytu jest zaznaczony, możesz go odznaczyć i kliknąć przycisk OK.</span><span class="sxs-lookup"><span data-stu-id="1b5d2-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="1b5d2-113">**Zawartość jest w widoku chronionym**</span><span class="sxs-lookup"><span data-stu-id="1b5d2-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="1b5d2-114">Pliki z Internetu i z innych potencjalnie niebezpiecznych lokalizacji mogą zawierać wirusy, robaki lub inne rodzaje złośliwego oprogramowania, które mogą uszkodzić komputer.</span><span class="sxs-lookup"><span data-stu-id="1b5d2-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="1b5d2-115">Jest to również często w przypadku załączników wiadomości e-mail lub pobranych plików.</span><span class="sxs-lookup"><span data-stu-id="1b5d2-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="1b5d2-116">Aby chronić komputer, pliki z tych potencjalnie niebezpiecznych lokalizacji są otwierane w widoku chronionym.</span><span class="sxs-lookup"><span data-stu-id="1b5d2-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="1b5d2-117">Korzystając z widoku chronionego, można odczytać plik i wyświetlić jego zawartość przy jednoczesnym zmniejszeniu ryzyka.</span><span class="sxs-lookup"><span data-stu-id="1b5d2-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="1b5d2-118">Aby uzyskać więcej informacji na temat widoku chronionego i sposobu zmiany ustawień, zobacz ten artykuł: [Co to jest widok chroniony?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="1b5d2-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="1b5d2-119">**Czy usługa OneDrive jest pełna?**</span><span class="sxs-lookup"><span data-stu-id="1b5d2-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="1b5d2-120">Jeśli plik jest przechowywany w usłudze OneDrive, a miejsce w magazynie usługi OneDrive jest zapełnione, nie będzie można zapisać dokumentu, dopóki nie znajdzie się w przydzielonym miejscu.</span><span class="sxs-lookup"><span data-stu-id="1b5d2-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="1b5d2-121">Możesz zaznaczyć wolne miejsce w usłudze OneDrive, klikając ikonę Usługi OneDrive w [https://onedrive.live.com](https://onedrive.live.com)centrum powiadomień i wybierając pozycję Zarządzaj magazynem, lub przejdź do , zaloguj się i zanotuj ilość używanego miejsca w lewym dolnym połówka ekranu.</span><span class="sxs-lookup"><span data-stu-id="1b5d2-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="1b5d2-122">**Czy pakiet Office jest aktywowany?**</span><span class="sxs-lookup"><span data-stu-id="1b5d2-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="1b5d2-123">Jeśli pakiet Office nie jest aktywowany lub subskrypcja wygasła, możesz być w trybie zmniejszonej funkcjonalności tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="1b5d2-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="1b5d2-124">Aby uzyskać informacje na temat aktywowania pakietu Office, zobacz: [Nielicencjonowany produkt i błędy aktywacji w pakiecie Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="1b5d2-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="1b5d2-125">**Jeśli wszystko inne zawiedzie...**</span><span class="sxs-lookup"><span data-stu-id="1b5d2-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="1b5d2-126">Spróbuj ponownie uruchomić komputer</span><span class="sxs-lookup"><span data-stu-id="1b5d2-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="1b5d2-127">Instalowanie aktualizacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="1b5d2-127">Install Office updates</span></span>
    
- <span data-ttu-id="1b5d2-128">Wykonywanie naprawy pakietu Office online</span><span class="sxs-lookup"><span data-stu-id="1b5d2-128">Perform an Online repair of Office</span></span>
    

