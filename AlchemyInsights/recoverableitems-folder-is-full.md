---
title: 1336 Folder RecoverableItems jest pełny
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720262"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="a49ff-102">Folder Elementy do odzyskania jest pełny</span><span class="sxs-lookup"><span data-stu-id="a49ff-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="a49ff-103">W przypadku skrzynek pocztowych usługi Exchange Online domyślny limit miejsca dla folderu Elementy możliwe do odzyskania wynosi 30 GB.</span><span class="sxs-lookup"><span data-stu-id="a49ff-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="a49ff-104">Limit magazynowania folderu Elementy możliwe do odzyskania jest automatycznie zwiększany do 100 GB, jeśli skrzynka pocztowa zostanie umieszczona w wstrzymaniu postępowania sądowego, blokadzie zbierania elektronicznych materiałów dowodowych lub jest przypisana do zasad przechowywania.</span><span class="sxs-lookup"><span data-stu-id="a49ff-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="a49ff-105">Gdy folder Elementy możliwe do odzyskania osiągnie limit magazynowania, działanie skrzynki pocztowej jest zagrożone w następujący sposób:</span><span class="sxs-lookup"><span data-stu-id="a49ff-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="a49ff-106">Użytkownik nie może usuwać elementów ze skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="a49ff-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="a49ff-107">Asystent folderów zarządzanych nie może usuwać elementów na podstawie tagu przechowywania lub ustawień folderu zarządzanego.</span><span class="sxs-lookup"><span data-stu-id="a49ff-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="a49ff-108">W przypadku skrzynek pocztowych, w których włączona lub wstrzymana jest funkcja odzyskiwania pojedynczego elementu, proces ochrony strony kopiowania przy zapisie nie może obsługiwać wersji elementów edytowanych przez użytkownika.</span><span class="sxs-lookup"><span data-stu-id="a49ff-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="a49ff-109">W przypadku skrzynek pocztowych z włączonym rejestrowaniem inspekcji skrzynek pocztowych w podfolderze Inspekcje w folderze Elementy podlegające odzyskiwalnej nie można zapisywać żadnych wpisów dziennika inspekcji skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="a49ff-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="a49ff-110">W przypadku skrzynek pocztowych, które nie są `Search-Mailbox -SearchDumpsterOnly -DeleteContent` wstrzymane, administratorzy mogą użyć polecenia programu Exchange Online PowerShell do usuwania elementów w folderze Elementy do odzyskania.</span><span class="sxs-lookup"><span data-stu-id="a49ff-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="a49ff-111">Aby uzyskać więcej informacji, zobacz następujące tematy:</span><span class="sxs-lookup"><span data-stu-id="a49ff-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="a49ff-112">Wyszukiwanie i usuwanie wiadomości</span><span class="sxs-lookup"><span data-stu-id="a49ff-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="a49ff-113">Szukaj-Skrzynka pocztowa</span><span class="sxs-lookup"><span data-stu-id="a49ff-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="a49ff-114">W przypadku wstrzymanych skrzynek pocztowych administratorzy muszą usunąć blokadę, zanim będą mogli usunąć elementy z folderu Elementy do odzyskania.</span><span class="sxs-lookup"><span data-stu-id="a49ff-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="a49ff-115">Aby uzyskać więcej informacji, zobacz [Usuwanie elementów w folderze Elementy możliwe do odzyskania w chmurowych skrzynkach pocztowych wstrzymanych](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="a49ff-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="a49ff-116">Aby zapobiec zapełnieniu folderu Elementy do odzyskania, administratorzy mogą zwiększyć limit magazynowania folderu Elementy odzyskiwalne dla wstrzymanych skrzynek pocztowych i skonfigurować zasady przechowywania skrzynek pocztowych, które przenoszą elementy z folderu Elementy do odzyskania do archiwalnej skrzynki pocztowej użytkownika.</span><span class="sxs-lookup"><span data-stu-id="a49ff-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="a49ff-117">Zobacz [Zwiększanie przydziału elementów do odzyskania dla wstrzymanych skrzynek pocztowych](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="a49ff-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
