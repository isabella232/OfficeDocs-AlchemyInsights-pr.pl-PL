---
title: Zasady przechowywania w Centrum administracyjnym programu Exchange nie działają
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
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952238"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Zasady przechowywania w Centrum administracyjnym programu Exchange

Jeśli chcesz, abyśmy uruchamiali automatyczne testy ustawień wymienionych poniżej, wybierz przycisk wstecz < — u góry tej strony, a następnie wprowadź adres e-mail użytkownika, który ma problemy z zasadami przechowywania.

Jeśli masz problemy z zasadami przechowywania w Centrum administracyjnym programu Exchange, które nie mają zastosowania do skrzynek pocztowych lub elementów, które nie są przenoszące do archiwaowej skrzynki pocztowej, sprawdź następujące kwestie:

**Główne przyczyny:**

- **Asystent folderów zarządzanych** nie przetworzył skrzynki pocztowej użytkownika. Asystent folderów zarządzanych co siedem dni podejmuje próbę przetwarzania każdej skrzynki pocztowej w organizacji opartej na chmurze.

  **Rozwiązanie:** Uruchom asystenta folderów zarządzanych.

- **W skrzynce pocztowej** **włączono funkcję RetentionHold.** Jeśli skrzynka pocztowa została umieszczona na wartości retentionhold, zasady przechowywania w skrzynce pocztowej nie będą przetwarzane w tym czasie.

  **Rozwiązanie:** Sprawdź stan ustawienia Hold (Przechowywanie) i zaktualizuj je zgodnie z potrzebami. Aby uzyskać szczegółowe informacje, zobacz [Przechowywanie skrzynki pocztowej.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Uwaga:** Jeśli skrzynka pocztowa jest mniejsza niż 10 MB, Asystent folderów zarządzanych nie będzie automatycznie przetwarzał tej skrzynki.
 
Aby uzyskać więcej informacji na temat zasad przechowywania w Centrum administracyjnym programu Exchange, zobacz:

- [Tagi przechowywania i zasady przechowywania](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Stosowanie zasad przechowywania do skrzynek pocztowych lub](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [Dodawanie lub usuwanie tagów przechowywania](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Jak określić typ hold'a umieszczonego w skrzynce pocztowej](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
