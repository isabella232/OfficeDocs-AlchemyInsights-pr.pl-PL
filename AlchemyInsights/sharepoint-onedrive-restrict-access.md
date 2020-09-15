---
title: Ograniczanie dostępu w programie SharePoint lub usłudze OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700465"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograniczanie dostępu w programie SharePoint lub usłudze OneDrive

Istnieje wiele sposobów ograniczania dostępu do usług SharePoint Online i OneDrive. Te różnorodne metody ograniczeń dostępu przedstawiono poniżej. 

**Ograniczenia uprawnień**

W usłudze SharePoint Online i usłudze OneDrive dla firm ograniczenie dostępu do elementów, takich jak witryny, pliki i foldery, jest udzielane tylko użytkownikom, którzy powinni mieć dostęp.

- [Dostosowywanie uprawnień do listy lub biblioteki programu SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Dostosowywanie uprawnień do witryny programu SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Zmienianie uprawnień w podfolderze](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Sterowanie dostępem z poziomu urządzeń niezarządzanych](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Jako administrator programu SharePoint lub administratora globalnego możesz zablokować lub ograniczyć dostęp do zawartości programu SharePoint i usługi OneDrive z urządzeń niezarządzanych (tych, które nie są dołączone lub są zgodne z usługą Intune).

**Ograniczenie lokalizacji sieciowej**

Jako administrator IT możesz kontrolować dostęp do zasobów programu SharePoint i usługi OneDrive na podstawie zdefiniowanych lokalizacji sieciowych, którym ufasz. Jest to również nazywane zasadami opartymi na lokalizacji. Aby uzyskać więcej informacji, zobacz [kontrolowanie dostępu do usługi SharePoint Online i danych usługi OneDrive na podstawie lokalizacji sieciowej](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) .

**Ograniczenie blokady witryny** 

W usłudze SharePoint Online możesz zablokować zbiór witryn, więc nikt nie ma dostępu. Jest ona ustawiana za pośrednictwem programu PowerShell i [powłoki zarządzania usługi SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) przy użyciu właściwości [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.

**Ograniczanie użytkowników do tworzenia witryn i podwitryn**

Jako administrator programu SharePoint lub Administrator globalny możesz umożliwić użytkownikom tworzenie i administrowanie swoimi witrynami programu SharePoint, Określanie rodzaju witryn, które mogą tworzyć, oraz Określanie lokalizacji witryn. Aby uzyskać więcej informacji, zobacz [Zarządzanie tworzeniem witryn w usłudze SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

