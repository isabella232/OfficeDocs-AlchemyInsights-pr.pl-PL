---
title: Ustawianie automatycznych odpowiedzi dla skrzynki pocztowej
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788892"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="7898d-102">Ustawianie automatycznych odpowiedzi dla skrzynki pocztowej użytkownika</span><span class="sxs-lookup"><span data-stu-id="7898d-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="7898d-103">**Metoda 1**</span><span class="sxs-lookup"><span data-stu-id="7898d-103">**Method 1**</span></span>

1. <span data-ttu-id="7898d-104">Zaloguj się do portalu platformy Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7898d-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="7898d-105">Przejdź do pozycji **Użytkownicy > Aktywni użytkownicy** (lub **Grupy > Udostępnione skrzynki pocztowe** w przypadku konfigurowania ustawień dla udostępnionej skrzynki).</span><span class="sxs-lookup"><span data-stu-id="7898d-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="7898d-106">Wybierz użytkownika, który ma skrzynkę pocztową programu Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="7898d-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="7898d-107">W menu wysuwanym po prawej stronie przejdź do pozycji **Ustawienia poczty > Odpowiedzi automatyczne** (w przypadku udostępnionej skrzynki pocztowej wystarczy kliknąć pozycję **Odpowiedzi automatyczne** w menu wysuwanym).</span><span class="sxs-lookup"><span data-stu-id="7898d-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="7898d-108">**Metoda 2**</span><span class="sxs-lookup"><span data-stu-id="7898d-108">**Method 2**</span></span>

1. <span data-ttu-id="7898d-109">Zaloguj się do portalu administracyjnego platformy Microsoft 365 przy użyciu poświadczeń administratora usługi.</span><span class="sxs-lookup"><span data-stu-id="7898d-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="7898d-110">Rozwiń pozycję **Centra administracyjne**, a następnie kliknij pozycję **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="7898d-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="7898d-111">Kliknij obraz w prawym górnym rogu, kliknij pozycję **Inny użytkownik**, a następnie wybierz skrzynkę pocztową użytkownika, którą chcesz zmienić.</span><span class="sxs-lookup"><span data-stu-id="7898d-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="7898d-112">Po lewej stronie wybierz pozycję **Opcje**, kliknij pozycję **Organizuj wiadomości e-mail**, a następnie kliknij pozycję **Odpowiedzi automatyczne.**</span><span class="sxs-lookup"><span data-stu-id="7898d-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="7898d-113">**Metoda 3**</span><span class="sxs-lookup"><span data-stu-id="7898d-113">**Method 3**</span></span>

<span data-ttu-id="7898d-114">Uruchom następujące polecenie cmdlet w module programu PowerShell dla usługi Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="7898d-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="7898d-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="7898d-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="7898d-116">Aby uzyskać więcej informacji o tym poleceniu cmdlet, zobacz [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="7898d-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
