---
title: 1336 RecoverableItems folder jest pełny
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741277"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="598ae-102">Folder Elementy odzyskiwalne jest pełny</span><span class="sxs-lookup"><span data-stu-id="598ae-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="598ae-103">W przypadku skrzynek pocztowych usługi Exchange Online domyślny limit przestrzeni dyskowej dla folderu Elementy odzyskiwalne wynosi 30 GB.</span><span class="sxs-lookup"><span data-stu-id="598ae-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="598ae-104">Limit magazynowania folderu Elementy odzyskiwalne jest automatycznie zwiększany do 100 GB, jeśli skrzynka pocztowa jest umieszczona w ramach wstrzymania, wstrzymania zbierania elektronicznych materiałów dowodowych lub przypisana do zasad przechowywania.</span><span class="sxs-lookup"><span data-stu-id="598ae-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="598ae-105">Jeśli folder Elementy odzyskiwalne osiągnie limit miejsca na przechowywanie, funkcje skrzynek pocztowych będą miały wpływ na następujące sposoby:</span><span class="sxs-lookup"><span data-stu-id="598ae-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="598ae-106">Użytkownik nie może usuwać elementów ze skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="598ae-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="598ae-107">Asystent folderów zarządzanych nie może usuwać elementów na podstawie tagu przechowywania lub ustawień folderu zarządzanego.</span><span class="sxs-lookup"><span data-stu-id="598ae-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="598ae-108">W przypadku skrzynek pocztowych, w których włączono funkcję odzyskiwania pojedynczego elementu lub są one zablokowane, proces ochrony przed zapisem na stronie kopiowania nie obsługuje wersji elementów edytowanych przez użytkownika.</span><span class="sxs-lookup"><span data-stu-id="598ae-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="598ae-109">W przypadku skrzynek pocztowych z włączonym rejestrowaniem inspekcji skrzynek pocztowych nie można zapisywać wpisów dziennika inspekcji skrzynki pocztowej w podfolderze inspekcje w folderze Elementy do odzyskania.</span><span class="sxs-lookup"><span data-stu-id="598ae-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="598ae-110">W przypadku skrzynek pocztowych, które nie są przechowywane, Administratorzy mogą użyć tego `Search-Mailbox -SearchDumpsterOnly -DeleteContent` polecenia w programie Exchange Online PowerShell, aby usunąć elementy z folderu Elementy odzyskiwalne.</span><span class="sxs-lookup"><span data-stu-id="598ae-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="598ae-111">Aby uzyskać więcej informacji, zobacz następujące tematy:</span><span class="sxs-lookup"><span data-stu-id="598ae-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="598ae-112">Wyszukiwanie i usuwanie wiadomości</span><span class="sxs-lookup"><span data-stu-id="598ae-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="598ae-113">Wyszukiwanie — Skrzynka pocztowa</span><span class="sxs-lookup"><span data-stu-id="598ae-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="598ae-114">W przypadku skrzynek pocztowych zablokowanych Administratorzy muszą usunąć blokadę, zanim będą mogli usunąć elementy z folderu Elementy odzyskiwalne.</span><span class="sxs-lookup"><span data-stu-id="598ae-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="598ae-115">Aby uzyskać więcej informacji, zobacz [usuwanie elementów w folderze Elementy odzyskiwalne w skrzynkach pocztowych opartych na chmurze](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="598ae-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="598ae-116">Aby zapobiec pełnemu zapełnieniu folderu Elementy możliwe, Administratorzy mogą zwiększyć limit magazynowania folderu Elementy odzyskiwalne dla skrzynek pocztowych zablokowanych i skonfigurować zasady przechowywania skrzynek pocztowych, które będą przenosić elementy z folderu Elementy odzyskiwalne do archiwum Skrzynka pocztowa użytkownika.</span><span class="sxs-lookup"><span data-stu-id="598ae-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="598ae-117">Zobacz [zwiększanie przydziału elementów odzyskiwalnych dla skrzynek pocztowych zablokowanych](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="598ae-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
