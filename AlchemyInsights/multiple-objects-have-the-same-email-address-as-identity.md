---
title: Wiele obiektów ma ten sam adres e-mail co tożsamość
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439715"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="b52dd-102">Wiele obiektów ma ten sam adres e-mail co tożsamość</span><span class="sxs-lookup"><span data-stu-id="b52dd-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="b52dd-103">**Wiele obiektów**</span><span class="sxs-lookup"><span data-stu-id="b52dd-103">**Multiple objects**</span></span>

<span data-ttu-id="b52dd-104">Jedną z typowych przyczyn tego błędu jest nie jest możliwe do routowania żądania programu Outlook Web Access poprawnie w obecności wielu obiektów o tym samym adresie e-mail jako tożsamości.</span><span class="sxs-lookup"><span data-stu-id="b52dd-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="b52dd-105">Aby znaleźć te obiekty, uruchom następujące polecenia:</span><span class="sxs-lookup"><span data-stu-id="b52dd-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="b52dd-106">· Odbiorca pobierz<email address></span><span class="sxs-lookup"><span data-stu-id="b52dd-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="b52dd-107">· Pobierz użytkownika<email address></span><span class="sxs-lookup"><span data-stu-id="b52dd-107">· Get-User <email address></span></span>

<span data-ttu-id="b52dd-108">· Get-User <email address> -SoftDeletedUżytnik</span><span class="sxs-lookup"><span data-stu-id="b52dd-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="b52dd-109">· Kontakt z użytkownikami<email address></span><span class="sxs-lookup"><span data-stu-id="b52dd-109">· Get-Contact <email address></span></span>

<span data-ttu-id="b52dd-110">· Get-Mailbox <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="b52dd-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="b52dd-111">· Get-Skrzynka pocztowa <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="b52dd-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="b52dd-112">· Get-Skrzynka pocztowa <email address> -Nieaktywna skrzynka pocztowaTylko</span><span class="sxs-lookup"><span data-stu-id="b52dd-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="b52dd-113">Aby rozwiązać ten problem, usuń wiele obiektów o tej samej tożsamości poczty e-mail i upewnij się, że istnieje pojedynczy obiekt o określonej tożsamości wiadomości e-mail i że jego typem adresata jest UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="b52dd-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="b52dd-114">**Ten sam adres jest używany w skrzynkach pocztowych firm i konsumentów**</span><span class="sxs-lookup"><span data-stu-id="b52dd-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="b52dd-115">Inną przyczyną jest, gdy ten sam adres jest używany dla skrzynek pocztowych firmy i konsumentów.</span><span class="sxs-lookup"><span data-stu-id="b52dd-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="b52dd-116">W takim przypadku użytkownik musi zmienić swój podstawowy alias konsumenta, dopóki Cafe obsługuje ten scenariusz.</span><span class="sxs-lookup"><span data-stu-id="b52dd-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="b52dd-117">Jest to trwały błąd, który nie zniknie bez interwencji.</span><span class="sxs-lookup"><span data-stu-id="b52dd-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="b52dd-118">Aby uzyskać szczegółowe informacje, zobacz [Zmienianie adresu e-mail lub numeru telefonu konta Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="b52dd-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>