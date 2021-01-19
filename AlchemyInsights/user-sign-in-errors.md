---
title: Błędy logowania użytkownika
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901258"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="7c0fc-102">Błędy logowania użytkownika</span><span class="sxs-lookup"><span data-stu-id="7c0fc-102">User sign-in errors</span></span>

<span data-ttu-id="7c0fc-103">**Rozwiązywanie problemów z diagnostyką logowania**</span><span class="sxs-lookup"><span data-stu-id="7c0fc-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="7c0fc-104">Aby wykryć przyczyny problemów związanych z logowaniem się użytkowników, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="7c0fc-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="7c0fc-105">Uruchom [diagnostykę logowania](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="7c0fc-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="7c0fc-106">Znajdź zdarzenie, które ma zostać zanalizowane, wprowadzając szczegółowe informacje o użytkowniku, aplikacji, godzinie logowania, identyfikatorze żądania lub identyfikatorze korelacji.</span><span class="sxs-lookup"><span data-stu-id="7c0fc-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="7c0fc-107">Przejrzyj wyniki diagnostyczne przedstawiające szczegóły dotyczące tego, co się stało, oraz jakie działania możesz podjąć w celu wprowadzenia zmian, jeśli konieczne są zmiany.</span><span class="sxs-lookup"><span data-stu-id="7c0fc-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="7c0fc-108">**Szukasz informacji na temat kodów błędów AADSTS, które są zwracane z usługi Microsoft Azure Active Directory (STS)?**</span><span class="sxs-lookup"><span data-stu-id="7c0fc-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="7c0fc-109">Przeczytaj [ten artykuł](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) , aby znaleźć AADSTS błędów, poprawki i proponowane obejścia</span><span class="sxs-lookup"><span data-stu-id="7c0fc-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>