---
title: Ograniczanie dostępu w programie SharePoint lub OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692775"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograniczanie dostępu w programie SharePoint lub OneDrive

Istnieje wiele sposobów ograniczania dostępu do usług usługi SharePoint Online/OneDrive. Te różne metody ograniczeń dostępu są opisane poniżej. 

**Ograniczenie uprawnień**

W usłudze SharePoint Online i usłudze OneDrive dla Firm ograniczamy dostęp do elementów, takich jak witryny, pliki i foldery, przyznając dostęp tylko tym grupom/osobom, które powinny mieć dostęp.

- [Dostosowywanie uprawnień do listy lub biblioteki programu SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Dostosowywanie uprawnień witryny programu SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Zmienianie uprawnień w podfolderze](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Sterowanie dostępem z poziomu urządzeń niezarządzanych](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Jako administrator programu SharePoint lub administrator globalny możesz blokować lub ograniczać dostęp do zawartości programu SharePoint i OneDrive z urządzeń niezarządzanych (tych, które nie są przyłączone do usługi AD hybrydowej lub są zgodne w usłudze Intune).

**Ograniczenie lokalizacji sieciowej**

Jako administrator IT możesz kontrolować dostęp do zasobów programu SharePoint i OneDrive na podstawie zaufanych lokalizacji sieciowych. Jest to również znane jako zasady oparte na lokalizacji. Aby uzyskać więcej informacji, zobacz [Kontrolowanie dostępu do danych usługi SharePoint Online i OneDrive na podstawie lokalizacji sieciowej](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Ograniczenie blokady witryny** 

W usłudze SharePoint Online masz możliwość zablokowania zbioru witryn, więc nikt nie ma do niego dostępu. Jest to ustawiane za pośrednictwem programu PowerShell i [powłoki zarządzania usługi SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) przy użyciu właściwości [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Ograniczanie użytkownikom tworzenia witryn lub podwitryn**

Jako administrator programu SharePoint lub administrator globalny możesz pozwolić użytkownikom tworzyć własne witryny programu SharePoint i administrować nimi, określać, jakiego rodzaju witryny mogą tworzyć, oraz określać lokalizację witryn. Aby uzyskać więcej informacji, zobacz [Zarządzanie tworzeniem witryny w usłudze SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

