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
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678767"
---
# <a name="enable-cost-management"></a>Włączanie zarządzania kosztami

**Co oznacza "koszty są wyłączone dla Twojej organizacji"?**

Organizacje korzystające z kont Enterprise Agreement (EA) lub Microsoft Customer Agreement (MCA) mogą wyłączyć dostęp do informacji o kosztach i cenach.

Po zalogowaniu się do portalu Azure Portal może korzystać z interfejsów API rozliczeń w celu programistycznego pobierania faktur (po włączeniu) i szczegółów użycia.

**Jak zezwolić dodatkowym użytkownikom na uzyskiwanie dostępu do faktur**

1. Przejdź do **bloku subskrypcje** w portalu Azure.
2. Wybierz pozycję **faktury** , a następnie pozycję **dostęp do faktur**.
3. Włącz program Access, a następnie Zapisz zmiany, aby umożliwić użytkownikom w rolach objętych zakresem abonamentu Pobieranie faktur.

> [!NOTE]
> Administrator konta może również skonfigurować możliwość wysyłania faktur pocztą e-mail. Aby dowiedzieć się więcej, zobacz [Uzyskiwanie faktury w wiadomości e-mail](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).

**Jak dodać użytkowników do roli czytnika rozliczeń**

1. Przejdź do **bloku subskrypcje** w portalu Azure.
2. Wybierz pozycję **Kontrola dostępu (IAM)** , a następnie kliknij przycisk **Dodaj**.
3. Wybierz pozycję **czytnik rozliczeń** na stronie **Wybieranie roli** .
4. Wpisz adres e-mail użytkownika, którego chcesz zaprosić, a następnie kliknij przycisk **OK** , aby wysłać zaproszenie.
5. Postępuj zgodnie z instrukcjami podanymi w wiadomości e-mail z zaproszeniem, aby zalogować się jako czytnik rozliczeń. Aby uzyskać więcej informacji, zobacz [udzielanie dostępu do rozliczeń](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Polecane dokumenty**

- [Włączanie widoków DA i AO za pośrednictwem portalu EA](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Koszty wliczone w zarządzanie kosztami](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Obsługiwane oferty platformy Microsoft Azure](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Przegląd kosztów w analizie kosztów](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Zapewnianie dostępu do informacji o rozliczeniach](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Sprawdzanie dostępu do umowy z klientem firmy Microsoft](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






