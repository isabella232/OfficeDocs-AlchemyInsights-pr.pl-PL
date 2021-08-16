---
title: Włączanie zarządzania kosztami
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: c3623aee9ab3592254ffb25aade7d52a2c7ddd49fde939956162cd4008d5ba19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003579"
---
# <a name="enable-cost-management"></a>Włączanie zarządzania kosztami

**Co oznaczają "koszty są wyłączone dla Twojej organizacji"?**

Organizacje korzystające Enterprise Agreement (EA) lub Microsoft Customer Agreement (MCA) mogą wyłączyć dostęp do informacji o kosztach i cenach.

Po zalogowaniu się do portalu Azure Portal mogą oni używać interfejsów API rozliczeń w celu programowego otrzymywania faktur (po ich rejestracji) i szczegółów użycia.

**Jak zezwolić dodatkowym użytkownikom na dostęp do faktur**

1. Przejdź do **bladej subskrypcji w** Azure Portal.
2. Wybierz **pozycję Faktury,** a **następnie dostęp do faktur.**
3. Włącz dostęp, a następnie zapisując zmiany, aby umożliwić użytkownikom pełniącym funkcje subskrypcji pobieranie faktur.

> [!NOTE]
> Administrator konta może też skonfigurować wysyłanie faktur pocztą e-mail. Aby dowiedzieć się więcej, zobacz [Uzyskiwanie faktury w wiadomości e-mail.](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)

**Jak dodać użytkowników do roli czytnika rozliczeń**

1. Przejdź do **bladej subskrypcji w** Azure Portal.
2. Wybierz **pozycję Kontrola dostępu (IAM),** a następnie kliknij przycisk **Dodaj**.
3. Wybierz **pozycję Czytnik rozliczeń** na stronie Wybierz **rolę.**
4. Wpisz adres e-mail użytkownika, którego chcesz zaprosić, a następnie kliknij przycisk **OK,** aby wysłać zaproszenie.
5. Postępuj zgodnie z instrukcjami podanymi w zaproszeniu e-mail, aby zalogować się jako czytnik rozliczeń. Aby uzyskać więcej informacji, zobacz [Udzielanie dostępu do rozliczeń.](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in)

**Polecane dokumenty**

- [Włączanie widoków DA i AO za pośrednictwem portalu EA](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Koszty zawarte w zarządzaniu kosztami](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Obsługiwane Microsoft Azure ofert](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Przeglądanie kosztów w analizie kosztów](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Zapewnianie dostępu do informacji rozliczeniowych](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Sprawdzanie dostępu do Umowy z Klientem Microsoft](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






