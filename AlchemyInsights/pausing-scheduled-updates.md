---
title: Wstrzymywanie zaplanowanych aktualizacji
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555514"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="04b8a-102">Wstrzymywanie zaplanowanych aktualizacji</span><span class="sxs-lookup"><span data-stu-id="04b8a-102">Pausing scheduled updates</span></span>

<span data-ttu-id="04b8a-103">Po wydaniu polecenia pauzy urządzenia nie przetwarzają polecenia, dopóki następnym razem zaewidencjonują je w usłudze Intune.</span><span class="sxs-lookup"><span data-stu-id="04b8a-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="04b8a-104">Z tego powodu urządzenia mogą mieć:</span><span class="sxs-lookup"><span data-stu-id="04b8a-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="04b8a-105">Zainstalowano zaplanowane aktualizacje przed zameldowanie.</span><span class="sxs-lookup"><span data-stu-id="04b8a-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="04b8a-106">Został wyłączony po wydaniu polecenia pauzy.</span><span class="sxs-lookup"><span data-stu-id="04b8a-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="04b8a-107">W takim przypadku, gdy urządzenia były włączone, mogły pobrać i zainstalować zaplanowane aktualizacje przed zaewidencjonowania.</span><span class="sxs-lookup"><span data-stu-id="04b8a-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>