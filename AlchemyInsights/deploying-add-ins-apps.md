---
title: Wdrażanie dodatków dla aplikacji Aplikacje Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233544"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Wdrażanie dodatków dla aplikacji Aplikacje Microsoft 365

Scentralizowane wdrażanie to zalecany sposób wdrażania dodatków Office użytkowników i grup w organizacji. Aby wdrożyć dodatki, wykonaj poniższe czynności:

**Uwaga:** Aby zainstalować dodatki dla użytkowników Office użytkowników, zobacz Wyświetlanie i instalowanie dodatków oraz zarządzanie nimi w [Office programów.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Upewnij się też, że jest włączone indywidualne Office dodatków ze Sklepu. Aby uzyskać szczegółowe informacje, zobacz Uniemożliwianie pobierania dodatków przez wyłączenie [Sklepu Office wszystkich](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)klientów (z wyjątkiem Outlook).

1. Upewnij się, że Twoje środowisko spełnia wymagania dotyczące wdrażania dodatków przy użyciu funkcji scentralizowanego wdrażania. Aby uzyskać szczegółowe informacje, zobacz [Wymagania.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)
2. Przejdź do **Ustawienia**  >  **zintegrowane aplikacje** Uzyskaj aplikacje w centrum administracyjnym usługi Microsoft 365, aby wdrożyć  >   dodatki. 

Uwagi: 

- Zintegrowane aplikacje wymagają, aby administrator ma uprawnienia administratora globalnego Exchange administratora.

- W przypadku wdrażania dodatków u wielu użytkowników zalecamy przypisywanie ich przy użyciu grup, a nie pojedynczych użytkowników. Aby uzyskać szczegółowe informacje, zobacz Zagadnienia dotyczące przypisywania dodatku [do użytkowników i grup.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- Scentralizowane wdrażanie nie obsługuje użytkowników w zagnieżdżonych grupach, które mają grupy nadrzędne. Aby uzyskać szczegółowe informacje, [zobacz Przydziały użytkowników i grup.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- Upewnij się, że usługa zarządzania Microsoft 365 (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') jest włączona dla użytkowników w celu zalogowania się. Aby uzyskać szczegółowe informacje, [zobacz Konfigurowanie właściwości aplikacji.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)

- Jeśli podczas wdrażania dodatków za pomocą zintegrowanych aplikacji wystąpią problemy, spróbuj wdrożyć je przy użyciu [dodatków.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

Aby uzyskać więcej informacji, zobacz:

[Wdrażanie dodatków w centrum administracyjnym](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Zarządzanie dodatki w centrum administracyjnym](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Zarządzanie dodatkimi przy użyciu poleceń cmdlet](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) programu PowerShell dla funkcji Scentralizowane wdrażanie 
 Publikowanie Office przy użyciu [funkcji scentralizowanego wdrażania za](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) pośrednictwem Microsoft 365 administracyjnego 
 [Rozwiązywanie problemów: Użytkownik nie widzi dodatków](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Rozwiązywanie problemów użytkowników z Office dodatków](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)