---
title: Korygowanie błędu „Aplikacja nie została wykryta”
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
- "9000171"
- "1712"
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836361"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="c35e5-102">Korygowanie błędu „Aplikacja nie została wykryta”</span><span class="sxs-lookup"><span data-stu-id="c35e5-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="c35e5-103">Błąd instalacji aplikacji „Aplikacja nie została wykryta po pomyślnym zakończeniu instalacji” zgłaszany przez usługę Intune może wystąpić na wszystkich głównych platformach systemu operacyjnego (Windows, iOS i Android).</span><span class="sxs-lookup"><span data-stu-id="c35e5-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="c35e5-104">Najczęstsze scenariusze, w których jest generowany ten błąd, są następujące:</span><span class="sxs-lookup"><span data-stu-id="c35e5-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="c35e5-105">Aplikacja została zaktualizowana poza usługą Intune (ze sklepu z aplikacjami innego producenta) po wdrożeniu początkowym.</span><span class="sxs-lookup"><span data-stu-id="c35e5-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="c35e5-106">Na przykład niektóre aplikacje, takie jak Google Chrome, mogą wykonywać aktualizacje automatyczne.</span><span class="sxs-lookup"><span data-stu-id="c35e5-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="c35e5-107">Użytkownik odinstalował aplikację po początkowej instalacji.</span><span class="sxs-lookup"><span data-stu-id="c35e5-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="c35e5-108">Aby rozwiązać ten problem, najpierw sprawdź dotknięte problemem urządzenia w celu ustalenia, z jakim scenariuszem tego błędu masz do czynienia.</span><span class="sxs-lookup"><span data-stu-id="c35e5-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="c35e5-109">Jeśli aplikacja została zaktualizowana poza usługą Intune, dla wdrożenia aplikacji można ustawić ignorowanie wersji aplikacji.</span><span class="sxs-lookup"><span data-stu-id="c35e5-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="c35e5-110">W tym celu w obszarze **Konfiguracja aplikacji > Informacje o aplikacji** ustaw dla opcji **Ignoruj wersję aplikacji** wartość **Tak**.</span><span class="sxs-lookup"><span data-stu-id="c35e5-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="c35e5-111">W przypadku kierowania do klienta być może warto wdrożyć aplikację jako „wymaganą”, aby upewnić się, że zostanie wdrożona najnowsza wersja.</span><span class="sxs-lookup"><span data-stu-id="c35e5-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="c35e5-112">Natomiast na platformie iOS możliwe jest używanie funkcji **automatycznej aktualizacji** skojarzonej z programem zakupów grupowych Apple Volume Purchase Program, który można skonfigurować tak, aby automatycznie aktualizować aplikacje do nowych wersji po ich udostępnieniu.</span><span class="sxs-lookup"><span data-stu-id="c35e5-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="c35e5-113">Aby uzyskać więcej informacji na temat rozwiązywania problemów z instalacją aplikacji, zobacz [Rozwiązywanie problemów z instalacją aplikacji](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="c35e5-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
