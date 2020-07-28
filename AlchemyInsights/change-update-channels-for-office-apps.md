---
title: Zmienianie kanałów aktualizacji dla aplikacji pakietu Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440016"
---
# <a name="change-update-channels-for-office-apps"></a>Zmienianie kanałów aktualizacji dla aplikacji pakietu Office

W przypadku nowych instalacji pakietu Office użyj ustawień pobierania oprogramowania pakietu Office, aby wybrać żądany kanał aktualizacji, a następnie zainstaluj (lub zainstaluj ponownie) aplikacje pakietu Office. Aby uzyskać więcej informacji, zobacz [Zarządzanie ustawieniami pobierania oprogramowania w usłudze Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Uwaga** Kanał aktualizacji wybrany przy użyciu ustawień pobierania oprogramowania pakietu Office dotyczy wszystkich użytkowników wykonujących nowe instalacje za pomocą portalu usługi O365. Aby uzyskać więcej informacji, zobacz [Pobieranie i instalowanie lub ponowne instalowanie usługi Microsoft 365 lub Office 2019 na komputerze PC lub Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

W przypadku istniejących instalacji pakietu Office użyj narzędzia wdrażania pakietu Office (ODT), aby przełączyć się na inny kanał aktualizacji:  

1. Pobierz najnowszą wersję narzędzia wdrażania pakietu Office (setup.exe) z [Centrum pobierania Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Zidentyfikuj nazwę kanału, na który chcesz się przełączyć. Aby uzyskać więcej informacji, zobacz [Opcje konfiguracji Narzędzia wdrażania pakietu Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Utwórz plik XML konfiguracji określający odpowiednią nazwę kanału, na przykład update.xml.  
    a. <Configuration>  
    b. <Aktualizacje **Channel ="Miesięczne"** />  
    c. </Configuration>
4. W wierszu polecenia z podwyższonym poziomem uprawnień przełącz się do lokalizacji folderu, w którym znajduje się setup.exe, i uruchom następujące polecenie:  
    a. setup.exe /configure update.xml
5. Uruchom aplikację pakietu Office (na przykład Excel), a następnie wybierz pozycję **Konto pliku**  >  **Account**. W sekcji Informacje o produkcie wybierz pozycję **Aktualizuj opcje**  >  **aktualizacji teraz**.

Aby uzyskać więcej informacji, zobacz [Jak przełączyć kanały aktualizacji dla istniejących aplikacji pakietu Office](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Aby przełączać kanały aktualizacji dla wybranej grupy użytkowników lub za pomocą programu Menedżer konfiguracji (SCCM), należy skonfigurować ustawienie Aktualizuj kanał przy użyciu obiektu zasad grupy. Aby uzyskać więcej informacji, zobacz [Omówienie kanałów aktualizacji aplikacji usługi Microsoft 365](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Aby uzyskać szczegółowe informacje, zobacz [Jak zarządzać kanałami proplus usługi Office 365 dla it pros](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) i [zarządzać aktualizacjami aplikacji Microsoft 365 za pomocą programu Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).