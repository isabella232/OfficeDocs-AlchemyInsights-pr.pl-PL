---
title: Problemy z oświadczeniami i atrybutami tokenu
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035968"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="8b819-102">Problemy z oświadczeniami i atrybutami tokenu</span><span class="sxs-lookup"><span data-stu-id="8b819-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="8b819-103">**Aktualizowanie, konfigurowanie lub usuwanie roszczeń tokenu**</span><span class="sxs-lookup"><span data-stu-id="8b819-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="8b819-104">Korzystając z usługi Azure Active Directory (Azure AD), możesz dostosować typ [oświadczenia](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) dla żądania roli w tokenie odpowiedzi, który otrzymasz po autoryzowaniu aplikacji.</span><span class="sxs-lookup"><span data-stu-id="8b819-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="8b819-105">Deweloperzy aplikacji mogą używać opcjonalnych roszczeń w swoich aplikacjach usługi Azure AD, aby określić, które oświadczenia chcą mieć w tokenach wysyłanych do aplikacji.</span><span class="sxs-lookup"><span data-stu-id="8b819-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="8b819-106">Aby uzyskać więcej informacji, zobacz ["Zapewnianie opcjonalnych roszczeń dotyczących aplikacji".](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)</span><span class="sxs-lookup"><span data-stu-id="8b819-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="8b819-107">[Skonfiguruj oświadczenia grupy dotyczące aplikacji za pomocą usługi Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)</span><span class="sxs-lookup"><span data-stu-id="8b819-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="8b819-108">W przypadku korzystania z bezproblemowego logowania pojedynczego w aplikacji zobacz oświadczenia dotyczące dostosowywania wydane w [tokenie SAML dla aplikacji dla przedsiębiorstw.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)</span><span class="sxs-lookup"><span data-stu-id="8b819-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="8b819-109">**Mapowanie atrybutów roszczeń**</span><span class="sxs-lookup"><span data-stu-id="8b819-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="8b819-110">Aby skonfigurować zasady mapowania roszczeń przy użyciu programu PowerShell, zobacz Dostosowywanie roszczeń pominiętych w tokenach dla określonej aplikacji w dzierżawie [(wersja Preview).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)</span><span class="sxs-lookup"><span data-stu-id="8b819-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="8b819-111">Atrybuty rozszerzenia schematu katalogu zapewniają sposób przechowywania dodatkowych danych w usłudze Azure Active Directory na obiektach użytkowników i innych obiektach katalogu, takich jak grupy, szczegóły dzierżawy, podmioty zabezpieczeń usług.</span><span class="sxs-lookup"><span data-stu-id="8b819-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="8b819-112">Do emitowania roszczeń aplikacji można używać tylko atrybutów rozszerzenia obiektów użytkowników.</span><span class="sxs-lookup"><span data-stu-id="8b819-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="8b819-113">[Używanie atrybutów rozszerzenia schematu katalogu](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) w oświadczeniach opisuje sposób używania atrybutów rozszerzenia schematu katalogu do wysyłania danych użytkowników do aplikacji w oświadczeniach tokenu.</span><span class="sxs-lookup"><span data-stu-id="8b819-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="8b819-114">Aby uzyskać więcej informacji na temat roszczeń tokenu, zobacz:</span><span class="sxs-lookup"><span data-stu-id="8b819-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="8b819-115">Roszczenia w tokenach dostępu</span><span class="sxs-lookup"><span data-stu-id="8b819-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="8b819-116">Roszczenia w id_token</span><span class="sxs-lookup"><span data-stu-id="8b819-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="8b819-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="8b819-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="8b819-118">Odwołanie do roszczeń tokenu SAML</span><span class="sxs-lookup"><span data-stu-id="8b819-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
