---
title: EmailAddress (GetPersonaType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 052055b5-4630-40ed-9b24-9e7f4bf7ba1d
description: O elemento EmailAddress (GetPersonaType) Especifica o endereço de email associado com a pessoa.
ms.openlocfilehash: a28a4a61a9719875fe99e1c950bcd3ec3af9ab13
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751985"
---
# <a name="emailaddress-getpersonatype"></a><span data-ttu-id="e3b83-103">EmailAddress (GetPersonaType)</span><span class="sxs-lookup"><span data-stu-id="e3b83-103">EmailAddress (GetPersonaType)</span></span>

<span data-ttu-id="e3b83-104">O elemento **EmailAddress (GetPersonaType)** Especifica o endereço de email associado com a pessoa.</span><span class="sxs-lookup"><span data-stu-id="e3b83-104">The **EmailAddress (GetPersonaType)** element specifies the email address associated with the persona.</span></span> 
  
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

 <span data-ttu-id="e3b83-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="e3b83-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e3b83-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e3b83-106">Attributes and elements</span></span>

<span data-ttu-id="e3b83-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e3b83-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e3b83-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e3b83-108">Attributes</span></span>

<span data-ttu-id="e3b83-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e3b83-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e3b83-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e3b83-110">Child elements</span></span>

<span data-ttu-id="e3b83-111">[Nome (string)](name-string.md) | [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) | [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) | [MailboxType](mailboxtype.md) | [ItemId](itemid.md) | [OriginalDisplayName](originaldisplayname.md)</span><span class="sxs-lookup"><span data-stu-id="e3b83-111">[Name (string)](name-string.md) | [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) | [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) | [MailboxType](mailboxtype.md) | [ItemId](itemid.md) | [OriginalDisplayName](originaldisplayname.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e3b83-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e3b83-112">Parent elements</span></span>

[<span data-ttu-id="e3b83-113">GetPersona</span><span class="sxs-lookup"><span data-stu-id="e3b83-113">GetPersona</span></span>](getpersona.md)
  
## <a name="remarks"></a><span data-ttu-id="e3b83-114">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="e3b83-114">Remarks</span></span>

<span data-ttu-id="e3b83-115">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e3b83-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="e3b83-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e3b83-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e3b83-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e3b83-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e3b83-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="e3b83-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e3b83-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e3b83-119">Schema Name</span></span>  <br/> |<span data-ttu-id="e3b83-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e3b83-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e3b83-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e3b83-121">Validation File</span></span>  <br/> |<span data-ttu-id="e3b83-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e3b83-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e3b83-123">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e3b83-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="e3b83-124">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="e3b83-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e3b83-125">Ver também</span><span class="sxs-lookup"><span data-stu-id="e3b83-125">See also</span></span>

- [<span data-ttu-id="e3b83-126">GetPersona</span><span class="sxs-lookup"><span data-stu-id="e3b83-126">GetPersona</span></span>](getpersona.md)
- [<span data-ttu-id="e3b83-127">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e3b83-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

