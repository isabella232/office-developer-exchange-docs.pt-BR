---
title: AddressEntity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ead22eab-f1e7-48b4-a165-db0e49fe86a8
description: O elemento AddressEntity especifica uma única entidade de endereço.
ms.openlocfilehash: c597557fe02a9c0ff7ed3c9862e1662cfbae596a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466903"
---
# <a name="addressentity"></a><span data-ttu-id="c3e18-103">AddressEntity</span><span class="sxs-lookup"><span data-stu-id="c3e18-103">AddressEntity</span></span>

<span data-ttu-id="c3e18-104">O elemento **AddressEntity** especifica uma única entidade de endereço.</span><span class="sxs-lookup"><span data-stu-id="c3e18-104">The **AddressEntity** element specifies a single address entity.</span></span> 
  
```XML
<AddressEntity>
    <Address></Address>
    <Position></Position>
</AddressEntity>
```

 <span data-ttu-id="c3e18-105">**AddressEntityType**</span><span class="sxs-lookup"><span data-stu-id="c3e18-105">**AddressEntityType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c3e18-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c3e18-106">Attributes and elements</span></span>

<span data-ttu-id="c3e18-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c3e18-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c3e18-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c3e18-108">Attributes</span></span>

<span data-ttu-id="c3e18-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c3e18-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c3e18-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c3e18-110">Child elements</span></span>

|<span data-ttu-id="c3e18-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c3e18-111">**Element**</span></span>|<span data-ttu-id="c3e18-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c3e18-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c3e18-113">Endereço (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="c3e18-113">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="c3e18-114">Especifica um endereço.</span><span class="sxs-lookup"><span data-stu-id="c3e18-114">Specifies an address.</span></span>  <br/> |
|[<span data-ttu-id="c3e18-115">Posição</span><span class="sxs-lookup"><span data-stu-id="c3e18-115">Position</span></span>](position.md) <br/> |<span data-ttu-id="c3e18-116">Especifica a posição em uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="c3e18-116">Specifies the position in an email message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c3e18-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c3e18-117">Parent elements</span></span>

|<span data-ttu-id="c3e18-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c3e18-118">**Element**</span></span>|<span data-ttu-id="c3e18-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c3e18-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c3e18-120">Endereços (ArrayOfAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="c3e18-120">Addresses (ArrayOfAddressEntitiesType)</span></span>](addresses-arrayofaddressentitiestype.md) <br/> |<span data-ttu-id="c3e18-121">Especifica uma matriz de elementos **AddressEntity** .</span><span class="sxs-lookup"><span data-stu-id="c3e18-121">Specifies an array of **AddressEntity** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c3e18-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c3e18-122">Text value</span></span>

<span data-ttu-id="c3e18-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c3e18-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c3e18-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="c3e18-124">Remarks</span></span>

<span data-ttu-id="c3e18-125">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c3e18-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c3e18-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c3e18-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c3e18-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c3e18-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c3e18-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="c3e18-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c3e18-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c3e18-129">Schema Name</span></span>  <br/> |<span data-ttu-id="c3e18-130">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="c3e18-130">Type schema</span></span>  <br/> |
|<span data-ttu-id="c3e18-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c3e18-131">Validation File</span></span>  <br/> |<span data-ttu-id="c3e18-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c3e18-132">types.xsd</span></span>  <br/> |
|<span data-ttu-id="c3e18-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="c3e18-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c3e18-134">Também consulte</span><span class="sxs-lookup"><span data-stu-id="c3e18-134">See also</span></span>

- [<span data-ttu-id="c3e18-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c3e18-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

