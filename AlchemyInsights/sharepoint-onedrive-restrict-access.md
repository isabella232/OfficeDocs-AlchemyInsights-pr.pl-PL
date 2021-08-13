---
title: Ograniczanie dostępu w SharePoint lub OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093846"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograniczanie dostępu w SharePoint lub OneDrive

Istnieje wiele sposobów ograniczenia dostępu do usług SharePoint Online/OneDrive online. Poniżej opisano poszczególne metody ograniczeń dostępu. 

**Ograniczenie uprawnień**

W SharePoint Online i OneDrive dla Firm dostęp do elementów, takich jak witryny, pliki i foldery, ograniczamy, udzielając dostępu tylko tym grupom/osobom, które powinny mieć dostęp.

- [Dostosowywanie uprawnień dla listy SharePoint lub biblioteki](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Dostosowywanie SharePoint witryny](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Zmienianie uprawnień w podfolderze](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Sterowanie dostępem z poziomu urządzeń niezarządzanych](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Jako administrator SharePoint lub administrator globalny możesz zablokować lub ograniczyć dostęp do zawartości usług SharePoint i OneDrive z urządzeń nieza zarządzania (tych, które nie są przyłączone ani zgodne w usłudze Ad hybrydowej w usłudze Intune).

**Ograniczenie lokalizacji sieciowej**

Jako administrator IT możesz sterować dostępem do zasobów SharePoint i OneDrive na podstawie zdefiniowanych lokalizacji sieciowych, którym ufasz. Zasady te są również nazywane zasadami opartymi na lokalizacji. Aby uzyskać więcej informacji, zobacz Kontrolowanie dostępu do [SharePoint online OneDrive danych na podstawie lokalizacji sieciowej.](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Ograniczenie blokady witryny** 

W SharePoint Online możesz zablokować zbiór witryn, aby nikt nie miał do niego dostępu. Jest on ustawiany za pośrednictwem programu PowerShell i powłoki SharePoint [zarządzania online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) przy użyciu właściwości [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Ograniczanie użytkownikom możliwości tworzenia witryn lub podwitryn**

Jako administrator SharePoint lub administrator globalny, możesz umożliwiać użytkownikom tworzenie własnych witryn SharePoint i administrowanie tymi witrynami, określanie rodzaju witryn, jakie mogą tworzyć, oraz określanie ich lokalizacji. Aby uzyskać więcej informacji, zobacz [Zarządzanie tworzeniem witryn w u SharePoint Online.](https://docs.microsoft.com/sharepoint/manage-site-creation)

