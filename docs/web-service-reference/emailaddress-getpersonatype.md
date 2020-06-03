---
title: EmailAddress (getpersonatype)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 052055b5-4630-40ed-9b24-9e7f4bf7ba1d
description: O elemento EmailAddress (getpersonatype) especifica o endereço de email associado ao persona.
ms.openlocfilehash: b58f61202cd94ff282b21138b47b40887b38752a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463451"
---
# <a name="emailaddress-getpersonatype"></a><span data-ttu-id="ddfb5-103">EmailAddress (getpersonatype)</span><span class="sxs-lookup"><span data-stu-id="ddfb5-103">EmailAddress (GetPersonaType)</span></span>

<span data-ttu-id="ddfb5-104">O elemento **EmailAddress (Getpersonatype)** especifica o endereço de email associado ao persona.</span><span class="sxs-lookup"><span data-stu-id="ddfb5-104">The **EmailAddress (GetPersonaType)** element specifies the email address associated with the persona.</span></span> 
  
```XML
<EmailAddress>
    <Name></Name>
    <EmailAddress></EmailAddress>
    <RoutingType></RoutingType>
    <MailboxType></MailboxType>
    <ItemId></ItemId>
    <OriginalDisplayName></OriginalDisplayName>
</EmailAddress>>
```

 <span data-ttu-id="ddfb5-105">**EmailAddresstype**</span><span class="sxs-lookup"><span data-stu-id="ddfb5-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ddfb5-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ddfb5-106">Attributes and elements</span></span>

<span data-ttu-id="ddfb5-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ddfb5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ddfb5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ddfb5-108">Attributes</span></span>

<span data-ttu-id="ddfb5-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ddfb5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ddfb5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ddfb5-110">Child elements</span></span>

<span data-ttu-id="ddfb5-111">[Nome (cadeia de caracteres)](name-string.md)  |  [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)  |  [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)  |  [MailboxType](mailboxtype.md)  |  [ItemId](itemid.md)  |  [OriginalDisplayName](originaldisplayname.md)</span><span class="sxs-lookup"><span data-stu-id="ddfb5-111">[Name (string)](name-string.md) | [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) | [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) | [MailboxType](mailboxtype.md) | [ItemId](itemid.md) | [OriginalDisplayName](originaldisplayname.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ddfb5-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ddfb5-112">Parent elements</span></span>

[<span data-ttu-id="ddfb5-113">Getpersona</span><span class="sxs-lookup"><span data-stu-id="ddfb5-113">GetPersona</span></span>](getpersona.md)
  
## <a name="remarks"></a><span data-ttu-id="ddfb5-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="ddfb5-114">Remarks</span></span>

<span data-ttu-id="ddfb5-115">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ddfb5-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="ddfb5-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ddfb5-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ddfb5-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ddfb5-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ddfb5-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="ddfb5-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ddfb5-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ddfb5-119">Schema Name</span></span>  <br/> |<span data-ttu-id="ddfb5-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ddfb5-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ddfb5-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ddfb5-121">Validation File</span></span>  <br/> |<span data-ttu-id="ddfb5-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ddfb5-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ddfb5-123">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ddfb5-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="ddfb5-124">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="ddfb5-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ddfb5-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="ddfb5-125">See also</span></span>

- [<span data-ttu-id="ddfb5-126">Getpersona</span><span class="sxs-lookup"><span data-stu-id="ddfb5-126">GetPersona</span></span>](getpersona.md)
- [<span data-ttu-id="ddfb5-127">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ddfb5-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

