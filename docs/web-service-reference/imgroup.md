---
title: Imgroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7b884e-ecf1-4e58-86ec-856b13a95f2b
description: O elemento imgroup representa um grupo de mensagens instantâneas.
ms.openlocfilehash: a0ff3fcb82e7f18837af5a6f5daa16e90043034d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460684"
---
# <a name="imgroup"></a><span data-ttu-id="42be1-103">Imgroup</span><span class="sxs-lookup"><span data-stu-id="42be1-103">ImGroup</span></span>

<span data-ttu-id="42be1-104">O elemento **imgroup** representa um grupo de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="42be1-104">The **ImGroup** element represents an instant messaging group.</span></span> 
  
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

 <span data-ttu-id="42be1-105">**Outgrouptype**</span><span class="sxs-lookup"><span data-stu-id="42be1-105">**ImGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="42be1-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="42be1-106">Attributes and elements</span></span>

<span data-ttu-id="42be1-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="42be1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="42be1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="42be1-108">Attributes</span></span>

<span data-ttu-id="42be1-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="42be1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="42be1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="42be1-110">Child elements</span></span>

<span data-ttu-id="42be1-111">[DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md)  |  [GroupType](grouptype.md)  |  [ExchangeStoreId](exchangestoreid.md)  |  [MemberCorrelationKey](membercorrelationkey.md)  |  [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)  |  [SmtpAddress](smtpaddress.md)</span><span class="sxs-lookup"><span data-stu-id="42be1-111">[DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md) | [GroupType](grouptype.md) | [ExchangeStoreId](exchangestoreid.md) | [MemberCorrelationKey](membercorrelationkey.md) | [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md) | [SmtpAddress](smtpaddress.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="42be1-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="42be1-112">Parent elements</span></span>

<span data-ttu-id="42be1-113">[Grupos (ArrayOfImGroupType)](groups-arrayofimgrouptype.md)  |  [AddDistributionGroupToImListResponse](adddistributiongrouptoimlistresponse.md)  |  [AddImGroupResponse](addimgroupresponse.md)</span><span class="sxs-lookup"><span data-stu-id="42be1-113">[Groups (ArrayOfImGroupType)](groups-arrayofimgrouptype.md) | [AddDistributionGroupToImListResponse](adddistributiongrouptoimlistresponse.md) | [AddImGroupResponse](addimgroupresponse.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="42be1-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="42be1-114">Remarks</span></span>

<span data-ttu-id="42be1-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="42be1-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="42be1-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="42be1-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="42be1-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="42be1-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="42be1-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="42be1-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="42be1-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="42be1-119">Schema name</span></span>  <br/> |<span data-ttu-id="42be1-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="42be1-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="42be1-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="42be1-121">Validation file</span></span>  <br/> |<span data-ttu-id="42be1-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="42be1-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="42be1-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="42be1-123">Can be empty</span></span>  <br/> ||
   

