---
title: 646 jak skonfigurować AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: dd6d6986b23c8adcc98fe713bacf32fb5bf8b4b6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29915593"
---
# <a name="configure-sync-features"></a>Konfigurowanie funkcji synchronizacji

Azure AD Connect zawiera kilka funkcji, które są domyślnie włączone, lub można włączyć później. Niektóre funkcje wymagają dodatkowej konfiguracji w konkretnych środowiskach.
  
- Limitów [Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) obiekty są synchronizowane Azure AD. Domyślnie wszystkie użytkownicy, kontakty, grupy, i Windows 10 kont komputerów są synchronizowane. Można uwzględnić lub wykluczyć na podstawie domen, jednostek organizacyjnych lub innych atrybutów obiektów. 
    
- [Synchronizacja mieszania hasła](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizuje wartość skrótu hasła w usłudze Active Directory lokalnie usługą Azure AD. Dzięki temu zarządzanie hasłami w jednym miejscu, ale korzystanie z tego samego hasła w obu lokalnych i środowiskach w chmurze. Ponieważ usługa Active Directory jest autorytatywnym źródłem informacji, można użyć własnych zasad haseł. 
    
- [Resetowania hasła Sklep internetowy (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) umożliwia użytkownikom resetowania haseł w chmurze podczas nadal stosowania zasad haseł użytkownika lokalnego. 
    
- [Urządzenie stornowania](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) pozwala zarejestrowanych urządzeń w Azure AD być zapisywane z powrotem na lokalnej usługi Active Directory, mogą być używane dla dostępu warunkowego. 
    
- [Zapobiegaj przypadkowym usunięciom](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) jest domyślnie włączona w celu zapobiegania usuwanie zbyt wiele równoczesnych obiektu (ponad 500 obiektów na synchronizacji). Można zmienić to ustawienie, aby zaspokoić potrzeby organizacji. 
    
- [Automatyczne uaktualnienie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) jest włączona domyślnie dla instalacji express i pomaga zapewnić, że używanej wersji Azure Połącz AD jest zawsze aktualna. 
    

