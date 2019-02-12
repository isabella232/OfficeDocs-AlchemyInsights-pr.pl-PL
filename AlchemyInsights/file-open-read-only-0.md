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
ms.assetid: 6a828f8d-ff31-40a7-b701-b2339e771817
ms.openlocfilehash: be232b682b7bb3d24f59ad10501edbd796e6bcaf
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29935879"
---
# <a name="file-open-read-only"></a><span data-ttu-id="31109-102">Otwieranie pliku tylko do odczytu</span><span class="sxs-lookup"><span data-stu-id="31109-102">File open read-only</span></span>

<span data-ttu-id="31109-p101">Może się okazać, że otwierając pliki, otworzyć jako tylko do odczytu. W niektórych przypadkach to aby zwiększyć bezpieczeństwo, takie jak otwierając pliki z Internetu, a innym razem, mogą występować z powodu ustawienia, które mogą być zmieniane. Poniżej przedstawiono kilka scenariuszy, w którym plik zostanie otwarty tylko do odczytu i czynności, jakie można podjąć, aby to zmienić.</span><span class="sxs-lookup"><span data-stu-id="31109-p101">You may find that when you are opening files, they open as read-only. In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed. Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="31109-106">**Mój program antywirusowy jest przyczyną je otworzyć tylko do odczytu**</span><span class="sxs-lookup"><span data-stu-id="31109-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="31109-p102">Niektóre programy antywirusowe mogą chronić potencjalnie niebezpiecznych plików przez otwarcie ich jako tylko do odczytu. Należy skontaktować się z dostawcą oprogramowania antywirusowego, aby dowiedzieć się, jak dostosować te ustawienia. BitDefender, na przykład ma zawartość na dodanie wykluczeń aplikacji tutaj: [jak dodać aplikację lub wykluczenia procesu w centrum sterowania Bitdefender](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span><span class="sxs-lookup"><span data-stu-id="31109-p102">Some antivirus programs may protect you from potentially unsafe files by opening them read-only. You may need to check with your antivirus provider to learn how to adjust these settings. BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="31109-110">**Właściwości pliku ustawiono atrybut tylko do odczytu?**</span><span class="sxs-lookup"><span data-stu-id="31109-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="31109-p103">Można sprawdzić właściwości pliku prawym przyciskiem myszy plik i wybierz polecenie Właściwości. Jeśli atrybut tylko do odczytu jest zaznaczone, można usunąć jego zaznaczenie i kliknij OK.</span><span class="sxs-lookup"><span data-stu-id="31109-p103">You can check the file properties by right-clicking on the file and choosing Properties. If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="31109-113">**Zawartość jest w widoku chronionym**</span><span class="sxs-lookup"><span data-stu-id="31109-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="31109-p104">Pliki z Internetu i innych potencjalnie niebezpiecznych lokalizacjach mogą zawierać wirusy, robaki lub inne rodzaje złośliwego oprogramowania, które mogą uszkodzić komputer. Jest to również często z załączników wiadomości e-mail lub pliki pobrane. Aby pomóc w ochronie tego komputera, pliki z lokalizacji tych potencjalnie niebezpieczne są otwierane w widoku chronionym. Za pomocą widoku chronionego, można czytać pliku i wyświetlić jego zawartość przy jednoczesnym zmniejszeniu ryzyka. Aby uzyskać więcej informacji w widoku chronionym i sposobu zmieniania ustawień, w tym artykule: [Co to jest widok chroniony?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="31109-p104">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer. This is also commonly the case with email attachments or files you've downloaded. To help protect your computer, files from these potentially unsafe locations are opened in Protected View. By using Protected View, you can read a file and see its contents while reducing the risks. For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="31109-119">**OneDrive jest zapełniony?**</span><span class="sxs-lookup"><span data-stu-id="31109-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="31109-p105">Jeśli plik jest przechowywany na OneDrive i z przestrzeni magazynowania jest pełny, nie można zapisać dokumentu, dopóki nie są pod przydzielonego miejsca. Wolne miejsce na dysku OneDrive można sprawdzić, klikając ikonę OneDrive w Centrum powiadomień i wybierając polecenie Zarządzanie magazynem, lub możesz przejść do [http://onedrive.live.com](http://onedrive.live.com), zaloguj się i zanotuj ilość zajętego miejsca w dolnym lewym rogu ekranu.</span><span class="sxs-lookup"><span data-stu-id="31109-p105">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space. You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="31109-122">**Urząd jest aktywowany?**</span><span class="sxs-lookup"><span data-stu-id="31109-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="31109-p106">Jeśli pakietu Office nie jest aktywowany lub jeśli Twoja subskrypcja wygasła, może być w trybie tylko do odczytu trybie zmniejszonej funkcjonalności. Szczegółowe informacje na temat aktywacji pakietu Office: [produkt bez licencji i błędów aktywacji pakietu Office](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="31109-p106">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode. For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="31109-125">**Jeśli wszystkie inne źródła zawiodą...**</span><span class="sxs-lookup"><span data-stu-id="31109-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="31109-126">Spróbuj ponownie uruchomić komputer</span><span class="sxs-lookup"><span data-stu-id="31109-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="31109-127">Zainstaluj aktualizacje pakietu Office</span><span class="sxs-lookup"><span data-stu-id="31109-127">Install Office updates</span></span>
    
- <span data-ttu-id="31109-128">Wykonać naprawy w trybie Online pakietu Office</span><span class="sxs-lookup"><span data-stu-id="31109-128">Perform an Online repair of Office</span></span>
    

