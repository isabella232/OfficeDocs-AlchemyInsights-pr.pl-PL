---
title: Rozwiązywanie problemów z certyfikatem podpisywania SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694445"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="bcd5a-102">Rozwiązywanie problemów z certyfikatem podpisywania SAML</span><span class="sxs-lookup"><span data-stu-id="bcd5a-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="bcd5a-103">Aby rozwiązać problem z certyfikatem podpisywania SAML, wykonaj następujące zalecane czynności:</span><span class="sxs-lookup"><span data-stu-id="bcd5a-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="bcd5a-104">Po dodaniu aplikacji przedsiębiorstwa, która obsługuje logowanie jednokrotne, platforma Azure wygeneruje certyfikat nazywany certyfikatem [podpisywania SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)</span><span class="sxs-lookup"><span data-stu-id="bcd5a-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="bcd5a-105">Ten certyfikat ma datę wygaśnięcia 3 lat.</span><span class="sxs-lookup"><span data-stu-id="bcd5a-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="bcd5a-106">Aby zmienić datę wygaśnięcia certyfikatu, zobacz Dostosowywanie daty wygaśnięcia certyfikatu federacji i wycofywanie go [do nowego certyfikatu.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)</span><span class="sxs-lookup"><span data-stu-id="bcd5a-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="bcd5a-107">Platforma Azure użyje tego certyfikatu do podpisania tokenów SAML żądanych przez aplikację i wysłania ich do aplikacji w celu pomyślnego logowania jednokrotnego.</span><span class="sxs-lookup"><span data-stu-id="bcd5a-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="bcd5a-108">Aby to ukończyć, pobierz certyfikat z portalu Azure Portal i wyślij go dostawcy aplikacji, aby ukończyć proces logowania jednokrotnego.</span><span class="sxs-lookup"><span data-stu-id="bcd5a-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="bcd5a-109">Po zakończeniu tego procesu aplikacja będzie ufać temu certyfikatowi i wszystkie tokeny SAML podpisane przez ten certyfikat zostaną zaakceptowane przez aplikację.</span><span class="sxs-lookup"><span data-stu-id="bcd5a-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="bcd5a-110">Jeśli ten certyfikat wygaśnie, utwórz nowy certyfikat, zaktualizuj go u dostawcy aplikacji, a następnie uacyjnij po stronie platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="bcd5a-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="bcd5a-111">Aby uzyskać więcej informacji, [zobacz Odnawianie certyfikatu, który wkrótce wygaśnie.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)</span><span class="sxs-lookup"><span data-stu-id="bcd5a-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="bcd5a-112">Jeśli certyfikat wygaśnie, użytkownik nie zostanie zablokowany.</span><span class="sxs-lookup"><span data-stu-id="bcd5a-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="bcd5a-113">[Dodaj adres e-mail, aby powiadomienia](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) otrzymywane przed wygaśnięciem bieżącego certyfikatu.</span><span class="sxs-lookup"><span data-stu-id="bcd5a-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="bcd5a-114">Krok 4 jest opcjonalny.</span><span class="sxs-lookup"><span data-stu-id="bcd5a-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="bcd5a-115">Zmienianie opcji podpisywania certyfikatu SAML aplikacji i algorytmu podpisywania certyfikatu.</span><span class="sxs-lookup"><span data-stu-id="bcd5a-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="bcd5a-116">Aby uzyskać więcej informacji, zobacz [Zmienianie opcji podpisywania certyfikatów i algorytmu podpisywania.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)</span><span class="sxs-lookup"><span data-stu-id="bcd5a-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

