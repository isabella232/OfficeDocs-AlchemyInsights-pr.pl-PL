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
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Rozwiązywanie problemów z certyfikatem podpisywania SAML

Aby rozwiązać problem z certyfikatem podpisywania SAML, wykonaj następujące zalecane czynności:

1. Po dodaniu aplikacji przedsiębiorstwa, która obsługuje logowanie jednokrotne, platforma Azure wygeneruje certyfikat nazywany certyfikatem [podpisywania SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications) Ten certyfikat ma datę wygaśnięcia 3 lat. Aby zmienić datę wygaśnięcia certyfikatu, zobacz Dostosowywanie daty wygaśnięcia certyfikatu federacji i wycofywanie go [do nowego certyfikatu.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)
2. Platforma Azure użyje tego certyfikatu do podpisania tokenów SAML żądanych przez aplikację i wysłania ich do aplikacji w celu pomyślnego logowania jednokrotnego. Aby to ukończyć, pobierz certyfikat z portalu Azure Portal i wyślij go dostawcy aplikacji, aby ukończyć proces logowania jednokrotnego.

Po zakończeniu tego procesu aplikacja będzie ufać temu certyfikatowi i wszystkie tokeny SAML podpisane przez ten certyfikat zostaną zaakceptowane przez aplikację.

3. Jeśli ten certyfikat wygaśnie, utwórz nowy certyfikat, zaktualizuj go u dostawcy aplikacji, a następnie uacyjnij po stronie platformy Azure. Aby uzyskać więcej informacji, [zobacz Odnawianie certyfikatu, który wkrótce wygaśnie.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)

> [!NOTE]
> Jeśli certyfikat wygaśnie, użytkownik nie zostanie zablokowany.

4. [Dodaj adres e-mail, aby powiadomienia](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) otrzymywane przed wygaśnięciem bieżącego certyfikatu.

> [!NOTE]
> Krok 4 jest opcjonalny.

5. Zmienianie opcji podpisywania certyfikatu SAML aplikacji i algorytmu podpisywania certyfikatu. Aby uzyskać więcej informacji, zobacz [Zmienianie opcji podpisywania certyfikatów i algorytmu podpisywania.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)

