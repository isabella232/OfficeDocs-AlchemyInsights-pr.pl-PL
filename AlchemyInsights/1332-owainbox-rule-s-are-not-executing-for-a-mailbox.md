---
title: 1332 OWA - reguł skrzynki odbiorczej są nie może być wykonane dla skrzynki pocztowej
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 0d3b7ce3d6b32d94a012eb3767c0747eed80f6e5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29915814"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Reguły skrzynki odbiorczej nie działa zgodnie z oczekiwaniami

Sprawdź następujące ustawienia:
  
- Wiadomości mogą być przekierowane, przekazany został lub odpowiedzi automatycznie na podstawie reguł skrzynki odbiorczej tylko jeden raz. Trwa przeadresowanie reguła (reguła skrzynki odbiorczej lub reguły przepływu poczty, znany również jako reguły transportu) można dodać maksymalnie dziesięć adresatów przekazywanie do wiadomości. Aby uzyskać więcej informacji zobacz [ograniczenia reguły dziennika, transportu i skrzynki odbiorczej](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).
    
- Reguły skrzynki odbiorczej nie działają na Skrzynka pocztowa dziennika alternatywny. Aby uzyskać więcej informacji o skrzynce pocztowej rejestrowanie alternatywny zobacz [Skrzynka pocztowa dziennika alternatywny](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).
    
Aby rozwiązać te problemy, zobacz [KB 2829319](https://support.microsoft.com/kb/2829319).
  
Jeżeli nie stosuje się poprzednie wydania, uruchom raport diagnostyczny reguły skrzynki odbiorczej przed zgłosić ten problem firmie Microsoft Support:
  
1. Otwieranie skrzynki pocztowej w programie Outlook w sieci web, a następnie kliknij przycisk **Ustawienia** \> **Opcje** \> **e-mail Organizuj** \> **reguł skrzynki odbiorczej**.
    
2. U dołu strony kliknij przycisk **Jeśli reguły nie działają kliknij tutaj, aby wygenerować raport diagnostyczny**.
    

