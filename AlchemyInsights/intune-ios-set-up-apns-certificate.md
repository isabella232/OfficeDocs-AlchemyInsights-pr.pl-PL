---
title: Konfigurowanie certyfikatu APNS dla usługi Intune na urządzeniu z systemem iOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "3543"
ms.openlocfilehash: 66590b8a063e74e80bbe3e1e497c596d63a54ece
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824049"
---
# <a name="intune-ios-set-up-apns-certificate"></a><span data-ttu-id="fd857-102">Konfigurowanie certyfikatu APNS dla usługi Intune na urządzeniu z systemem iOS</span><span class="sxs-lookup"><span data-stu-id="fd857-102">Intune iOS set up APNS certificate</span></span>

<span data-ttu-id="fd857-103">Certyfikat Apple dla aktywnej komunikacji MDM (nazywany również Usługą powiadomień w trybie push firmy Apple — APNS) nie został skonfigurowany dla Twojej subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="fd857-103">An Apple MDM Push certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured on your subscription.</span></span>

<span data-ttu-id="fd857-104">Bez skonfigurowania certyfikatu Apple dla aktywnej komunikacji MDM nie można rejestrować w usłudze urządzeń z systemem iOS i MacOS ani zarządzać tymi urządzeniami.</span><span class="sxs-lookup"><span data-stu-id="fd857-104">Without an Apple MDM Push certificate configured, you'll be unable to enroll and manage iOS and MacOS devices.</span></span> <span data-ttu-id="fd857-105">Po dodaniu certyfikatu do usługi Intune użytkownicy będą mogli zainstalować aplikację Portal firmy, aby zarejestrować swoje urządzenia z systemem iOS.</span><span class="sxs-lookup"><span data-stu-id="fd857-105">After you add the certificate to Intune, your users can install the Company Portal app to enroll their iOS devices.</span></span>

<span data-ttu-id="fd857-106">W artykule dostępnym po kliknięciu poniższego linku znajdziesz przewodnik opisujący krok po kroku dodawanie certyfikat APNS do dzierżawy usługi Intune:</span><span class="sxs-lookup"><span data-stu-id="fd857-106">For a step-by-step guide to adding an APNS certificate to your Intune tenant, please review the content on the following link:</span></span>

- [<span data-ttu-id="fd857-107">Pobierz certyfikat Apple dla aktywnej komunikacji MDM</span><span class="sxs-lookup"><span data-stu-id="fd857-107">Get an Apple MDM Push certificate</span></span>](https://docs.microsoft.com/mem/intune/enrollment/apple-mdm-push-certificate-get)

<span data-ttu-id="fd857-108">Jeśli występują problemy z certyfikatem Apple dla aktywnej komunikacji MDM (APNs), zapoznaj się z tym wpisem na blogu: [Usługa Intune i certyfikat APNs — często zadawane pytania i typowe problemy](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)</span><span class="sxs-lookup"><span data-stu-id="fd857-108">If you are having issues with the Apple Push Notification certificate (APNs) refer to this blog post: [Intune and the APNs certificate: FAQ and common issues](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)</span></span>
