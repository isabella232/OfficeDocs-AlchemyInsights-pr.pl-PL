---
title: 2681 symulator ataku w pakiecie Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305341"
---
# <a name="attack-simulator-in-office-365"></a><span data-ttu-id="0f1e5-102">Symulator ataku w pakiecie Office 365</span><span class="sxs-lookup"><span data-stu-id="0f1e5-102">Attack Simulator in Office 365</span></span>

- <span data-ttu-id="0f1e5-103">Czy brakuje symulatora ataku?</span><span class="sxs-lookup"><span data-stu-id="0f1e5-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="0f1e5-104">Symulator ataku wymaga **pakietu office 365 zaawansowane zagrożenie ochrony plan 2 (ATP plan 2)** lub **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="0f1e5-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="0f1e5-105">Symulator ataku **nie** jest uwzględniony w pakiecie Office 365 zaawansowane zagrożenie ochrony plan 1 (plan ATP 1), Office 365 Enterprise E3 lub wszelkie subskrypcje Office 365 Business.</span><span class="sxs-lookup"><span data-stu-id="0f1e5-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Office 365 Business subscriptions.</span></span>

- <span data-ttu-id="0f1e5-106">Konto używane do uruchamiania symulowanych ataków wymaga administratora globalnego lub uprawnienia administratora zabezpieczeń i uwierzytelnianie wieloskładnikowe (MFA).</span><span class="sxs-lookup"><span data-stu-id="0f1e5-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="0f1e5-107">Aby uzyskać więcej informacji na temat wymagań symulator ataku Zobacz w [tym temacie](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="0f1e5-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="0f1e5-108">Ważne rzeczy, o których warto wiedzieć o **Brute Force hasło** ataku symulacje:</span><span class="sxs-lookup"><span data-stu-id="0f1e5-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="0f1e5-109">Jeśli konto docelowe ma włączoną usługę MFA i hasło zostało odgadnięte poprawnie, konto nie będą wyświetlane jako zagrożone (drugi współczynnik uwierzytelniania będzie niekompletna).</span><span class="sxs-lookup"><span data-stu-id="0f1e5-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="0f1e5-110">Plik haseł nie może być większy niż 10 MB.</span><span class="sxs-lookup"><span data-stu-id="0f1e5-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="0f1e5-111">Użyj jednego hasła w wierszu i Dołącz pusty wiersz (powrót karetki) po ostatnim hasło na liście.</span><span class="sxs-lookup"><span data-stu-id="0f1e5-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="0f1e5-112">Ważne informacje o symulacjach dołączania **włóczni do phishingu** :</span><span class="sxs-lookup"><span data-stu-id="0f1e5-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="0f1e5-113">Według projektu nie można podać niestandardowej wartości **adresu URL serwera logowania phishingowego**.</span><span class="sxs-lookup"><span data-stu-id="0f1e5-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="0f1e5-114">Jeśli odbiorca używa [Włącz dodatek raportu Raport](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , aby zgłosić wiadomość jako phishing, może nie odbierać alerty dla wiadomości (ponieważ jest to symulowany atak).</span><span class="sxs-lookup"><span data-stu-id="0f1e5-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="0f1e5-115">Raporty: po zakończeniu symulowanego ataku możesz kliknąć pozycję **szczegóły ataku** , aby wyświetlić raport.</span><span class="sxs-lookup"><span data-stu-id="0f1e5-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="0f1e5-116">Aby uzyskać szczegółowe instrukcje i nowe funkcje w symulatorze ataku, zobacz [symulator ataku w pakiecie Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="0f1e5-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
