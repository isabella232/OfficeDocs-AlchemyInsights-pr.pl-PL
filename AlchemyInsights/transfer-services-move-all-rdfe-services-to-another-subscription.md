---
title: Transfer usług — przenoszenie wszystkich usług frontonu reddog do innej subskrypcji
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692172"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="a2687-102">Transfer usług — przenoszenie wszystkich usług frontonu reddog do innej subskrypcji</span><span class="sxs-lookup"><span data-stu-id="a2687-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="a2687-103">**Przenoszenie zasobów**</span><span class="sxs-lookup"><span data-stu-id="a2687-103">**Move resources**</span></span>

<span data-ttu-id="a2687-104">Zasoby platformy Azure można przenieść do innej subskrypcji platformy Azure lub grupy zasobów w ramach tej samej subskrypcji za pomocą usługi Azure Portal, platformy Azure CLI, usługi Azure CLI lub interfejsu API usługi w celu przeniesienia zasobów.</span><span class="sxs-lookup"><span data-stu-id="a2687-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="a2687-105">Aby można było przenosić zasoby, zobacz:</span><span class="sxs-lookup"><span data-stu-id="a2687-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="a2687-106">Lista kontrolna przed przeniesieniem zasobów</span><span class="sxs-lookup"><span data-stu-id="a2687-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="a2687-107">Usługi, które można przenosić</span><span class="sxs-lookup"><span data-stu-id="a2687-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="a2687-108">Jak sprawdzić poprawność przeniesienia</span><span class="sxs-lookup"><span data-stu-id="a2687-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="a2687-109">Przenoszenie wskazówek dotyczących usług</span><span class="sxs-lookup"><span data-stu-id="a2687-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="a2687-110">Aby przenieść istniejące zasoby do innej grupy zasobów lub abonamentu, możesz skorzystać z następujących czynności:</span><span class="sxs-lookup"><span data-stu-id="a2687-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="a2687-111">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="a2687-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="a2687-112">Środowisko Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="a2687-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="a2687-113">Usługa Azure CLI</span><span class="sxs-lookup"><span data-stu-id="a2687-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="a2687-114">INTERFEJS API USŁUGI</span><span class="sxs-lookup"><span data-stu-id="a2687-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="a2687-115">Samouczek: [przenoszenie zasobów platformy Azure do innej grupy zasobów lub subskrypcji](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="a2687-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="a2687-116">**Rozwiązywanie problemów z usługą Azure Resource Manager**</span><span class="sxs-lookup"><span data-stu-id="a2687-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="a2687-117">Zapoznaj się z poniższymi artykułami, aby dowiedzieć się więcej o typowych błędach wdrażania usługi Azure oraz otrzymywać informacje umożliwiające ich usunięcie.</span><span class="sxs-lookup"><span data-stu-id="a2687-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="a2687-118">Jeśli nie możesz znaleźć kodu błędu dotyczącego błędu wdrażania, zobacz [Znajdowanie kodu błędu](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="a2687-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="a2687-119">Rozwiązywanie problemów z błędami wdrażania</span><span class="sxs-lookup"><span data-stu-id="a2687-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="a2687-120">Rozwiązywanie problemów dotyczących przenoszenia zasobów platformy Azure do nowej grupy zasobów lub subskrypcji</span><span class="sxs-lookup"><span data-stu-id="a2687-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="a2687-121">Pamiętaj, że jeśli chcesz uaktualnić subskrypcję platformy Azure, na przykład przełączenie się za darmo w celu płacenia na bieżąco, musisz przekonwertować abonament.</span><span class="sxs-lookup"><span data-stu-id="a2687-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="a2687-122">Aby uaktualnić bezpłatny okres próbny, zobacz [uaktualnianie bezpłatnego okresu próbnego lub abonamentu Microsoft Wyobraźmy sobie na abonament na bieżąco](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="a2687-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="a2687-123">Aby zmienić konto Płać na bieżąco, zobacz [Zmienianie abonamentu na usługę Azure Pay na bieżąco do innej oferty](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="a2687-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="a2687-124">**Aby dodać lub skojarzyć subskrypcję platformy Azure Active Directory:**</span><span class="sxs-lookup"><span data-stu-id="a2687-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="a2687-125">Zaloguj się i wybierz abonament, którego chcesz użyć, na [stronie Subskrypcje w portalu Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="a2687-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="a2687-126">Wybierz pozycję **Zmień katalog**.</span><span class="sxs-lookup"><span data-stu-id="a2687-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="a2687-127">Przejrzyj wyświetlone ostrzeżenia, a następnie wybierz pozycję **Zmień**.</span><span class="sxs-lookup"><span data-stu-id="a2687-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="a2687-128">Po zmianie katalogu dla subskrypcji zostanie wyświetlony komunikat o powodzeniu.</span><span class="sxs-lookup"><span data-stu-id="a2687-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="a2687-129">Użyj przełącznika *katalogów* , aby przejść do nowego katalogu.</span><span class="sxs-lookup"><span data-stu-id="a2687-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="a2687-130">Poprawne wyświetlanie wszystkich elementów może potrwać do 10 minut.</span><span class="sxs-lookup"><span data-stu-id="a2687-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="a2687-131">**Polecane dokumenty**</span><span class="sxs-lookup"><span data-stu-id="a2687-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="a2687-132">Przenoszenie własności subskrypcji platformy Azure</span><span class="sxs-lookup"><span data-stu-id="a2687-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="a2687-133">Przenoszenie zasobów do nowej grupy zasobów lub subskrypcji</span><span class="sxs-lookup"><span data-stu-id="a2687-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="a2687-134">Zarządzanie zasobami za pomocą portalu Azure</span><span class="sxs-lookup"><span data-stu-id="a2687-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
