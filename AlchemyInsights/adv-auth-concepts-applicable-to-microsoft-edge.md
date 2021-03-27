---
title: Pojęcia zaawansowanego uwierzytelniania dotyczące programu Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398595"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="fed25-102">Pojęcia zaawansowanego uwierzytelniania dotyczące programu Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="fed25-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="fed25-103">Poniżej przedstawiono pojęcia zaawansowanego uwierzytelniania, które mają zastosowanie do programu Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="fed25-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="fed25-104">**Aktywne uwierzytelnianie**</span><span class="sxs-lookup"><span data-stu-id="fed25-104">**Proactive Authentication**</span></span>

<span data-ttu-id="fed25-105">Po włączeniu zasad [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) przeglądarka Microsoft Edge będzie próbować aktywnie uwierzytelniać użytkowników zalogowanych za pośrednictwem usług firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fed25-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="fed25-106">W regularnych odstępach czasu usługa online będzie sprawdzać, czy w pliku manifestu nie ma zaktualizowanego pliku manifestu, który zawiera konfigurację, która działa proaktywnie.</span><span class="sxs-lookup"><span data-stu-id="fed25-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="fed25-107">Korzyści: Aktywne uwierzytelnianie umożliwia uwierzytelnianie w najważniejszych usługach, takich jak strona nowej karty pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="fed25-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="fed25-108">Ponadto jeśli wyszukiwarka jest używana za pomocą usługi Bing, aktywne uwierzytelnianie zwiększa wydajność paska adresu i pomaga generować wyniki wyszukiwania spersonalizowane do potrzeb Twojej firmy.</span><span class="sxs-lookup"><span data-stu-id="fed25-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="fed25-109">**Funkcja CredUI funkcji Windows Hello do uwierzytelniania NTLM**</span><span class="sxs-lookup"><span data-stu-id="fed25-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="fed25-110">Jeśli logowanie jednokrotne (SSO) nie jest dostępne, gdy witryna internetowa próbuje zalogować użytkownika za pośrednictwem mechanizmu NTLM lub Negotiate, ta funkcja umożliwi użytkownikowi udostępnianie poświadczeń systemu operacyjnego witrynie internetowej i spełnienie wyzwania związanego z uwierzytelnianiem przy użyciu interfejsu użytkownika Wer. Windows Hello.</span><span class="sxs-lookup"><span data-stu-id="fed25-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="fed25-111">Ten przepływ logowania jest wyświetlany tylko w systemie Windows 10 i tylko dla użytkowników, którzy nie uzyskają logowania jednokrotnego podczas NTLM lub wyzwania Wynegocjuj.</span><span class="sxs-lookup"><span data-stu-id="fed25-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="fed25-112">**Automatyczne logowanie przy użyciu zapisanych haseł**</span><span class="sxs-lookup"><span data-stu-id="fed25-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="fed25-113">Użytkownicy, którzy zapisują hasła w programie Microsoft Edge, mogą włączyć automatyczne logowanie się do witryn internetowych, w których zapisano poświadczenia.</span><span class="sxs-lookup"><span data-stu-id="fed25-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="fed25-114">Użytkownicy mogą włączać i wyłączać tę funkcję w edge://settings/passwords, a także skonfigurować ją w zasadach [menedżera](https://go.microsoft.com/fwlink/?linkid=2134622) haseł.</span><span class="sxs-lookup"><span data-stu-id="fed25-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
