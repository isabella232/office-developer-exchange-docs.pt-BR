---
title: ImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7b884e-ecf1-4e58-86ec-856b13a95f2b
description: O elemento ImGroup representa um grupo de mensagens instantâneo.
ms.openlocfilehash: 2a444158dbc6a73b1aee7b306cc251d33d005c43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823890"
---
# <a name="imgroup"></a><span data-ttu-id="cef5b-103">ImGroup</span><span class="sxs-lookup"><span data-stu-id="cef5b-103">ImGroup</span></span>

<span data-ttu-id="cef5b-104">O elemento **ImGroup** representa um grupo de mensagens instantâneo.</span><span class="sxs-lookup"><span data-stu-id="cef5b-104">The **ImGroup** element represents an instant messaging group.</span></span> 
  
```XML
<ImGroup>
   <DisplayName/>
   <GroupType/>
   <ExchangeStoreId/>
   <MemberCorrelationKey/>
   <ExtendedProperties/>
   <SmtpAddress/>
</ImGroup>
```

 <span data-ttu-id="cef5b-105">**ImGroupType**</span><span class="sxs-lookup"><span data-stu-id="cef5b-105">**ImGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cef5b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="cef5b-106">Attributes and elements</span></span>

<span data-ttu-id="cef5b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cef5b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cef5b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cef5b-108">Attributes</span></span>

<span data-ttu-id="cef5b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cef5b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cef5b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cef5b-110">Child elements</span></span>

<span data-ttu-id="cef5b-111">[DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md) | [GroupType](grouptype.md) | [ExchangeStoreId](exchangestoreid.md) | [MemberCorrelationKey](membercorrelationkey.md) | [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)  |  [ SmtpAddress](smtpaddress.md)</span><span class="sxs-lookup"><span data-stu-id="cef5b-111">[DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md) | [GroupType](grouptype.md) | [ExchangeStoreId](exchangestoreid.md) | [MemberCorrelationKey](membercorrelationkey.md) | [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md) | [SmtpAddress](smtpaddress.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cef5b-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cef5b-112">Parent elements</span></span>

<span data-ttu-id="cef5b-113">[Grupos (ArrayOfImGroupType)](groups-arrayofimgrouptype.md) | [AddDistributionGroupToImListResponse](adddistributiongrouptoimlistresponse.md) | [AddImGroupResponse](addimgroupresponse.md)</span><span class="sxs-lookup"><span data-stu-id="cef5b-113">[Groups (ArrayOfImGroupType)](groups-arrayofimgrouptype.md) | [AddDistributionGroupToImListResponse](adddistributiongrouptoimlistresponse.md) | [AddImGroupResponse](addimgroupresponse.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cef5b-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="cef5b-114">Remarks</span></span>

<span data-ttu-id="cef5b-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cef5b-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cef5b-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cef5b-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cef5b-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="cef5b-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cef5b-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="cef5b-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cef5b-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cef5b-119">Schema name</span></span>  <br/> |<span data-ttu-id="cef5b-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="cef5b-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cef5b-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cef5b-121">Validation file</span></span>  <br/> |<span data-ttu-id="cef5b-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cef5b-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cef5b-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="cef5b-123">Can be empty</span></span>  <br/> ||
   

