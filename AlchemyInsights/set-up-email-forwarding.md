---
title: Konfigurowanie przesyłania dalej poczty e-mail
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "20"
- "1200004"
ms.assetid: 15abf81d-5c5d-49da-ac81-1b4daa1809f6
ms.openlocfilehash: a7fba259375c667ff2e0f14a03972e102468cd27
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51787147"
---
# <a name="check-the-email-forwarding-settings-for-a-mailbox"></a><span data-ttu-id="a396f-102">Sprawdzanie ustawień przesyłania dalej poczty e-mail dla skrzynki pocztowej</span><span class="sxs-lookup"><span data-stu-id="a396f-102">Check the email forwarding settings for a mailbox</span></span>

<span data-ttu-id="a396f-103">Po pierwsze, przesyłanie dalej poczty e-mail musi być włączone na poziomie dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="a396f-103">Firstly, email forwarding has to be enabled on the tenant level.</span></span> <span data-ttu-id="a396f-104">Jeśli w skrzynce pocztowej nie działa funkcja przesyłania dalej poczty e-mail (jest wyświetlany komunikat o błędzie "Odmowa dostępu **550 5.7.520,** Oznacza to, że Twoja organizacja nie zezwala na przesyłanie dalej zewnętrzne" — zobacz Kontrolowanie automatycznego zewnętrznego przesyłania dalej wiadomości e-mail na platformie [Microsoft 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="a396f-104">If you have set up email forwarding on a mailbox, but it is not working (you get an error **"550 5.7.520 Access denied, Your organization does not allow external forwarding"**) please see [Control automatic external email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide).</span></span>

<span data-ttu-id="a396f-105">Sprawdzanie ustawień przesyłania dalej wiadomości e-mail w skrzynce pocztowej jest łatwe!</span><span class="sxs-lookup"><span data-stu-id="a396f-105">It's easy to verify the email forwarding settings on a mailbox!</span></span> <span data-ttu-id="a396f-106">Po prostu wykonaj poniższe czynności.</span><span class="sxs-lookup"><span data-stu-id="a396f-106">Just follow these steps.</span></span>
  
> <span data-ttu-id="a396f-107">Jeśli jest to skrzynka pocztowa użytkownika, przejdź do **witryny Aktywni** użytkownicy użytkownicy i wybierz użytkownika, którego skrzynkę \>  pocztową przesyłasz dalej.</span><span class="sxs-lookup"><span data-stu-id="a396f-107">If this is a user mailbox, go to **Users** \> **Active users** and select the user whose mailbox you're forwarding.</span></span> <span data-ttu-id="a396f-108">Na karcie **Poczta** wybierz pozycję **Zarządzaj przesyłaniem dalej poczty e-mail**.</span><span class="sxs-lookup"><span data-stu-id="a396f-108">On the **Mail** tab, select **Manage email forwarding**.</span></span>

> <span data-ttu-id="a396f-109">Jeśli jest to udostępniona skrzynka pocztowa, przejdź do **grupy** Udostępnione skrzynki pocztowe i wybierz udostępnioną skrzynkę pocztową przesyłaną \>  dalej.</span><span class="sxs-lookup"><span data-stu-id="a396f-109">If this is a shared mailbox, go to **Groups** \> **Shared mailboxes** and select the shared mailbox you're forwarding.</span></span> <span data-ttu-id="a396f-110">Wybierz pozycję **Edytuj, aby** przesyłać dalej wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="a396f-110">Select **Edit** for email forwarding.</span></span>

<span data-ttu-id="a396f-111">Aby uzyskać więcej informacji, zobacz [Konfigurowanie przesyłania dalej poczty e-mail na platformie Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)</span><span class="sxs-lookup"><span data-stu-id="a396f-111">For more information, see [Configure email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>
  
<span data-ttu-id="a396f-112">Aby wysłać instrukcje do użytkowników w celu skonfigurowania przesyłania dalej poczty e-mail we własnych skrzynkach pocztowych, wskaż im temat Przesyłanie dalej wiadomości e-mail z [platformy Microsoft 365 na inne konto e-mail.](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e)</span><span class="sxs-lookup"><span data-stu-id="a396f-112">To send instructions to your users so they can set up email forwarding on their own mailboxes, point them to [Forward email from Microsoft 365 to another email account](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e).</span></span> <span data-ttu-id="a396f-113">Pamiętaj, że możesz przesyłać dalej tylko na jeden adres e-mail.</span><span class="sxs-lookup"><span data-stu-id="a396f-113">Please note that you can forward to only one email address.</span></span> <span data-ttu-id="a396f-114">Jeśli musisz skonfigurować przesyłanie dalej do grupy osób, utwórz listę dystrybucyjną (w obszarze Grupy **),** dodaj do tej grupy użytkowników, a następnie skonfiguruj przesyłanie dalej do tej grupy.</span><span class="sxs-lookup"><span data-stu-id="a396f-114">If you need to set up forwarding to a group of people, create a distribution list (under **Groups**), add your users to it, and then configure forwarding to that group.</span></span>
  
<span data-ttu-id="a396f-115">Pracownik odchodzi z Ciebie?</span><span class="sxs-lookup"><span data-stu-id="a396f-115">Do you have an employee leaving?</span></span> <span data-ttu-id="a396f-116">Zobacz [Usuwanie byłego pracownika z platformy Microsoft 365,](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee) aby uzyskać zalecane instrukcje.</span><span class="sxs-lookup"><span data-stu-id="a396f-116">See [Remove a former employee from Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee) for the recommended steps.</span></span>