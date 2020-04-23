---
title: 646 Jak skonfigurować AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722573"
---
# <a name="configure-sync-features"></a>Konfigurowanie funkcji synchronizacji

Usługa Azure AD Connect zawiera kilka funkcji, które są domyślnie włączone lub które można włączyć później. Niektóre funkcje wymagają dodatkowej konfiguracji w określonych środowiskach.

- [Filtrowanie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) ogranicza obiekty są synchronizowane z usługą Azure AD. Domyślnie wszyscy użytkownicy, kontakty, grupy i konta komputerów z systemem Windows 10 są synchronizowane. Obiekty można dołączać lub wykluczać na podstawie domen, obiektów organizacyjnych lub innych atrybutów.

- [Synchronizacja skrótu hasła](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizuje skrót hasła z lokalnej usługi Active Directory do usługi Azure AD. Umożliwia to zarządzanie hasłami w jednej lokalizacji, ale używanie tego samego hasła zarówno w środowisku lokalnym, jak i w chmurze. Ponieważ usługa Active Directory jest źródłem autorytatywnym, można użyć własnych zasad haseł.

- [Samoobsługowe resetowanie haseł (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) umożliwia użytkownikom resetowanie własnych haseł w chmurze przy jednoczesnym stosowaniu lokalnych zasad haseł.

- [Zapis wsteczny urządzenia](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) umożliwia zarejestrowanym urządzeniom w usłudze Azure AD zapisywanie z powrotem w lokalnej usłudze Active Directory, dzięki czemu mogą być używane do dostępu warunkowego.

- [Zapobieganie przypadkowym usuwaniom](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) jest domyślnie włączone, aby zapobiec zbyt wielu równoczesnym usuwaniom obiektów (ponad 500 obiektów na synchronizację). To ustawienie można zmienić w celu zaspokojenia potrzeb organizacji.

- [Automatyczne uaktualnianie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) jest domyślnie włączone dla instalacji ekspresowych i pomaga upewnić się, że twoja wersja usługi Azure AD Connect jest zawsze aktualna.
