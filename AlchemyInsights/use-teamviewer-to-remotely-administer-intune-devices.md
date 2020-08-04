---
title: Zdalne administrowanie urządzeniami usługi Intune za pomocą funkcji TeamViewer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555244"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="3aa5c-102">Zdalne administrowanie urządzeniami usługi Intune za pomocą funkcji TeamViewer</span><span class="sxs-lookup"><span data-stu-id="3aa5c-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="3aa5c-103">Urządzenia zarządzane przez usługę Intune mogą być administrowane zdalnie za pomocą [programu TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="3aa5c-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="3aa5c-104">Aby administrować usłudze Intune przy użyciu programu TeamViewer, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="3aa5c-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="3aa5c-105">Rozpocznij od uzyskania poświadczeń od programu TeamViewer, aby skonfigurować łącznik TeamViewer w usłudze Intune.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="3aa5c-106">Dzięki temu administrator może wprowadzić poświadczenia w interfejsie użytkownika łącznika teamviewer w obszarze Urządzenia, jednorazowa operacja w celu ustanowienia łącza między usługą Intune i usługą TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="3aa5c-107">**Część 1: Rozpoczęcie sesji za pomocą urządzenia zdalnego**</span><span class="sxs-lookup"><span data-stu-id="3aa5c-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="3aa5c-108">W obszarze **Wszystkie urządzenia**wybierz urządzenie, z którego chcesz rozpocząć sesję zdalną.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="3aa5c-109">Od **... Więcej**, wybierz **pozycję Nowa sesja pomocy zdalnej**.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="3aa5c-110">Wybierz **pozycję Tak,** aby potwierdzić, że chcesz ustanowić sesję zdalną.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="3aa5c-111">Po potwierdzeniu żądania "Inicjowanie nowej sesji zdalnej" przez usługę TeamViewer zostanie wyświetlona opcja **Uruchom pomoc zdalną** pod szczegółowymi informacjami o okienku Przegląd (lub Essentials) dla urządzenia.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="3aa5c-112">Wybierz **pozycję Zobacz więcej,** aby rozwinąć okienko i wyświetlić stan Pomocy zdalnej.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="3aa5c-113">Wybierz **pozycję Rozpocznij sesję zdalną,** aby zainicjować sesję po stronie administratora.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="3aa5c-114">Wybierz, aby pobrać plik binarny TeamViewer (Windows) i wybierz pozycję **Uruchom**.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="3aa5c-115">**Uwaga** Możesz zignorować dowolną stronę przeglądarki internetowej otwartą na stronie internetowej TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="3aa5c-116">Potwierdź żądanie aplikacji TeamViewer, aby wprowadzić zmiany na urządzeniu (tylko windows).</span><span class="sxs-lookup"><span data-stu-id="3aa5c-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="3aa5c-117">Uruchomiono aplikację TeamViewer i zawiera kod sesji do uwierzytelniania połączenia z urządzeniem zdalnym.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="3aa5c-118">**Część 2: Na urządzeniu przeznaczonym do zdalnej sesji**</span><span class="sxs-lookup"><span data-stu-id="3aa5c-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="3aa5c-119">Otwórz portal firmy usługi Intune.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="3aa5c-120">Poszukaj flagi powiadomień: "Administrator IT żąda kontroli nad tym urządzeniem dla sesji pomocy zdalnej" i wybierz powiadomienie.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="3aa5c-121">Wybierz, aby pobrać aplikację TeamViewer lub potwierdzić pobranie aplikacji TeamViewer ze sklepu z aplikacjami, a następnie wybierz pozycję **Uruchom**.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="3aa5c-122">**Uwaga** Możesz zignorować dowolną stronę przeglądarki internetowej otwartą na stronie internetowej TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="3aa5c-123">Potwierdź żądanie aplikacji TeamViewer, aby wprowadzić zmiany na urządzeniu (tylko windows).</span><span class="sxs-lookup"><span data-stu-id="3aa5c-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="3aa5c-124">Uruchomiono aplikację TeamViewer i zawiera kod sesji do uwierzytelniania połączenia z urządzeniem zdalnym.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="3aa5c-125">Wyskakujące okienko z pytaniem, czy chcesz zezwolić na rozpoczęcie sesji.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="3aa5c-126">**Uwaga** Kody sesji generowane przez usługę TeamViewer są tylko jednorazowe.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="3aa5c-127">W przypadku utraty połączenia należy:</span><span class="sxs-lookup"><span data-stu-id="3aa5c-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="3aa5c-128">Zamknij wystąpienie aplikacji TeamViewer na urządzeniu zdalnym i na stacji roboczej administratora.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="3aa5c-129">Zamknij portal firmy na urządzeniu zdalnym.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="3aa5c-130">Inicjowanie nowej "Nowej sesji pomocy zdalnej" z portalu administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="3aa5c-131">Otwórz ponownie portal firmy na urządzeniu zdalnym, aby otrzymać nowe powiadomienie.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="3aa5c-132">Pobierz i otwórz aplikację TeamViewer zarówno na urządzeniu zdalnym, jak i na stacji roboczej administratora, tak jak poprzednio.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>