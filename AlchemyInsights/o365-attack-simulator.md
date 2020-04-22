---
title: 2681 Symulator ataku w usłudze Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713476"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="9201b-102">Symulator ataku w usłudze Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9201b-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="9201b-103">Brakuje Ci Symulatora Ataku?</span><span class="sxs-lookup"><span data-stu-id="9201b-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="9201b-104">Symulator ataku wymaga **planu zaawansowanej ochrony przed zagrożeniami usługi Office 365 2 (plan ATP 2)** lub **usługi Office 365 Enterprise E5.**</span><span class="sxs-lookup"><span data-stu-id="9201b-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="9201b-105">Symulator ataku **nie** jest uwzględniony w planie zaawansowanej ochrony przed zagrożeniami usługi Office 365 1 (plan ATP 1), usłudze Office 365 Enterprise E3 ani w żadnych subskrypcjach aplikacji microsoft 365 dla firm.</span><span class="sxs-lookup"><span data-stu-id="9201b-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="9201b-106">Konto używane do przeprowadzania symulowanych ataków wymaga uprawnień administratora globalnego lub administratora zabezpieczeń oraz uwierzytelniania wieloskładnikowego(MFA).</span><span class="sxs-lookup"><span data-stu-id="9201b-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="9201b-107">Aby uzyskać więcej informacji na temat wymagań symulatora ataku, zobacz [ten temat](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="9201b-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="9201b-108">Ważne informacje o symulacjach ataku **Brute Force Password:**</span><span class="sxs-lookup"><span data-stu-id="9201b-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="9201b-109">Jeśli konto docelowe ma włączone uwierzytelnianie wieloskładnikowe i hasło zostało poprawnie odgadnięty, konto nie będzie wyświetlane jako naruszone (drugi czynnik uwierzytelniania będzie niekompletny).</span><span class="sxs-lookup"><span data-stu-id="9201b-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="9201b-110">Plik hasła nie może być większy niż 10 MB.</span><span class="sxs-lookup"><span data-stu-id="9201b-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="9201b-111">Użyj jednego hasła w wierszu i dołącz pusty wiersz (powrót karetki) po ostatnim haśle na liście.</span><span class="sxs-lookup"><span data-stu-id="9201b-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="9201b-112">Ważne informacje o **spear phishingu** dołączyć symulacje:</span><span class="sxs-lookup"><span data-stu-id="9201b-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="9201b-113">Zgodnie z projektem nie można podać niestandardowej wartości **adresu URL serwera logowania do witryn wyłudzających informacje.**</span><span class="sxs-lookup"><span data-stu-id="9201b-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="9201b-114">Jeśli adresat używa [dodatku Włącz komunikat o zgłoś,](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) aby zgłosić wiadomość jako wyłudzającą informacje, może nie być wyświetlanych alertów dotyczących wiadomości (ponieważ jest to symulowany atak).</span><span class="sxs-lookup"><span data-stu-id="9201b-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="9201b-115">Raporty: Po zakończeniu symulowanego ataku możesz kliknąć **szczegóły ataku,** aby zobaczyć raport.</span><span class="sxs-lookup"><span data-stu-id="9201b-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="9201b-116">Aby uzyskać szczegółowe instrukcje i nowe funkcje w symulatorze ataku, zobacz [Symulator ataku w usłudze Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="9201b-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
