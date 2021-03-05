---
title: Inicjowanie obsługi użytkowników w dni robocze u użytkowników usługi AD przechodzi do stanu kwarantanny
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481881"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="76e2b-102">Inicjowanie obsługi użytkowników w dni robocze u użytkowników usługi AD przechodzi do stanu kwarantanny</span><span class="sxs-lookup"><span data-stu-id="76e2b-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="76e2b-103">**Inicjowanie obsługi użytkowników w dni robocze u użytkowników usługi AD przechodzi do stanu kwarantanny i w u usługi AD nie są tworzona żadna użytkownicy**</span><span class="sxs-lookup"><span data-stu-id="76e2b-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="76e2b-104">Zadanie inicjowania obsługi użytkowników usługi AD w dzień roboczy przeszedł do stanu kwarantanny, a w dziennikach inspekcji są wyświetlane zdarzenia niepowodzenia eksportu z komunikatem o **błędzie: OperationsError-SvcErr: Wystąpił błąd operacji. Dla usługi katalogowej nie skonfigurowano żadnego odwołania przełożonego. Usługa katalogowa nie może więc wydawać poleceń** do obiektów spoza tego lasu.</span><span class="sxs-lookup"><span data-stu-id="76e2b-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="76e2b-105">Ten błąd jest zazwyczaj wyświetlany, jeśli obiekt OU kontenera usługi Active Directory nie został poprawnie skonfigurowany lub występują problemy z mapowaniem wyrażeń używanym dla elementu **parentDistinguishedName.**</span><span class="sxs-lookup"><span data-stu-id="76e2b-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="76e2b-106">Sprawdź, czy parametr Default OU for New Users (Domyślna wersja systemu operacyjnego dla **nowych użytkowników)** nie zawiera literówek.</span><span class="sxs-lookup"><span data-stu-id="76e2b-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="76e2b-107">Upewnij się, że określona grupa OU już istnieje w ad.</span><span class="sxs-lookup"><span data-stu-id="76e2b-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="76e2b-108">Jeśli używasz wartości **parentDistinguishedName** podczas mapowania atrybutów, upewnij się, że zawsze jest szacowana jako znany kontener w domenie usługi AD.</span><span class="sxs-lookup"><span data-stu-id="76e2b-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="76e2b-109">Sprawdź zdarzenie Eksportowanie w dziennikach inspekcji, aby wyświetlić wygenerowaną wartość.</span><span class="sxs-lookup"><span data-stu-id="76e2b-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="76e2b-110">Aby uzyskać więcej szczegółowych informacji na temat konfigurowania dnia roboczego dla automatycznego inicjowania obsługi, zobacz Samouczek: Konfigurowanie dnia roboczego [dla automatycznego inicjowania obsługi administracyjnej użytkowników.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="76e2b-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

