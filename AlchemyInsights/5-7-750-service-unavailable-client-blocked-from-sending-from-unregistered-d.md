---
title: 1048 5.7.750 Usługa jest niedostępna. Klient zablokowany na wysyłanie z niezarejestrowanych domen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 5879c5996a28e8e9e61c696c51e7c590d1245ba1
ms.sourcegitcommit: edb9be61ff8c4df2a600f70952f6fa731c2093a9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/04/2021
ms.locfileid: "52774261"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="aa4d7-103">5.7.750 Zablokowano wysyłanie z niezarejestrowanych domen przez klienta</span><span class="sxs-lookup"><span data-stu-id="aa4d7-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="aa4d7-104">Ten błąd występuje, gdy z domen, które nie mają obsługi administracyjnej, wysyłanych jest duża liczba wiadomości (dodano jako zaakceptowane domeny i sprawdzono ich poprawność).</span><span class="sxs-lookup"><span data-stu-id="aa4d7-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="aa4d7-105">Aby uniknąć tego błędu, możesz użyć łącznika przepływu poczty opartego na certyfikacie, w którym domena certyfikatu jest domeną aprowizacyjną, lub możesz aprowizować wszystkie domeny wysyłające.</span><span class="sxs-lookup"><span data-stu-id="aa4d7-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>

<span data-ttu-id="aa4d7-106">Aby uzyskać więcej informacji, zobacz Rozwiązywanie problemów dotyczących dostarczania wiadomości e-mail związanych z kodami błędów [od 5.7.700 do 5.7.750 w programie Exchange Online.](https://go.microsoft.com/fwlink/?linkid=2164955)</span><span class="sxs-lookup"><span data-stu-id="aa4d7-106">For more information, see [Fix email delivery issues for error codes 5.7.700 through 5.7.750 in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).</span></span>