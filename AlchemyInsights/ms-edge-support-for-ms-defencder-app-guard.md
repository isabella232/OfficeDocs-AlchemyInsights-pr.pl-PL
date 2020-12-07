---
title: Pomoc techniczna Microsoft Edge na potrzeby aplikacji Microsoft Defender Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584015"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Pomoc techniczna Microsoft Edge na potrzeby aplikacji Microsoft Defender Application Guard

Funkcja Application Guard przeznaczona dla systemu Windows 10 i Microsoft Edge korzysta z podejścia do izolacji sprzętu, które umożliwia użytkownikowi nawigację po niezaufanej witrynie wewnątrz izolowanego kontenera funkcji Hyper-V, oddzielonym od systemu operacyjnego hosta.

Administrator przedsiębiorstwa zdefiniował listę zaufanych witryn internetowych, zasobów chmur i sieci wewnętrznych. Gdy użytkownik odwiedzi witrynę, której nie ma na liście, program Microsoft Edge otworzy witrynę w kontenerze. Oznacza to, że jeśli witryna stanie się szkodliwa, komputer hosta pozostanie chroniony, a osoba atakująca nie będzie mogła uzyskać dostępu do danych przedsiębiorstwa.

Instalacja rozszerzeń w kontenerze jest obsługiwana w programie Microsoft Edge w wersji 81 i może być kontrolowana za pośrednictwem zasad. Adres updateURL, który jest wykorzystywany w zasadach ExtensionInstallForcelist, należy dodać jako zasób neutralny w zasadach izolacji sieciowej, które są używane przez funkcję Application Guard.

Aby uzyskać więcej informacji, zobacz [Pomoc techniczna Microsoft Edge dla usługi Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).
