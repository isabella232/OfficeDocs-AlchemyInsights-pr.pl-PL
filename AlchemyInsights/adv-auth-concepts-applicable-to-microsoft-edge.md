---
title: Zaawansowane pojęcia dotyczące uwierzytelniania dotyczące przeglądarki Microsoft Edge
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573526"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="34c8b-102">Zaawansowane pojęcia dotyczące uwierzytelniania dotyczące przeglądarki Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="34c8b-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="34c8b-103">Poniżej przedstawiono zaawansowane koncepcje uwierzytelniania dotyczące przeglądarki Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="34c8b-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="34c8b-104">**Aktywne uwierzytelnianie**</span><span class="sxs-lookup"><span data-stu-id="34c8b-104">**Proactive Authentication**</span></span>

<span data-ttu-id="34c8b-105">Po włączeniu zasad [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) program Microsoft Edge będzie próbować aktywnie uwierzytelniać zalogowanych użytkowników za pośrednictwem usług firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="34c8b-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="34c8b-106">W regularnych odstępach czasu będzie używana usługa online, aby sprawdzić, czy jest dostępny zaktualizowany manifest zawierający konfigurację regulującą aktywne uwierzytelnianie.</span><span class="sxs-lookup"><span data-stu-id="34c8b-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="34c8b-107">Korzyści: aktywne uwierzytelnianie umożliwia uwierzytelnianie na najważniejszych usługach, takich jak strona nowej karty pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="34c8b-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="34c8b-108">Ponadto, jeśli usługa Bing jest używana jako wyszukiwarka, Funkcja aktywnego uwierzytelniania zwiększa wydajność paska adresu i pomaga wygenerować wyniki wyszukiwania, które są personalizowane do potrzeb Twojej firmy.</span><span class="sxs-lookup"><span data-stu-id="34c8b-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="34c8b-109">**Windows Hello CredUI dla uwierzytelniania NTLM**</span><span class="sxs-lookup"><span data-stu-id="34c8b-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="34c8b-110">Jeśli funkcja logowania jednokrotnego (SSO) jest niedostępna, gdy witryna sieci Web usiłuje zalogować się do użytkownika za pomocą mechanizmu NTLM lub Negotiate, ta funkcja umożliwi użytkownikowi udostępnianie poświadczeń systemu operacyjnego w witrynie sieci Web i zaspokojenie tego wezwania uwierzytelniania przy użyciu interfejsu użytkownika usługi Windows Hello Credentials.</span><span class="sxs-lookup"><span data-stu-id="34c8b-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="34c8b-111">Ten przepływ logowania będzie wyświetlany tylko w systemie Windows 10 i tylko dla użytkowników, którzy nie korzystają z rejestracji jednokrotnej w protokole NTLM lub negocjacyjnym.</span><span class="sxs-lookup"><span data-stu-id="34c8b-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="34c8b-112">**Automatyczne logowanie przy użyciu zapisanych haseł**</span><span class="sxs-lookup"><span data-stu-id="34c8b-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="34c8b-113">Użytkownicy, którzy zapisują hasła w przeglądarce Microsoft Edge, mogą włączyć automatyczne logowanie do witryn internetowych, w których mają zapisane poświadczenia.</span><span class="sxs-lookup"><span data-stu-id="34c8b-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="34c8b-114">Użytkownicy mogą włączać i wyłączać tę funkcję w edge://settings/passwords, a także można ją skonfigurować w zasadach [Menedżera haseł](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="34c8b-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
