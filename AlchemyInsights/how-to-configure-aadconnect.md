---
title: 646 jak skonfigurować AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704499"
---
# <a name="configure-sync-features"></a>Konfigurowanie funkcji synchronizacji

Usługa Azure AD Connect zawiera kilka funkcji, które są domyślnie włączone lub można je włączyć później. Niektóre funkcje wymagają dodatkowej konfiguracji w określonych środowiskach.

- Ograniczenia [filtrowania](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) obiekty są synchronizowane z usługą Azure AD. Domyślnie synchronizowane są wszyscy użytkownicy, kontakty, grupy i konta komputerów z systemem Windows 10. Możesz uwzględnić lub wykluczyć obiekty na podstawie domen, jednostek organizacyjnych lub innych atrybutów.

- [Synchronizacja skrótu hasła](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizuje skrót hasła z lokalnej usługi Active Directory z usługą Azure AD. Umożliwia to zarządzanie hasłami w jednym miejscu, ale używanie tego samego hasła w środowiskach lokalnych i w chmurze. Usługa Active Directory jest źródłem autorytatywnym, ale można korzystać z własnych zasad haseł.

- Samoobsługowe [Resetowanie hasła (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) umożliwia użytkownikom Resetowanie własnych haseł w chmurze przy jednoczesnym stosowaniu lokalnych zasad haseł.

- [Zapisanie urządzenia](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) umożliwia zapisanie zarejestrowanych urządzeń w usłudze Azure AD z powrotem do lokalnej usługi Active Directory, aby można było ich użyć na potrzeby dostępu warunkowego.

- [Zapobieganie przypadkowemu usuwaniu](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) jest domyślnie włączone, co zapobiega zbyt wielu jednoczesnym usuwaniem obiektów (ponad 500 obiektów na synchronizację). Możesz zmienić to ustawienie, aby zaspokoić potrzeby Twojej organizacji.

- [Automatyczne uaktualnienie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) jest domyślnie włączone dla instalacji ekspresowych i zapewnia, że Twoja wersja usługi Azure AD Connect jest zawsze aktualna.
