---
title: Błędy tworzenia zdarzeń na żywo w usłudze Yammer
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
- "9002495"
- "5112"
ms.openlocfilehash: 383943d670c935403fb7f4466a72474120e27e7a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825525"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="ca1ac-102">Błędy tworzenia zdarzeń na żywo w usłudze Yammer</span><span class="sxs-lookup"><span data-stu-id="ca1ac-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="ca1ac-103">**Tworzenie zdarzenia na żywo w usłudze Yammer**</span><span class="sxs-lookup"><span data-stu-id="ca1ac-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="ca1ac-104">W usłudze Yammer zostanie wyświetlona opcja umożliwiająca tworzenie zdarzenia na żywo przez cały czas.</span><span class="sxs-lookup"><span data-stu-id="ca1ac-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="ca1ac-105">W niektórych przypadkach może się zdarzyć, że użytkownik nie spełnił wymagań wstępnych związanych z tworzeniem zdarzenia na żywo i wystąpił błąd podczas próby jego utworzenia.</span><span class="sxs-lookup"><span data-stu-id="ca1ac-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="ca1ac-106">Poniższe elementy opisują typowe przyczyny tego problemu i dostarczają sposobów ich rozwiązania dla użytkowników końcowych.</span><span class="sxs-lookup"><span data-stu-id="ca1ac-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="ca1ac-107">**Kto może tworzyć zdarzenia na żywo**</span><span class="sxs-lookup"><span data-stu-id="ca1ac-107">**Who can create live events**</span></span>
- <span data-ttu-id="ca1ac-108">Licencja usługi Office 365 Enterprise E1, E3 lub E5 bądź Office 365 A3 lub A5.</span><span class="sxs-lookup"><span data-stu-id="ca1ac-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="ca1ac-109">Uprawnienie do tworzenia wydarzeń na żywo w centrum administracyjnym aplikacji Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ca1ac-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="ca1ac-110">Uprawnienie do tworzenia wydarzeń na żywo w usłudze Microsoft Stream (w przypadku wydarzeń realizowanych za pomocą zewnętrznych usług lub urządzeń do obsługi transmisji).</span><span class="sxs-lookup"><span data-stu-id="ca1ac-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="ca1ac-111">Pełne członkostwo w zespole wewnątrz organizacji (nie możesz być gościem ani użytkownikiem z innej organizacji).</span><span class="sxs-lookup"><span data-stu-id="ca1ac-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="ca1ac-112">Włączone funkcje planowania spotkań prywatnych, udostępniania ekranu oraz udostępniania wideo IP w zasadach spotkań aplikacji Teams.</span><span class="sxs-lookup"><span data-stu-id="ca1ac-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="ca1ac-113">**Zasady tworzenia zdarzeń na żywo**</span><span class="sxs-lookup"><span data-stu-id="ca1ac-113">**Live event creation policies**</span></span>

<span data-ttu-id="ca1ac-114">Usługa Yammer postępuje zgodnie z zasadami dotyczącymi zdarzeń na żywo skonfigurowanymi w dzierżawie usługi Office 365 dla usługi Stream.</span><span class="sxs-lookup"><span data-stu-id="ca1ac-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="ca1ac-115">Domyślnie wszyscy w organizacji mogą tworzyć zdarzenia na żywo.</span><span class="sxs-lookup"><span data-stu-id="ca1ac-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="ca1ac-116">Administratorzy mogą [wprowadzić zmiany w tym ustawieniu, co może uniemożliwić użytkownikom tworzenie zdarzenia na żywo](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span><span class="sxs-lookup"><span data-stu-id="ca1ac-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="ca1ac-117">Ważne jest, aby upewnić się, że użytkownicy mają uprawnienia do tworzenia zdarzeń na żywo, jeśli wystąpi błąd zasad.</span><span class="sxs-lookup"><span data-stu-id="ca1ac-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
