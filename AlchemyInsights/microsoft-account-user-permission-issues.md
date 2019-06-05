---
title: Tworzenie i używanie udostępnionej skrzynki pocztowej
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717356"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Rozwiązywanie problemu - nie można odnaleźć w katalogu użytkownika

<p>Jeśli użytkownicy otrzymują komunikat o błędzie <strong> &ldquo; &hellip;użytkownik może&rsquo;t można znaleźć w katalogu. Spróbuj ponownie,&hellip; </strong> gdzie typ problemu jest <strong> &ldquo;użytkownika nie jest w katalogu.&rdquo;</strong>, mogą być wykonywane czynności do rozwiązania tego problemu.</p> <ol> <li>Upewnij się, konto, na którym przyjęte wiadomości e-mail z zaproszeniem jest to samo konto, który jest używany do logowania się później. Upewnij się, że użytkownik korzysta z tego samego konta aby zaakceptować zaproszenie i zalogować się do witryny. <br /><br />Aby uzyskać więcej informacji zobacz <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">jak zarządzać aliasy konta Microsoft</a> do zarządzania logowania usługi Office 365. <br /><br /></li> <li>Przejdź do każdej witryny, w której użytkownik odbiera błąd. <br /><br />. Dodaj <strong> &ldquo;/_layouts/15/people.aspx/membershipgroupid=0&rdquo; </strong> (ujęty w cudzysłów podwójny) na końcu adresu URL witryny. <br /><br />Przykład: https://&lt;contoso&gt;.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0 <br /><br />b. Wybierz użytkownika z listy. <br /><br />c. Kliknij przycisk <strong>Usuń uprawnienia użytkownika na Wstążce</strong>. <br /><br />d. Dodać z powrotem użytkownika i ponownie wysłać zaproszenia do użytkownika.</li> </ol>

