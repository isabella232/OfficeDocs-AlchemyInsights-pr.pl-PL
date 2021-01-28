---
title: Dzienniki i raportowanie
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
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036008"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="7f554-102">Dzienniki i raportowanie</span><span class="sxs-lookup"><span data-stu-id="7f554-102">Logs and Reporting</span></span>

<span data-ttu-id="7f554-103">[Odpowiedzi na często zadawane pytania](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) dotyczące raportowania w usłudze Azure Active Directory (Azure AD) w ramach raportowania w usłudze Azure Active Directory są odpowiedziami na często zadawane pytania.</span><span class="sxs-lookup"><span data-stu-id="7f554-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="7f554-104">Aby uzyskać więcej informacji, zobacz [raporty usługi Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)</span><span class="sxs-lookup"><span data-stu-id="7f554-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="7f554-105">**Rozwiązywanie problemów z inspekcją**</span><span class="sxs-lookup"><span data-stu-id="7f554-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="7f554-106">Jeśli masz problemy z wyświetlaniem niektórych działań inspekcji, a na tej liście brakuje [działania,](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)zdaj zgłoszenie do pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="7f554-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="7f554-107">Jeśli masz problemy z wyświetlaniem dzienników inspekcji w dzierżawie, zachowaj bilet pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="7f554-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="7f554-108">Jeśli działania inspekcji nie są natychmiast wyświetlane w portalu [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) Azure Portal, wyewidencjonaj nasze informacje o opóźnieniach i jeśli opóźnienie przekracza udokumentowane opóźnienie, schowaj bilet pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="7f554-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="7f554-109">Przechowywanie dzienników aktywności usługi Azure AD</span><span class="sxs-lookup"><span data-stu-id="7f554-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="7f554-110">Jeśli nie widzisz całej inspekcji dla wybranego zakresu dat, możesz pobrać z portalu Azure maksymalnie 250 000 wierszy (posortowanych według najnowszych) logów.</span><span class="sxs-lookup"><span data-stu-id="7f554-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="7f554-111">Aby uzyskać więcej informacji, zobacz [Pobieranie działań inspekcji.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)</span><span class="sxs-lookup"><span data-stu-id="7f554-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="7f554-112">**Rozwiązywanie problemów z logowaniem**</span><span class="sxs-lookup"><span data-stu-id="7f554-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="7f554-113">Dane z ostatnich 30 dni są dostępne tylko w przypadku licencji usługi Azure AD Premium (P1 lub P2) dla dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="7f554-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="7f554-114">Logowanie jest dostępne tylko dla dzierżaw usługi Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="7f554-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="7f554-115">Nie jest dostępna w przypadku dzierżaw z licencją bezpłatną ani podstawową.</span><span class="sxs-lookup"><span data-stu-id="7f554-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="7f554-116">Jeśli Twoja dzierżawa ma licencję Premium P1 i nie widzisz logowania, zapoznaj się z informacjami o opóźnieniach i zapisz bilet pomocy technicznej, jeśli opóźnienie przekracza udokumentowane opóźnienie. [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies)</span><span class="sxs-lookup"><span data-stu-id="7f554-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="7f554-117">Jeśli nie widzisz wszystkich logowania dla wybranego zakresu dat, pamiętaj, że możesz pobrać maksymalnie 250 000 wierszy (posortowanych według najnowszych) logów z portalu Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="7f554-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="7f554-118">Aby uzyskać więcej informacji, zobacz [Pobieranie działań logowania.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)</span><span class="sxs-lookup"><span data-stu-id="7f554-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="7f554-119">**Rozwiązywanie problemów z raportami zabezpieczeń (użytkownicy oflagowywali na ryzyko, ryzykowne logowanie)**</span><span class="sxs-lookup"><span data-stu-id="7f554-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="7f554-120">Użytkownicy oflagowywali w raporcie o zabezpieczeniach ryzyka</span><span class="sxs-lookup"><span data-stu-id="7f554-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="7f554-121">Raport ryzykownych logowania w portalu usługi Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="7f554-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="7f554-122">Zdarzenia ryzyka związane z usługą Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="7f554-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
