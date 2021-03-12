---
title: Przykładowa usługa Microsoft Defender dla zasad ochrony przed wyłudzaniem informacji w usłudze Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750792"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="8af4e-102">Przykładowa usługa Microsoft Defender dla zasad ochrony przed wyłudzaniem informacji w usłudze Office 365</span><span class="sxs-lookup"><span data-stu-id="8af4e-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="8af4e-103">Te ustawienia umożliwiają zasady o nazwie *Domain (Domena) i GENERAL (Dyrektor generalny).*</span><span class="sxs-lookup"><span data-stu-id="8af4e-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="8af4e-104">Te zasady zapewniają zarówno ochronę użytkowników, jak i domen przed personifikacji, a następnie dotyczą wszystkich wiadomości e-mail odbieranych przez użytkowników w domenie.</span><span class="sxs-lookup"><span data-stu-id="8af4e-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="8af4e-105">Najpierw dodaj następujące informacje, aby utworzyć zasady:</span><span class="sxs-lookup"><span data-stu-id="8af4e-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="8af4e-106">**Nazwa:** Opis domeny i dyrektora **generalnego:** gwarantuje, że dyrektor generalny i Twoja domena nie są personifikowane.</span><span class="sxs-lookup"><span data-stu-id="8af4e-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="8af4e-107">**Dotyczy:** Wybierz **domenę adresata to**.</span><span class="sxs-lookup"><span data-stu-id="8af4e-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="8af4e-108">W **obszarze Dowolny z nich** wybierz pozycję **Wybierz**, a następnie wybierz domenę.</span><span class="sxs-lookup"><span data-stu-id="8af4e-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="8af4e-109">Wybierz **pozycję + Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="8af4e-109">Select **+ Add**.</span></span> <span data-ttu-id="8af4e-110">Zaznacz pole wyboru obok nazwy domeny na liście (na przykład *contoso.com*), a następnie wybierz pozycję **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="8af4e-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="8af4e-111">Wybierz **pozycję Gotowe**.</span><span class="sxs-lookup"><span data-stu-id="8af4e-111">Select **Done**.</span></span>
- <span data-ttu-id="8af4e-112">Po utworzeniu zasad można je dostosować, korzystając z następujących opcji:</span><span class="sxs-lookup"><span data-stu-id="8af4e-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="8af4e-113">**Dodawanie użytkowników w celu ochrony:** W tym przykładzie dodaj co najmniej adres e-mail dyrektora generalnego.</span><span class="sxs-lookup"><span data-stu-id="8af4e-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="8af4e-114">**Dodawanie domen w celu ochrony**: Dodaj domenę organizacji, która zawiera biuro Dyrektora Generalnego.</span><span class="sxs-lookup"><span data-stu-id="8af4e-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="8af4e-115">**Wybierz akcje:** Jeśli wiadomość e-mail jest wysyłana przez spersonifikowanego **użytkownika,** wybierz pozycję Przekieruj wiadomość na inny adres e-mail **,** a następnie wprowadź adres e-mail administratora zabezpieczeń (na przykład *securityadmin@contoso.com).*</span><span class="sxs-lookup"><span data-stu-id="8af4e-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="8af4e-116">W **przypadku, gdy wiadomość e-mail jest wysyłana za pomocą personifikacji domeny,** wybierz **pozycję Poddaj wiadomość kwarantannie**.</span><span class="sxs-lookup"><span data-stu-id="8af4e-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="8af4e-117">**Inteligencja** skrzynek pocztowych: ta opcja jest domyślnie zaznaczona podczas tworzenia nowych zasad ochrony przed wyłudzaniem informacji.</span><span class="sxs-lookup"><span data-stu-id="8af4e-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="8af4e-118">Aby uzyskać najlepsze **wyniki, pozostaw** to ustawienie wł.</span><span class="sxs-lookup"><span data-stu-id="8af4e-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="8af4e-119">**Dodaj zaufanych nadawców i domeny:** W tym przykładzie nie definiuj żadnych zastępować.</span><span class="sxs-lookup"><span data-stu-id="8af4e-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="8af4e-120">Po przejrzenia ustawień wybierz pozycję Utwórz **te zasady** lub **Zapisz** odpowiednio do potrzeb.</span><span class="sxs-lookup"><span data-stu-id="8af4e-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="8af4e-121">Aby dowiedzieć się więcej, zobacz [Zasady ochrony przed wyłudzaniem informacji na platformy Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)</span><span class="sxs-lookup"><span data-stu-id="8af4e-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
