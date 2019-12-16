---
title: Ograniczanie dostępu w programie SharePoint lub OneDrive
ms.author: pebaum
author: pebaum
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 242388af3ae8887616fc123f24502a8e5ac8dfbe
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053775"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograniczanie dostępu w programie SharePoint lub OneDrive

Istnieje wiele sposobów ograniczania dostępu do usług SharePoint Online/OneDrive. Te różne metody ograniczania dostępu są opisane poniżej. 

**Ograniczenie uprawnień**

W programie SharePoint Online i OneDrive dla firm możemy ograniczyć dostęp do elementów, takich jak witryny, pliki i foldery, udzielając tylko dostępu do tych grup/osób, które powinny mieć dostęp.

- [Dostosowywanie uprawnień do listy lub biblioteki programu SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Dostosowywanie uprawnień witryny programu SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Zmienianie uprawnień do podfolderu](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Sterowanie dostępem z poziomu urządzeń niezarządzanych](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Jako administrator programu SharePoint lub globalnego w pakiecie Office 365, można zablokować lub ograniczyć dostęp do zawartości programu SharePoint i OneDrive z niezarządzanych urządzeń (te nie hybrydowy AD przyłączony lub zgodny w usłudze Intune).

**Ograniczenie lokalizacji sieciowej**

Administrator IT może kontrolować dostęp do zasobów programu SharePoint i usługi OneDrive na podstawie zdefiniowanych zaufanych lokalizacji sieciowych. Jest to również nazywane zasadami opartymi na lokalizacji. Aby uzyskać więcej informacji, zobacz [Kontrola dostępu do usługi SharePoint Online i OneDrive danych w oparciu o lokalizację sieciową](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Ograniczenie blokady witryny** 

W programie SharePoint Online masz możliwość blokowania zbioru witryn, więc nikt nie ma dostępu. Jest to ustawiane za pomocą programu PowerShell i [powłoki zarządzania programu SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) za pomocą właściwości [Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.

**Ograniczanie użytkownikom możliwości tworzenia witryn lub podwitryn**

Jako administrator programu SharePoint lub Office 365 globalnego administratora, możesz pozwolić użytkownikom na tworzenie i administrowanie własnymi witrynami programu SharePoint, określić, jakiego rodzaju witryn mogą tworzyć i określić lokalizację witryn. Aby uzyskać więcej informacji, zobacz [Zarządzanie tworzeniem witryny w programie SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

