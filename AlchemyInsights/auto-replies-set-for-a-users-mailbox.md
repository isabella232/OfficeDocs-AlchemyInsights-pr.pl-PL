---
title: Ustawianie automatycznych odpowiedzi dla skrzynki pocztowej
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820944"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="8eb3c-102">Ustawianie automatycznych odpowiedzi dla skrzynki pocztowej użytkownika</span><span class="sxs-lookup"><span data-stu-id="8eb3c-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="8eb3c-103">**Metoda 1**</span><span class="sxs-lookup"><span data-stu-id="8eb3c-103">**Method 1**</span></span>

1. <span data-ttu-id="8eb3c-104">Zaloguj się do portalu platformy Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="8eb3c-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="8eb3c-105">Przejdź do pozycji **Użytkownicy > Aktywni użytkownicy** (lub **Grupy > Udostępnione skrzynki pocztowe** w przypadku konfigurowania ustawień dla udostępnionej skrzynki).</span><span class="sxs-lookup"><span data-stu-id="8eb3c-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="8eb3c-106">Wybierz użytkownika, który ma skrzynkę pocztową programu Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="8eb3c-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="8eb3c-107">W menu wysuwanym po prawej stronie przejdź do pozycji **Ustawienia poczty > Odpowiedzi automatyczne** (w przypadku udostępnionej skrzynki pocztowej wystarczy kliknąć pozycję **Odpowiedzi automatyczne** w menu wysuwanym).</span><span class="sxs-lookup"><span data-stu-id="8eb3c-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="8eb3c-108">**Metoda 2**</span><span class="sxs-lookup"><span data-stu-id="8eb3c-108">**Method 2**</span></span>

1. <span data-ttu-id="8eb3c-109">Zaloguj się do portalu administracyjnego platformy Microsoft 365 przy użyciu poświadczeń administratora usługi.</span><span class="sxs-lookup"><span data-stu-id="8eb3c-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="8eb3c-110">Rozwiń pozycję **Centra administracyjne**, a następnie kliknij pozycję **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="8eb3c-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="8eb3c-111">Kliknij obraz w prawym górnym rogu, kliknij pozycję **Inny użytkownik**, a następnie wybierz skrzynkę pocztową użytkownika, którą chcesz zmienić.</span><span class="sxs-lookup"><span data-stu-id="8eb3c-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="8eb3c-112">Po lewej stronie wybierz pozycję **Opcje**, kliknij pozycję **Organizuj wiadomości e-mail**, a następnie kliknij pozycję **Odpowiedzi automatyczne.**</span><span class="sxs-lookup"><span data-stu-id="8eb3c-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="8eb3c-113">**Metoda 3**</span><span class="sxs-lookup"><span data-stu-id="8eb3c-113">**Method 3**</span></span>

<span data-ttu-id="8eb3c-114">Uruchom następujące polecenie cmdlet w module programu PowerShell dla usługi Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="8eb3c-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="8eb3c-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="8eb3c-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="8eb3c-116">Aby uzyskać więcej informacji o tym poleceniu cmdlet, zobacz [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="8eb3c-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
