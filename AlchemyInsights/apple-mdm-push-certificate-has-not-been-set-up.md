---
title: Nie skonfigurowano certyfikatu Apple MDM Push Certificate
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440015"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="9682a-102">Nie skonfigurowano certyfikatu Apple MDM Push Certificate</span><span class="sxs-lookup"><span data-stu-id="9682a-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="9682a-103">Certyfikat push apple MDM (znany również jako certyfikat apns (Apple Push Notification Service) nie został skonfigurowany dla subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="9682a-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="9682a-104">Bez skonfigurowanego certyfikatu push urządzenia mdm systemu Apple MDM nie można rejestrować urządzeń z systemem iOS i Mac OS i zarządzać nimi.</span><span class="sxs-lookup"><span data-stu-id="9682a-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="9682a-105">Po dodaniu certyfikatu do usługi Intune użytkownicy mogą zainstalować aplikację Portal firmy, aby zarejestrować swoje urządzenia z systemem iOS.</span><span class="sxs-lookup"><span data-stu-id="9682a-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="9682a-106">Wybierz **"Zgadzam się".**</span><span class="sxs-lookup"><span data-stu-id="9682a-106">Select **"I agree."**</span></span> <span data-ttu-id="9682a-107">, aby udzielić firmie Microsoft uprawnień do wysyłania danych do firmy Apple.</span><span class="sxs-lookup"><span data-stu-id="9682a-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="9682a-108">Wybierz **pozycję Pobierz csr** żądanie podpisywania certyfikatu usługi Intune wymagane do utworzenia certyfikatu wypychania urządzenia Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="9682a-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="9682a-109">Plik jest używany do żądania certyfikatu relacji zaufania z portalu Apple Push Certificates Portal.</span><span class="sxs-lookup"><span data-stu-id="9682a-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="9682a-110">Wybierz **pozycję Utwórz certyfikat wypychania mdm,** aby przejść do portalu Apple Push Certificates Portal.</span><span class="sxs-lookup"><span data-stu-id="9682a-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="9682a-111">Zaloguj się za pomocą firmowego konta Apple ID, a następnie wybierz pozycję **Utwórz certyfikat**.</span><span class="sxs-lookup"><span data-stu-id="9682a-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="9682a-112">Wybierz **pozycję Wybierz plik**, przejdź do pliku żądania podpisywania certyfikatu, a następnie wybierz pozycję **Przekaż**.</span><span class="sxs-lookup"><span data-stu-id="9682a-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="9682a-113">Na stronie Potwierdzenie wybierz pozycję **Pobierz,** aby pobrać plik certyfikatu (pem), a następnie zapisz plik lokalnie.</span><span class="sxs-lookup"><span data-stu-id="9682a-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="9682a-114">**Uwaga:** Certyfikat jest skojarzony z identyfikatorem Apple ID użytym do jego utworzenia.</span><span class="sxs-lookup"><span data-stu-id="9682a-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="9682a-115">Najlepszym rozwiązaniem jest używanie firmowego konta Apple ID do zadań zarządzania i upewnienie się, że skrzynka pocztowa jest monitorowana przez więcej niż jedną osobę lub przy użyciu listy dystrybucyjnej.</span><span class="sxs-lookup"><span data-stu-id="9682a-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="9682a-116">Nigdy nie używaj osobistego konta Apple ID.</span><span class="sxs-lookup"><span data-stu-id="9682a-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="9682a-117">Użyj tego samego konta Apple ID, aby odnawiać certyfikat Apple Push co 12 miesięcy.</span><span class="sxs-lookup"><span data-stu-id="9682a-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="9682a-118">Wprowadź identyfikator Apple ID użyty do utworzenia certyfikatu wypychania urządzenia Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="9682a-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="9682a-119">Zapisz ten identyfikator jako przypomnienie, gdy trzeba odnowić certyfikat.</span><span class="sxs-lookup"><span data-stu-id="9682a-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="9682a-120">Przejdź do pliku certyfikatu (pem), wybierz pozycję **Otwórz**, a następnie wybierz pozycję **Przekaż**.</span><span class="sxs-lookup"><span data-stu-id="9682a-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="9682a-121">Dzięki certyfikatowi wypychania usługa Intune może rejestrować urządzenia firmy Apple i zarządzać nimi.</span><span class="sxs-lookup"><span data-stu-id="9682a-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>