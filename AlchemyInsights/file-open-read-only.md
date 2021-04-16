---
title: Otwieranie pliku tylko do odczytu
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813194"
---
# <a name="file-open-read-only"></a><span data-ttu-id="afcd1-102">Otwieranie pliku tylko do odczytu</span><span class="sxs-lookup"><span data-stu-id="afcd1-102">File open read-only</span></span>

<span data-ttu-id="afcd1-103">Może się okazać, że podczas otwierania plików będą one otwierane jako tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="afcd1-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="afcd1-104">W niektórych przypadkach jest to ze względu na dodatkowe zabezpieczenia, na przykład podczas otwierania plików z Internetu i w innych przypadkach, może to być spowodowane ustawieniem, które można zmienić.</span><span class="sxs-lookup"><span data-stu-id="afcd1-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="afcd1-105">Oto kilka scenariuszy, w których plik jest otwierany w stanie tylko do odczytu, a niektóre czynności, które możesz wykonać, aby to zmienić.</span><span class="sxs-lookup"><span data-stu-id="afcd1-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="afcd1-106">**Moje oprogramowanie antywirusowe powoduje, że otwiera się w stanie tylko do odczytu**</span><span class="sxs-lookup"><span data-stu-id="afcd1-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="afcd1-107">Niektóre programy antywirusowe mogą chronić użytkownika przed potencjalnie niebezpiecznymi plikami, otwierając je tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="afcd1-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="afcd1-108">Aby dowiedzieć się, jak dostosować te ustawienia, może być konieczne s skontaktuj się z dostawcą oprogramowania antywirusowego.</span><span class="sxs-lookup"><span data-stu-id="afcd1-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="afcd1-109">Na przykład w programie BitDefender opisano dodawanie wykluczeń aplikacji tutaj: Jak dodać wykluczenia aplikacji lub procesów w Centrum sterowania [Bitdefender.](https://aka.ms/AA6098i)</span><span class="sxs-lookup"><span data-stu-id="afcd1-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="afcd1-110">**Czy właściwości pliku są ustawione na tylko do odczytu?**</span><span class="sxs-lookup"><span data-stu-id="afcd1-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="afcd1-111">Możesz sprawdzić właściwości pliku, klikając go prawym przyciskiem myszy i wybierając polecenie Właściwości.</span><span class="sxs-lookup"><span data-stu-id="afcd1-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="afcd1-112">Jeśli zaznaczono atrybut Tylko do odczytu, możesz usunąć jego zaznaczenie i kliknąć przycisk OK.</span><span class="sxs-lookup"><span data-stu-id="afcd1-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="afcd1-113">**Zawartość jest w widoku chronionym**</span><span class="sxs-lookup"><span data-stu-id="afcd1-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="afcd1-114">Pliki z Internetu i innych potencjalnie niebezpiecznych lokalizacji mogą zawierać wirusy, robaki lub inne rodzaje złośliwego oprogramowania, które może uszkodzić Twój komputer.</span><span class="sxs-lookup"><span data-stu-id="afcd1-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="afcd1-115">Dotyczy to zazwyczaj załączników wiadomości e-mail lub pobranych plików.</span><span class="sxs-lookup"><span data-stu-id="afcd1-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="afcd1-116">Aby chronić komputer, pliki z tych potencjalnie niebezpiecznych lokalizacji są otwierane w widoku chronionym.</span><span class="sxs-lookup"><span data-stu-id="afcd1-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="afcd1-117">Widok chroniony pozwala odczytywać plik i wyświetlać jego zawartość, zmniejszając ryzyko.</span><span class="sxs-lookup"><span data-stu-id="afcd1-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="afcd1-118">Aby uzyskać więcej informacji na temat widoku chronionego i sposobu zmieniania ustawień, zobacz ten artykuł: [Co to jest widok chroniony?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="afcd1-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="afcd1-119">**Czy onedrive jest pełne?**</span><span class="sxs-lookup"><span data-stu-id="afcd1-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="afcd1-120">Jeśli plik jest przechowywany w usłudze OneDrive i całe miejsca do magazynowania w usłudze OneDrive zostanie zapełnione, nie będzie można zapisać dokumentu, dopóki nie będzie wolnego miejsca.</span><span class="sxs-lookup"><span data-stu-id="afcd1-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="afcd1-121">Możesz sprawdzić wolne miejsce w usłudze OneDrive, klikając ikonę usługi OneDrive w centrum powiadomień i wybierając pozycję Zarządzaj przestrzenią dyskową. Możesz też przejść do pozycji , zalogować się i zanotować ilość używanego miejsca w lewym dolnym rogu [https://onedrive.live.com](https://onedrive.live.com) ekranu.</span><span class="sxs-lookup"><span data-stu-id="afcd1-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="afcd1-122">**Czy pakiet Office został aktywowany?**</span><span class="sxs-lookup"><span data-stu-id="afcd1-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="afcd1-123">Jeśli pakiet Office nie został aktywowany lub jeśli Twoja subskrypcja wygasła, być może używasz trybu ograniczonej funkcjonalności, który jest trybem tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="afcd1-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="afcd1-124">Aby uzyskać informacje na temat aktywowania pakietu Office, zobacz: Błędy "Produkt bez licencji" i [błędy aktywacji w psłudze Office.](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="afcd1-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="afcd1-125">**Jeśli wszystko inne zawiedzie...**</span><span class="sxs-lookup"><span data-stu-id="afcd1-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="afcd1-126">Spróbuj ponownie uruchomić komputer</span><span class="sxs-lookup"><span data-stu-id="afcd1-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="afcd1-127">Instalowanie aktualizacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="afcd1-127">Install Office updates</span></span>
    
- <span data-ttu-id="afcd1-128">Wykonywanie naprawy online pakietu Office</span><span class="sxs-lookup"><span data-stu-id="afcd1-128">Perform an Online repair of Office</span></span>
    

