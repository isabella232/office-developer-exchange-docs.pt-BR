---
title: AddressListId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a3334bb2-90dc-4fe1-96d9-890b13d9ff30
description: O elemento AddressListId Especifica o identificador de uma lista de endereços.
ms.openlocfilehash: d8a513559b7d127559537b43d7c6c0a4db121702
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751069"
---
# <a name="addresslistid"></a><span data-ttu-id="4442b-103">AddressListId</span><span class="sxs-lookup"><span data-stu-id="4442b-103">AddressListId</span></span>

<span data-ttu-id="4442b-104">O elemento **AddressListId** Especifica o identificador de uma lista de endereços.</span><span class="sxs-lookup"><span data-stu-id="4442b-104">The **AddressListId** element specifies the identifier of an address list.</span></span> 
  
```XML
<AddressListId Id="">
</AddressListId>
```

 <span data-ttu-id="4442b-105">**AddressListIdType**</span><span class="sxs-lookup"><span data-stu-id="4442b-105">**AddressListIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4442b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4442b-106">Attributes and elements</span></span>

<span data-ttu-id="4442b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4442b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4442b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4442b-108">Attributes</span></span>

|<span data-ttu-id="4442b-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="4442b-109">**Attribute**</span></span>|<span data-ttu-id="4442b-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4442b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4442b-111">**ID de**</span><span class="sxs-lookup"><span data-stu-id="4442b-111">**Id**</span></span> <br/> |<span data-ttu-id="4442b-112">Um identificador de lista de endereços de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="4442b-112">A string address list identifier.</span></span> <span data-ttu-id="4442b-113">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="4442b-113">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4442b-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4442b-114">Child elements</span></span>

<span data-ttu-id="4442b-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4442b-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4442b-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4442b-116">Parent elements</span></span>

|<span data-ttu-id="4442b-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4442b-117">**Element**</span></span>|<span data-ttu-id="4442b-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4442b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4442b-119">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="4442b-119">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="4442b-120">Indica a pasta que está programada para ações que usam pastas.</span><span class="sxs-lookup"><span data-stu-id="4442b-120">Indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="4442b-121">Este elemento deve estar presente quando copiar, excluir, mover e definindo o estado lido em itens da conversa em uma pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="4442b-121">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span>  <br/> |
|[<span data-ttu-id="4442b-122">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="4442b-122">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="4442b-123">Especifica o identificador da pasta para o qual os itens de email são copiados.</span><span class="sxs-lookup"><span data-stu-id="4442b-123">Specifies the identifier of the folder to which email items are copied.</span></span>  <br/> |
|[<span data-ttu-id="4442b-124">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="4442b-124">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="4442b-125">Indica a pasta de destino para cópia e mover ações.</span><span class="sxs-lookup"><span data-stu-id="4442b-125">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="4442b-126">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="4442b-126">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="4442b-127">Especifica o identificador da pasta para o qual os itens de email são movidos</span><span class="sxs-lookup"><span data-stu-id="4442b-127">Specifies the identifier of the folder to which email items are moved</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4442b-128">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="4442b-128">Remarks</span></span>

<span data-ttu-id="4442b-129">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4442b-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4442b-130">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4442b-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4442b-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4442b-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4442b-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="4442b-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4442b-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4442b-133">Schema Name</span></span>  <br/> |<span data-ttu-id="4442b-134">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="4442b-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="4442b-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4442b-135">Validation File</span></span>  <br/> |<span data-ttu-id="4442b-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4442b-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4442b-137">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="4442b-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4442b-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="4442b-138">See also</span></span>

- [<span data-ttu-id="4442b-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4442b-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

