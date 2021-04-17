---
title: Rozwiązywanie problemów z aplikacjami platformy Microsoft 365 Nie można odnaleźć skojarzonego komunikatu z licencjami pakietu Office
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
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816498"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="e766d-102">Naprawianie komunikatu "Nie można znaleźć skojarzonych licencji pakietu Office" dla aplikacji platformy Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e766d-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="e766d-103">Jeśli zostanie wyświetlony ten komunikat, spróbuj wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="e766d-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="e766d-104">Sprawdź ustawienia zapory, oprogramowania antywirusowego i serwera proxy, aby upewnić się, że nie blokują one dostępu do Internetu do aplikacji platformy Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e766d-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="e766d-105">Zobacz Adresy URL i zakresy adresów [IP platformy Microsoft 365.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="e766d-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="e766d-106">Usuń i [ponownie przyzmij licencję pakietu Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) dla użytkownika, którego dotyczy problem.</span><span class="sxs-lookup"><span data-stu-id="e766d-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="e766d-107">Otwórz aplikację pakietu Office i [wyloguj się](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) z istniejących kont użytkowników.</span><span class="sxs-lookup"><span data-stu-id="e766d-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="e766d-108">Przejdź do pozycji Ustawienia systemu Windows > **Konta**  >  **e-& konta e-mail** i usuń wszystkie konta służbowe z wyjątkiem kont, których dotyczy problem.</span><span class="sxs-lookup"><span data-stu-id="e766d-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="e766d-109">Przejdź do pozycji Ustawienia systemu Windows > **Konta** Uzyskaj dostęp do konta służbowego i odłącz wszystkie konta służbowe z wyjątkiem konta, którego  >  dotyczy problem.</span><span class="sxs-lookup"><span data-stu-id="e766d-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="e766d-110">Zresetuj stan aktywacji pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="e766d-110">Reset the Office activation state.</span></span> <span data-ttu-id="e766d-111">[Dowiedz się, jak to zrobić](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="e766d-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="e766d-112">[Zaloguj się przy](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) użyciu konta użytkownika, którego dotyczy problem.</span><span class="sxs-lookup"><span data-stu-id="e766d-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="e766d-113">Aby uzyskać dodatkowe rozwiązania problemów, zobacz [Błędy "Produkt bez licencji" i błędy aktywacji w psłudze Office.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="e766d-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>