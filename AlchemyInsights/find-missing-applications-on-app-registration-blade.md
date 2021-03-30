---
title: Znajdowanie brakujących aplikacji w bladej rejestracji aplikacji
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404700"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Znajdowanie brakujących aplikacji w bladej rejestracji aplikacji

1. Nie można znaleźć aplikacji w portalu rejestracji aplikacji.

    Jeśli aplikacja jest aplikacją wielodostępną i została zarejestrowana w innej dzierżawie, nie będzie wyświetlana w obszarze rejestracja aplikacji blade. Można jednak znaleźć go w obszarze Blade aplikacji dla przedsiębiorstw, gdy uzyska on dostęp (po zakończeniu zgody) i zostanie utworzony podmiot zabezpieczeń usługi w Twojej dzierżawie. Aby uzyskać więcej informacji, zobacz Aplikacje & głównych użytkowników usługi [w usłudze Azure AD — platforma tożsamości firmy Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Nie można wyświetlić aplikacji w panelu rejestracji aplikacji, nawet jeśli jesteś administratorem.

    Upewnij się, że jesteś we właściwym katalogu w portalu Azure Portal.
3. Moja aplikacja nie jest wymieniona na liście bladej Enterprise Applications, ale pojawia się podczas wykonywania zapytań za pomocą polecenia programu PowerShell.

    Czasami po usunięciu aplikacji z portalu Azure nie jest ona pokazywana w portalu, ale może nie zostać całkowicie usunięta. Aby uzyskać więcej informacji, zobacz:
    - Możesz pobrać listę usuniętych wcześniej aplikacji i sprawdzić, czy ta aplikacja jest wyświetlona na liście za pomocą polecenia programu PowerShell: **Get-AzureADDeletedApplication.** Aby dowiedzieć się więcej, [zobacz Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Jeśli chcesz całkowicie usunąć aplikację, możesz wykonać następujące czynności w programie PowerShell: **Remove-AzureADApplication -ObjectId.** Aby dowiedzieć się więcej, [zobacz Usuwanie-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Możesz również spróbować przywrócić usuniętą aplikację, używając następującego polecenia programu PowerShell: Przywróć polecenie **AzureADDeletedApplication -ObjectId.** Aby dowiedzieć się więcej, zobacz [Przywracanie-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. Nie mogę znaleźć listy wszystkich wstępnie zainstalowanych aplikacji dla przedsiębiorstw w mojej nowej dzierżawie platformy Azure.

    Domyślnie w usłudze Azure AD nie ma wstępnie zainstalowanych aplikacji dla przedsiębiorstw. Musisz dodać go ręcznie z opcji "Nowa aplikacja", przeglądając ją z galerii usługi Azure AD lub dodać aplikację nie galerii. Aby dowiedzieć się więcej, zobacz [Szybki start: dodawanie aplikacji do dzierżawy usługi Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Jeśli jesteś administratorem globalnym, możesz łatwo uzyskać dostęp do aplikacji za pomocą ikony Uruchamianie aplikacji [platformy Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)
5. Nie mogę znaleźć moich aplikacji w portalu Moje aplikacje.

    Upewnij się, że aplikacje nie są ukryte na stronie kolekcji Moje aplikacje. Aby dowiedzieć się więcej, [zobacz Kolekcje (wersja zapoznawcza) w portalu Moje aplikacje — Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. Aby uruchomić aplikacje z portalu Moje aplikacje, zobacz Znajdowanie i & aplikacji w portalu Moje aplikacje [— Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)
7. Aplikacja Mover usługi Office 365 nie jest pokazywana na bladej aplikacji Enterprise Applications po instalacji.

    Aplikacja "Office 365 Mover" jest aplikacją z wieloma usługami, która nie musi być dodawana do AAD przy użyciu sekcji Aplikacje galerii w obszarze Rejestracja aplikacji dla przedsiębiorstw. Aby uzyskać dostęp do aplikacji Mover usługi Office 365, po prostu zaloguj się do tej aplikacji i zostanie w nim konieczne uzyskanie zgody użytkownika na te uprawnienia. Gdy użytkownik wyraża zgodę, ta aplikacja zostanie automatycznie dodana do dzierżawy przy użyciu identyfikatora e-mail, który się zalogowano.

    Po zalogowaniu się do aplikacji wpis tej aplikacji powinien być w stanie znaleźć się pod grotem aplikacji dla przedsiębiorstw w AAD. Aby wyszukać aplikację, wpisz jej imię i nazwisko, na przykład "Office 365 Mover" lub po prostu wyszukaj tekst "biuro", a aplikacja powinna zostać wyświetlona na liście. Aby dowiedzieć się więcej, zobacz Usługa [Office 365 Mover](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)informuje, że jest już zainstalowana, ale nie jest wymieniona w galerii aplikacji dla przedsiębiorstw.
8. Szybki start: Wyświetl listę aplikacji, które używają dzierżawy usługi [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) do zarządzania tożsamościami, aby dowiedzieć się, jak wyświetlić aplikacje, nazywane też aplikacjami, które zostały już ustawione do używania Twojej dzierżawy usługi Azure AD jako ich dostawcy tożsamości (IdP).
9. [Rozwiązywanie typowych problemów związanych z dodawaniem lub usuwaniem aplikacji](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) do usługi Azure Active Directory ułatwia zrozumienie typowych problemów występujących u użytkowników z wyświetlaniem aplikacji w usłudze Azure Active Directory.
