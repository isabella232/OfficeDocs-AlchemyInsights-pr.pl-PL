---
title: 2681 symulatora ataków w systemie Microsoft 365
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
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759229"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="45b47-102">Symulator ataków w systemie Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="45b47-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="45b47-103">Czy brakuje symulatora ataku?</span><span class="sxs-lookup"><span data-stu-id="45b47-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="45b47-104">Symulator ataków wymaga **pakietu office 365 Advanced Threat Protection Plan 2 (ATP plan 2)** lub **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="45b47-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="45b47-105">Aplikacja symulatora ataków **nie** jest dostępna w pakiecie Office 365 Advanced Threat Protection Plan 1 (plan ATP 1), Office 365 Enterprise E3 ani żadnych aplikacji Microsoft 365 dla subskrypcji biznesowych.</span><span class="sxs-lookup"><span data-stu-id="45b47-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="45b47-106">Konto używane do uruchamiania symulowanych ataków wymaga uprawnień administratora globalnego lub administratora zabezpieczeń oraz uwierzytelniania wieloskładnikowego (MFA).</span><span class="sxs-lookup"><span data-stu-id="45b47-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="45b47-107">Aby uzyskać więcej informacji na temat wymagań dotyczących ataków na ataki, zobacz [ten temat](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="45b47-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="45b47-108">Ważne zagadnienia związane z symulacją ataków za ataki za pośrednictwem **hasła** :</span><span class="sxs-lookup"><span data-stu-id="45b47-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="45b47-109">Jeśli dla konta docelowego jest włączone uwierzytelnianie wieloskładnikowe, a hasło zostało nagrane poprawnie, konto nie będzie widoczne jako zagrożone (drugi współczynnik uwierzytelniania będzie niekompletny).</span><span class="sxs-lookup"><span data-stu-id="45b47-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="45b47-110">Rozmiar pliku hasła nie może przekraczać 10 MB.</span><span class="sxs-lookup"><span data-stu-id="45b47-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="45b47-111">Użyj jednego hasła na wiersz i Dołącz pusty wiersz (znak powrotu karetki) po ostatnim haśle na liście.</span><span class="sxs-lookup"><span data-stu-id="45b47-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="45b47-112">Ważne zagadnienia dotyczące **Spearych informacji** o dołączaniu do witryn wyłudzających informacje:</span><span class="sxs-lookup"><span data-stu-id="45b47-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="45b47-113">Według projektu nie można podać wartości niestandardowej dla **adresu URL serwera logowania wyłudzających informacje**.</span><span class="sxs-lookup"><span data-stu-id="45b47-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="45b47-114">Jeśli odbiorca używa [dodatku Włącz wiadomość raportu](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , aby zgłosić wiadomość jako wyłudzanie informacji, użytkownik może nie otrzymywać alertów dotyczących wiadomości (ponieważ jest to symulowane ataki).</span><span class="sxs-lookup"><span data-stu-id="45b47-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="45b47-115">Raporty: po zakończeniu symulowanego ataku można kliknąć pozycję **szczegóły ataku** , aby wyświetlić raport.</span><span class="sxs-lookup"><span data-stu-id="45b47-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="45b47-116">Szczegółowe instrukcje i nowe funkcje w symulatorze ataku znajdziesz [w witrynie Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="45b47-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
