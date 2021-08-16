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
ms.openlocfilehash: 3aacc3c6675f4102a5b34a435c862215dbfd0479b75549d608ed3c91021ed3d7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031416"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Wdrażanie dodatków dla aplikacji Aplikacje Microsoft 365

Scentralizowane wdrażanie to zalecany sposób wdrażania dodatków Office użytkowników i grup w organizacji. Aby wdrożyć dodatki, wykonaj poniższe czynności:

**Uwaga:** Aby zainstalować dodatki dla użytkowników Office użytkowników, zobacz Wyświetlanie i instalowanie dodatków oraz zarządzanie nimi w [Office programów.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Upewnij się też, że jest włączone indywidualne Office dodatków ze Sklepu. Aby uzyskać szczegółowe informacje, zobacz Uniemożliwianie pobierania dodatków przez wyłączenie [Sklepu Office wszystkich](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)klientów (z wyjątkiem Outlook).

1. Upewnij się, że Twoje środowisko spełnia wymagania dotyczące wdrażania dodatków przy użyciu funkcji scentralizowanego wdrażania. Aby uzyskać szczegółowe informacje, zobacz [Wymagania.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)
2. Przejdź do **Ustawienia** zintegrowane aplikacje Uzyskaj aplikacje w aplikacji centrum administracyjne platformy Microsoft 365, aby wdrożyć  >    >   dodatki. 

Uwagi: 

- Zintegrowane aplikacje wymagają, aby administrator ma uprawnienia administratora globalnego Exchange administratora.

- W przypadku wdrażania dodatków u wielu użytkowników zalecamy przypisywanie ich przy użyciu grup, a nie pojedynczych użytkowników. Aby uzyskać szczegółowe informacje, zobacz Zagadnienia dotyczące przypisywania dodatku [do użytkowników i grup.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- Scentralizowane wdrażanie nie obsługuje użytkowników w zagnieżdżonych grupach, które mają grupy nadrzędne. Aby uzyskać szczegółowe informacje, [zobacz Przydziały użytkowników i grup.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- Upewnij się, że usługa zarządzania Microsoft 365 (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') jest włączona dla użytkowników w celu zalogowania się. Aby uzyskać szczegółowe informacje, [zobacz Konfigurowanie właściwości aplikacji.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)

- Jeśli podczas wdrażania dodatków za pomocą zintegrowanych aplikacji wystąpią problemy, spróbuj wdrożyć je przy użyciu [dodatków.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

Więcej informacji można znaleźć w następujących artykułach:

[Wdrażanie dodatków w centrum administracyjnym](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Zarządzanie dodatki w centrum administracyjnym](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Zarządzanie dodatkimi przy użyciu poleceń cmdlet](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) programu PowerShell dla funkcji Scentralizowane wdrażanie 
 [Publikowanie Office dodatków przy użyciu funkcji scentralizowanego wdrażania za pośrednictwem centrum administracyjne platformy Microsoft 365](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Rozwiązywanie problemów: Użytkownik nie widzi dodatków](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Rozwiązywanie problemów użytkowników z Office dodatków](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)