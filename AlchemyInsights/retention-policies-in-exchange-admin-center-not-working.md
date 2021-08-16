---
title: Zasady przechowywania w Exchange administracyjnej nie działają
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074942"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Zasady przechowywania w Exchange administracyjnym

Jeśli chcesz, abyśmy uruchamiali automatyczne testy ustawień wymienionych poniżej, wybierz przycisk wstecz < — u góry tej strony, a następnie wprowadź adres e-mail użytkownika, który ma problemy z zasadami przechowywania.

Jeśli w Centrum administracyjnym programu Exchange występują problemy z zasadami przechowywania, które nie mają zastosowania do skrzynek pocztowych lub elementów nieunoszących się do archiwaowej skrzynki pocztowej, sprawdź następujące kwestie:

**Główne przyczyny:**

- **Asystent folderów zarządzanych** nie przetworzył skrzynki pocztowej użytkownika. Asystent folderów zarządzanych co siedem dni podejmuje próbę przetwarzania każdej skrzynki pocztowej w organizacji opartej na chmurze.

  **Rozwiązanie:** Uruchom asystenta folderów zarządzanych.

- **W skrzynce pocztowej** **włączono funkcję RetentionHold.** Jeśli skrzynka pocztowa została umieszczona na wartości retentionhold, zasady przechowywania w skrzynce pocztowej nie będą przetwarzane w tym czasie.

  **Rozwiązanie:** Sprawdź stan ustawienia Hold (Przechowywanie) i zaktualizuj je zgodnie z potrzebami. Aby uzyskać szczegółowe informacje, zobacz [Przechowywanie skrzynki pocztowej.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Uwaga:** Jeśli skrzynka pocztowa jest mniejsza niż 10 MB, Asystent folderów zarządzanych nie będzie automatycznie przetwarzał tej skrzynki.
 
Aby uzyskać więcej informacji na temat zasad przechowywania w centrum Exchange administracyjnego, zobacz:

- [Tagi przechowywania i zasady przechowywania](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Stosowanie zasad przechowywania do skrzynek pocztowych lub](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [Dodawanie lub usuwanie tagów przechowywania](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Jak określić typ hold'a umieszczonego w skrzynce pocztowej](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
