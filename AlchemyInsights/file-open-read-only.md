---
title: Plik otwarty tylko do odczytu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745617"
---
# <a name="file-open-read-only"></a><span data-ttu-id="5b078-102">Plik otwarty tylko do odczytu</span><span class="sxs-lookup"><span data-stu-id="5b078-102">File open read-only</span></span>

<span data-ttu-id="5b078-103">Podczas otwierania plików może się okazać, że są one otwierane w trybie tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="5b078-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="5b078-104">W razie potrzeby jest to Zwiększanie bezpieczeństwa, na przykład podczas otwierania plików z Internetu i innych godzin, może być spowodowane ustawieniem, które można zmienić.</span><span class="sxs-lookup"><span data-stu-id="5b078-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="5b078-105">Poniżej przedstawiono niektóre scenariusze, w których plik jest otwierany tylko do odczytu, i czynności, które można wykonać w celu zmiany tego pliku.</span><span class="sxs-lookup"><span data-stu-id="5b078-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="5b078-106">**Mój program antywirusowy powoduje, że są otwierane tylko do odczytu**</span><span class="sxs-lookup"><span data-stu-id="5b078-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="5b078-107">Niektóre programy antywirusowe mogą chronić Cię przed potencjalnie niebezpiecznymi plikami, otwierając je w trybie tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="5b078-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="5b078-108">Aby dowiedzieć się, jak dostosować te ustawienia, może być konieczne skontaktowanie się z dostawcą programu antywirusowego.</span><span class="sxs-lookup"><span data-stu-id="5b078-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="5b078-109">BitDefender, na przykład, ma zawartość dotyczącą dodawania wykluczeń aplikacji: [jak dodać wykluczenia aplikacji lub procesu w centrum kontroli BitDefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="5b078-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="5b078-110">**Czy właściwości pliku są ustawione jako tylko do odczytu?**</span><span class="sxs-lookup"><span data-stu-id="5b078-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="5b078-111">Możesz sprawdzić właściwości pliku, klikając go prawym przyciskiem myszy i wybierając polecenie Właściwości.</span><span class="sxs-lookup"><span data-stu-id="5b078-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="5b078-112">Jeśli atrybut tylko do odczytu jest zaznaczony, możesz usunąć jego zaznaczenie, a następnie kliknąć przycisk OK.</span><span class="sxs-lookup"><span data-stu-id="5b078-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="5b078-113">**Zawartość jest w widoku chronionym**</span><span class="sxs-lookup"><span data-stu-id="5b078-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="5b078-114">Pliki z Internetu i innych potencjalnie niebezpiecznych lokalizacji mogą zawierać wirusy, robaki lub inne typy złośliwego oprogramowania, które mogą uszkodzić komputer.</span><span class="sxs-lookup"><span data-stu-id="5b078-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="5b078-115">Jest to również często przypadek z dołączonymi załącznikami wiadomości e-mail lub plikami, które zostały pobrane.</span><span class="sxs-lookup"><span data-stu-id="5b078-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="5b078-116">Aby ułatwić ochronę komputera, pliki z tych potencjalnie niebezpiecznych lokalizacji są otwierane w widoku chronionym.</span><span class="sxs-lookup"><span data-stu-id="5b078-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="5b078-117">Za pomocą widoku chronionego można odczytać plik i wyświetlić jego zawartość, zmniejszając ryzyko.</span><span class="sxs-lookup"><span data-stu-id="5b078-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="5b078-118">Aby uzyskać więcej informacji na temat widoku chronionego i sposobu zmieniania ustawień, zobacz ten artykuł: [co to jest Widok chroniony?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="5b078-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="5b078-119">**Czy usługa OneDrive jest pełna?**</span><span class="sxs-lookup"><span data-stu-id="5b078-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="5b078-120">Jeśli plik jest przechowywany w usłudze OneDrive, a ilość miejsca do magazynowania w usłudze OneDrive jest pełna, nie będzie można zapisać dokumentu, dopóki nie znajdzie się pod przydzielonym obszarem.</span><span class="sxs-lookup"><span data-stu-id="5b078-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="5b078-121">Możesz sprawdzić ilość wolnego miejsca w usłudze OneDrive, klikając ikonę usługi OneDrive w centrum powiadomień, a następnie wybierając pozycję Zarządzaj miejscem do magazynowania, lub przejdź do [https://onedrive.live.com](https://onedrive.live.com) pozycji zalogować się, a następnie zanotuj ilość miejsca zajętego w lewym dolnym rogu ekranu.</span><span class="sxs-lookup"><span data-stu-id="5b078-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="5b078-122">**Czy pakiet Office jest aktywowany?**</span><span class="sxs-lookup"><span data-stu-id="5b078-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="5b078-123">Jeśli pakiet Office nie został aktywowany lub subskrypcja wygasła, możesz być w trybie tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="5b078-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="5b078-124">Aby uzyskać informacje o tym, jak aktywować pakiet Office, zobacz: [Błędy nielicencjonowanego produktu i aktywacji w pakiecie Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="5b078-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="5b078-125">**Jeśli nie uda się...**</span><span class="sxs-lookup"><span data-stu-id="5b078-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="5b078-126">Spróbuj ponownie uruchomić komputer</span><span class="sxs-lookup"><span data-stu-id="5b078-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="5b078-127">Instalowanie aktualizacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="5b078-127">Install Office updates</span></span>
    
- <span data-ttu-id="5b078-128">Wykonywanie naprawy online pakietu Office</span><span class="sxs-lookup"><span data-stu-id="5b078-128">Perform an Online repair of Office</span></span>
    

