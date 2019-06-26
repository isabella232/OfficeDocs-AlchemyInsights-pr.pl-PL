---
title: Ograniczanie dostępu w programie SharePoint lub OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: db84f77208dca60c6dee98cdb0c7f1ea7fa8fe17
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223722"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograniczanie dostępu w programie SharePoint lub OneDrive

Istnieje wiele sposobów, aby ograniczyć dostęp do usług SharePoint Online/OneDrive. Te różne metody ograniczania dostępu są przedstawione poniżej. 

**Ograniczenie uprawnień**

W SharePoint Online i OneDrive dla firmy możemy ograniczyć dostęp do elementów, takich jak witryny, pliki i foldery tylko udzielenie dostępu do tych grup/użytkowników, którzy powinni mieć dostęp.

- [Dostosowywanie uprawnień dla listy programu SharePoint lub biblioteki](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Dostosowywanie uprawnień witryny programu SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Należy zmienić uprawnienia do podfolderu](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Sterowanie dostępem z poziomu urządzeń niezarządzanych](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Jako programu SharePoint lub administratora globalnego w usłudze Office 365, możesz zablokować lub ograniczyć dostęp do zawartości programu SharePoint i OneDrive z niezarządzanych urządzeń (tych mieszańców AD sprzężone lub zgodny w usłudze Intune).

**Ograniczenia lokalizacji w sieci**

Jako administrator można kontrolować dostęp do zasobów programu SharePoint i OneDrive w oparciu o zaufanych lokalizacji sieci. To jest również znany jako zasad opartych na lokalizacji. Aby uzyskać więcej informacji zobacz [Kontrola dostępu do programu SharePoint w trybie Online i OneDrive dane oparte na lokalizacji sieciowej](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Ograniczenia blokowanie witryny** 

W ramach programu SharePoint w trybie Online mają zdolność do blokowania zbioru witryn, dlatego nikt nie ma dostępu. To jest ustawiany za pomocą środowiska PowerShell i [Online powłoki zarządzania programu SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) przy użyciu właściwości - LockState [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) .

**Zabronić użytkownikom tworzenie witryn i podwitryn**

Jako administrator programu SharePoint lub globalnego administratora usługi Office 365, można pozwolić użytkownikom tworzyć i administrować własnych witryn programu SharePoint, określić, jakiego rodzaju witryn mogą utworzyć, a następnie określ lokalizację witryny. Aby uzyskać więcej informacji zobacz [Tworzenie witryny Zarządzanie w dokumentacji Online programu SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation)

