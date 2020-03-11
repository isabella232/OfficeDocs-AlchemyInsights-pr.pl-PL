---
title: Logowanie się do systemu Windows 10 bez użycia hasła
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588290"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="56b54-102">Logowanie się do systemu Windows 10 bez użycia hasła</span><span class="sxs-lookup"><span data-stu-id="56b54-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="56b54-103">Aby uniknąć konieczności wpisywania hasła podczas uruchamiania systemu Windows, zalecamy użycie jednej z opcji bezpiecznego logowania funkcji Windows Hello, takiej jak numer PIN, rozpoznawanie twarzy lub odcisk palca, jeśli są dostępne.</span><span class="sxs-lookup"><span data-stu-id="56b54-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="56b54-104">Jeśli naprawdę chcesz wyłączyć bezpieczne logowanie, zobacz instrukcje "Automatycznie zaloguj się do systemu Windows 10" poniżej.</span><span class="sxs-lookup"><span data-stu-id="56b54-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="56b54-105">**Bezpieczne alternatywy dla hasła do konta w systemie Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="56b54-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="56b54-106">Przejdź do **pozycji Ustawienia > konta > opcje logowania** (lub kliknij [tutaj](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="56b54-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="56b54-107">Zostaną wyświetlone dostępne opcje logowania.</span><span class="sxs-lookup"><span data-stu-id="56b54-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="56b54-108">Na przykład:</span><span class="sxs-lookup"><span data-stu-id="56b54-108">For example:</span></span>

![Opcje logowania.](media/sign-in-options.png)

<span data-ttu-id="56b54-110">Kliknij lub naciśnij jedną z opcji, aby ją skonfigurować.</span><span class="sxs-lookup"><span data-stu-id="56b54-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="56b54-111">Następnym razem, gdy uruchomisz lub odblokujesz system Windows, będziesz mógł użyć nowej opcji zamiast hasła.</span><span class="sxs-lookup"><span data-stu-id="56b54-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="56b54-112">**Automatyczne logowanie się do systemu Windows 10**</span><span class="sxs-lookup"><span data-stu-id="56b54-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="56b54-113">**Uwaga:** Automatyczne logowanie jest wygodne, ale wprowadza zagrożenie bezpieczeństwa, zwłaszcza jeśli komputer jest dostępny dla wielu osób.</span><span class="sxs-lookup"><span data-stu-id="56b54-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="56b54-114">Kliknij lub naciśnij przycisk **Start** na pasku zadań.</span><span class="sxs-lookup"><span data-stu-id="56b54-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="56b54-115">Wpisz **netplwiz** i naciśnij klawisz Enter, aby otworzyć okno Konta użytkowników.</span><span class="sxs-lookup"><span data-stu-id="56b54-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="56b54-116">W **przypadku kont użytkowników**kliknij konto, na które chcesz automatycznie zalogować się podczas uruchamiania systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="56b54-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="56b54-117">Wyczyść pole wyboru "Użytkownicy muszą wprowadzić nazwę użytkownika i hasło, aby korzystać z tego komputera".</span><span class="sxs-lookup"><span data-stu-id="56b54-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Użytkownicy muszą wprowadzić opcję nazwy użytkownika i hasła.](media/users-must-enter-username.png)

5. <span data-ttu-id="56b54-119">Kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="56b54-119">Click **OK**.</span></span> <span data-ttu-id="56b54-120">Zostaniesz poproszony o wprowadzenie i potwierdzenie hasła dla wybranego konta.</span><span class="sxs-lookup"><span data-stu-id="56b54-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="56b54-121">Kliknij **przycisk OK,** aby zakończyć.</span><span class="sxs-lookup"><span data-stu-id="56b54-121">Click **OK** to finish.</span></span> <span data-ttu-id="56b54-122">Przy następnym uruchomieniu systemu Windows 10 automatycznie zaloguje się na wybrane konto.</span><span class="sxs-lookup"><span data-stu-id="56b54-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
