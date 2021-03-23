---
title: Importowanie i eksportowanie z Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037252"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="266dc-102">Importowanie i eksportowanie z Yammer</span><span class="sxs-lookup"><span data-stu-id="266dc-102">Import and export from Yammer</span></span>

<span data-ttu-id="266dc-103">**Importowanie**</span><span class="sxs-lookup"><span data-stu-id="266dc-103">**Import**</span></span>

<span data-ttu-id="266dc-104">Opcje importowania użytkowników różnią się w zależności od tego, Yammer jest w trybie natywnym platformy [Microsoft 365.](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)</span><span class="sxs-lookup"><span data-stu-id="266dc-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="266dc-105">Tryb **nienatywny:** Użytkowników można importować do grup przy użyciu pozycji Dodaj z książki adresowej [(ograniczenie](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) do 100 użytkowników) w ustawieniach grupy lub do sieci przy użyciu funkcji aktualizacji zbiorczej w obrębie administratora sieci. [](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users)</span><span class="sxs-lookup"><span data-stu-id="266dc-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="266dc-106">**Tryb natywny:** Członkostwo w grupie i operacje członkostwa w sieci powinny być wykonywane z portalu administracyjnego [platformy Microsoft 365,](https://docs.microsoft.com/microsoft-365/admin/add-users)portalu [usługi Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)lub innej opcji usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="266dc-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="266dc-107">Sieci w trybie natywnym nie mają już dostępu do aktualizacji zbiorczej i innych starszych funkcji.</span><span class="sxs-lookup"><span data-stu-id="266dc-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="266dc-108">Yammer nie było obsługiwane importowanie zawartości z poziomu administratora sieci nawet wtedy, gdy funkcja eksportowania danych była używana w innej sieci.</span><span class="sxs-lookup"><span data-stu-id="266dc-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="266dc-109">Zawartość może być publikowana ponownie przez rozwiązania partnerów lub Yammer interfejsów API rest.</span><span class="sxs-lookup"><span data-stu-id="266dc-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="266dc-110">**Eksportowanie**</span><span class="sxs-lookup"><span data-stu-id="266dc-110">**Export**</span></span>

<span data-ttu-id="266dc-111">[Eksportowanie danych sieciowych przez administratora](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) sieci zezwala na eksportowanie zawartości z Yammer sieci, w tym wiadomości i plików.</span><span class="sxs-lookup"><span data-stu-id="266dc-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="266dc-112">Załączniki mogą być bardzo duże, co spowoduje, że eksport będzie się odbywał bardzo długo.</span><span class="sxs-lookup"><span data-stu-id="266dc-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="266dc-113">Zalecamy eksportowanie aktywnych sieci przy użyciu interfejsu [API eksportu danych](https://developer.yammer.com/docs/data-export-api) w fragmentach według dnia lub tygodnia.</span><span class="sxs-lookup"><span data-stu-id="266dc-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="266dc-114">Pomoc techniczna firmy Microsoft nie udostępni w tym celu skryptów niestandardowych.</span><span class="sxs-lookup"><span data-stu-id="266dc-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="266dc-115">W celu [wyeksportowania](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) zawartości dla pojedynczego użytkownika istnieje osobny eksport RODO.</span><span class="sxs-lookup"><span data-stu-id="266dc-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>