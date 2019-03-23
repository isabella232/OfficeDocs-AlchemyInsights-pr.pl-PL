---
title: 1048 5.7.750 usługa jest niedostępna. Klient zablokowaną możliwość wysyłania z niezarejestrowanych domen
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom: 1048
ms.openlocfilehash: 5eb42679f123fcd1b680327329721cb47e18e11a
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776511"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="a56d9-103">5.7.750 klienta zablokowaną możliwość wysyłania z niezarejestrowanych domena</span><span class="sxs-lookup"><span data-stu-id="a56d9-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="a56d9-104">Ten błąd występuje w przypadku dużej liczby wiadomości są wysyłane z domen, które nie są obsługiwane w usłudze Office 365 (dodawane jako zaakceptowane domeny i sprawdzone).</span><span class="sxs-lookup"><span data-stu-id="a56d9-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>
  
<span data-ttu-id="a56d9-105">Aby uniknąć tego błędu, można użyć łącznika przepływu poczty opartego na certyfikatach gdzie certyfikatu domena jest domeną obsługiwaną lub umożliwia obsługę wszystkich domen wysyłającego.</span><span class="sxs-lookup"><span data-stu-id="a56d9-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
  

