---
title: Logowanie się do systemu Windows 10 bez użycia hasła
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719963"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="bf876-102">Logowanie się do systemu Windows 10 bez użycia hasła</span><span class="sxs-lookup"><span data-stu-id="bf876-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="bf876-103">Aby uniknąć konieczności wpisywania hasła podczas uruchamiania systemu Windows, zalecamy używanie jednej z bezpiecznych opcji logowania funkcji Windows Hello, takich jak kod PIN, rozpoznawanie twarzy lub odcisk cyfrowy, jeśli są one dostępne.</span><span class="sxs-lookup"><span data-stu-id="bf876-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="bf876-104">Jeśli naprawdę chcesz wyłączyć bezpieczne logowanie, zobacz poniższe instrukcje "automatyczne logowanie do systemu Windows 10" poniżej.</span><span class="sxs-lookup"><span data-stu-id="bf876-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="bf876-105">**Zabezpieczanie hasła konta w usłudze Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="bf876-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="bf876-106">Przejdź do obszaru **ustawienia > konta > opcji logowania** (lub kliknij [tutaj](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="bf876-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="bf876-107">Zostaną wyświetlone dostępne opcje logowania.</span><span class="sxs-lookup"><span data-stu-id="bf876-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="bf876-108">Przykład:</span><span class="sxs-lookup"><span data-stu-id="bf876-108">For example:</span></span>

![Opcje logowania.](media/sign-in-options.png)

<span data-ttu-id="bf876-110">Kliknij lub naciśnij dowolną z opcji, aby ją skonfigurować.</span><span class="sxs-lookup"><span data-stu-id="bf876-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="bf876-111">Gdy następnym razem uruchomisz lub odblokowuje system Windows, będziesz mieć możliwość skorzystania z opcji Nowy zamiast hasła.</span><span class="sxs-lookup"><span data-stu-id="bf876-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="bf876-112">**Automatyczne logowanie w systemie Windows 10**</span><span class="sxs-lookup"><span data-stu-id="bf876-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="bf876-113">**Uwaga**: automatyczne logowanie jest wygodne, ale stanowi zagrożenie bezpieczeństwa, szczególnie wtedy, gdy komputer jest dostępny dla wielu osób.</span><span class="sxs-lookup"><span data-stu-id="bf876-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="bf876-114">Kliknij lub naciśnij przycisk **Start** na pasku zadań.</span><span class="sxs-lookup"><span data-stu-id="bf876-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="bf876-115">Wpisz **netplwiz** i naciśnij klawisz ENTER, aby otworzyć okno konta użytkowników.</span><span class="sxs-lookup"><span data-stu-id="bf876-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="bf876-116">W obszarze **konta użytkowników**kliknij konto, z którym chcesz automatycznie logować się podczas uruchamiania systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="bf876-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="bf876-117">Wyczyść pole wyboru "użytkownicy muszą wprowadzić nazwę użytkownika i hasło, aby używać tego komputera".</span><span class="sxs-lookup"><span data-stu-id="bf876-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Użytkownicy muszą wprowadzić odpowiednią nazwę użytkownika i hasło.](media/users-must-enter-username.png)

5. <span data-ttu-id="bf876-119">Kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="bf876-119">Click **OK**.</span></span> <span data-ttu-id="bf876-120">Zostanie wyświetlony monit o wprowadzenie i potwierdzenie hasła dla wybranego konta.</span><span class="sxs-lookup"><span data-stu-id="bf876-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="bf876-121">Kliknij przycisk **OK** , aby zakończyć.</span><span class="sxs-lookup"><span data-stu-id="bf876-121">Click **OK** to finish.</span></span> <span data-ttu-id="bf876-122">Następnym razem po uruchomieniu systemu Windows 10 zostanie automatycznie zalogowanie się do wybranego konta.</span><span class="sxs-lookup"><span data-stu-id="bf876-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
