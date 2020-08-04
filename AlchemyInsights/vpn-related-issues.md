---
title: Problemy związane z siecią VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555231"
---
# <a name="vpn-related-issues"></a>Problemy związane z siecią VPN

Pomyślne wdrożenie łączności sieci VPN dla klientów MDM zależy od wdrożonego profilu, który poprawnie odzwierciedla wymagania infrastruktury sieci VPN. Aby uzyskać odpowiednie ustawienia dla platform klienckich, które badasz, zobacz: 

[Ustawienia urządzenia holograficznego systemu Windows 10 i systemu Windows w celu dodawania połączeń sieci VPN przy użyciu usługi Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Dodawanie ustawień sieci VPN na urządzeniach z systemem iOS i iPadOS w usłudze Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Ustawienia urządzenia z systemem Android do konfigurowania sieci VPN w usłudze Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Dodawanie ustawień sieci VPN na urządzeniach z systemem macOS w usłudze Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Jeśli profil sieci VPN używa uwierzytelniania opartego na certyfikatach, upewnij się, że profile certyfikatów głównych i certyfikatów uwierzytelniania klienta połączone z profilem sieci VPN zostały pomyślnie wdrożone.

**Typowe problemy**

**Wdrożyłem profil sieci VPN na urządzeniu. Usługa Intune pokazuje, że zakończyło się pomyślnie, ale urządzenie nie łączy się z siecią VPN.**

Pomyślny stan oznacza, że usługa Intune pomyślnie wdrożyła profil skonfigurowany. Jednak te konfiguracje mogą nie odpowiadać wymaganiom sieci i/lub uwierzytelniania. Przejrzyj dzienniki w usłudze infrastruktury i uwierzytelniania (na serwerze sieci VPN i serwerze NPS/Radius), aby uzyskać więcej informacji na temat próby połączenia. Może być konieczna praca z zespołem infrastruktury sieciowej lub dostawcą sieci VPN innej firmy w celu zbierania i przeglądania dzienników.

**Po skonfigurowaniu niestandardowej sieci VPN dla systemu iOS funkcja sieci VPN dla aplikacji nie jest dostępna.**

Sieć VPN dla aplikacji dla urządzeń z systemem iOS w usłudze Intune jest obecnie dostępna dla określonej listy dostawców i partnerów, którzy muszą również spełniać wymagania wstępne certyfikatu przed skonfigurowaniem sieci VPN dla poszczególnych aplikacji. Aby uzyskać więcej informacji, zobacz [Konfigurowanie wirtualnej sieci prywatnej (VPN) dla urządzeń z systemem iOS/iPadOS dla aplikacji w usłudze Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Aby uzyskać więcej informacji o wszystkich typach połączeń sieci VPN w usłudze Intune, zobacz Tworzenie profilów sieci VPN w [celu nawiązania połączenia z serwerami sieci VPN w usłudze Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**Sieć VPN na żądanie systemu iOS nie jest wyzwalana, gdy jest dostępna skonfigurowana domena**

Aby przetestować automatyczne ustawienia sieci VPN, ustaw następujące wartości:

Chcę wykonać następujące czynności: **Oceń każdą próbę połączenia** 

Wybierz, czy chcesz się połączyć: **W razie potrzeby połącz się**

Gdy użytkownicy uzyskują dostęp do tych domen: **docelowa** *nazwa domeny*

Jeśli powyższa konfiguracja nie powiedzie się, dodaj następujący element:

Gdy ten adres URL jest nieosiągalny, wymuś połączenie sieci VPN: **BADURL**