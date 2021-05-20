---
title: 2681 Attack Podczas Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545736"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="99233-102">Attack Pochoć w Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="99233-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="99233-103">Czy brakuje Ci ataku?</span><span class="sxs-lookup"><span data-stu-id="99233-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="99233-104">Podczas ataków Do ataki jest wymagany program **Microsoft Defender Office 365 plan 2** lub Office 365 Enterprise **E5.**</span><span class="sxs-lookup"><span data-stu-id="99233-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="99233-105">Ataki Dla **usług** Microsoft Defender for Office 365 Plan 1, E3 i E3 Office 365 Enterprise nie są uwzględnione w Aplikacje Microsoft 365 dla firm subskrypcji usługi.</span><span class="sxs-lookup"><span data-stu-id="99233-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="99233-106">Konto służące do uruchamiania symulowanych ataków wymaga uprawnień administratora globalnego lub administratora zabezpieczeń oraz uwierzytelniania wieloskładnikowego (MFA).</span><span class="sxs-lookup"><span data-stu-id="99233-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="99233-107">Aby uzyskać więcej informacji na temat wymagań dotyczących ataków, zobacz [ten temat.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="99233-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="99233-108">Ważne informacje na temat symulacyjnych **ataków na wymuszanie** haseł:</span><span class="sxs-lookup"><span data-stu-id="99233-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="99233-109">Jeśli dla konta docelowego włączono uwierzytelnianie MFA i hasło zostało odgadane poprawnie, konto nie będzie wyświetlane jako naruszone (drugi współczynnik uwierzytelniania będzie niekompletny).</span><span class="sxs-lookup"><span data-stu-id="99233-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="99233-110">Plik hasła nie może być większy niż 10 MB.</span><span class="sxs-lookup"><span data-stu-id="99233-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="99233-111">Użyj jednego hasła w wierszu i uwzględnij pusty wiersz (powrót karetki) po ostatnim hasłem na liście.</span><span class="sxs-lookup"><span data-stu-id="99233-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="99233-112">Ważne informacje na temat symulacyjnych dołączania **wiadomości wyłudzających** informacje:</span><span class="sxs-lookup"><span data-stu-id="99233-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="99233-113">Domyślnie nie można podać niestandardowej wartości adresu URL serwera **logowania wyłudzania informacji.**</span><span class="sxs-lookup"><span data-stu-id="99233-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="99233-114">Jeśli adresat użyje dodatku [Włącz](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) wiadomość raportu w celu zgłoszenia wiadomości jako próby wyłudzenia informacji, alerty dotyczące wiadomości mogą nie być odbierane (ponieważ jest to symulowany atak).</span><span class="sxs-lookup"><span data-stu-id="99233-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="99233-115">Raporty: Po zakończeniu symulowanego ataku możesz kliknąć pozycję **Szczegóły** ataków, aby wyświetlić raport.</span><span class="sxs-lookup"><span data-stu-id="99233-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="99233-116">Aby uzyskać szczegółowe instrukcje i nowe funkcje w programie Attack Podczas tego ataku, zobacz [Temat ataków w programie Microsoft 365.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="99233-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
