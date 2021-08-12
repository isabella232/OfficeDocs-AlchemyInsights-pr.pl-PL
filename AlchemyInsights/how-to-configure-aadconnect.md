---
title: 646 Jak skonfigurować program AADConnect
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
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963653"
---
# <a name="configure-sync-features"></a>Konfigurowanie funkcji synchronizacji

Usługa Azure AD Połączenie zawiera kilka funkcji, które są domyślnie włączone lub które można włączyć później. Niektóre funkcje wymagają dodatkowej konfiguracji w określonych środowiskach.

- [Limity filtrowania](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) są synchronizowane z usługą Azure AD. Domyślnie wszyscy użytkownicy, kontakty, grupy i Windows 10 są synchronizowane. Obiekty można dołączać i wykluczać na podstawie domen, użytkowników OU lub innych atrybutów.

- [Synchronizacja skrótów haseł](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizuje skróty haseł z lokalnej usługi Active Directory z usługą Azure AD. Umożliwia to zarządzanie hasłami w jednej lokalizacji, ale używanie tego samego hasła zarówno w środowisku lokalnym, jak i w chmurze. Ponieważ usługa Active Directory jest autorytatywnym źródłem, można używać własnych zasad haseł.

- Funkcja samodzielnego resetowania [hasła (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) umożliwia użytkownikom samodzielne resetowanie haseł w chmurze przy jednoczesnym stosowaniu lokalnych zasad haseł.

- [Funkcja zapisu urządzenia umożliwia](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) zarejestrowanie urządzeń w usłudze Azure AD w celu ich zwrotu do lokalnej usługi Active Directory w celu uzyskania dostępu warunkowego.

- [Funkcja zapobiega przypadkowemu usunięciu](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) jest domyślnie włączona, aby zapobiec zbyt wielu jednoczesnym usunięciom obiektów (więcej niż 500 obiektów na synchronizację). Możesz zmienić to ustawienie, aby spełniało potrzeby Twojej organizacji.

- [Automatyczne uaktualnianie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) jest domyślnie włączone dla instalacji ekspresowych i pomaga zapewnić, że Twoja wersja usługi Azure AD Połączenie jest aktualna.
