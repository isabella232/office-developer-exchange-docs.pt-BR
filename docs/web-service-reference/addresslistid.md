---
title: AddressListid
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a3334bb2-90dc-4fe1-96d9-890b13d9ff30
description: O elemento AddressListid especifica o identificador de uma lista de endereços.
ms.openlocfilehash: c33944bf6e41903a5de596628e1ce7ba9f7421e1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463605"
---
# <a name="addresslistid"></a><span data-ttu-id="3984e-103">AddressListid</span><span class="sxs-lookup"><span data-stu-id="3984e-103">AddressListId</span></span>

<span data-ttu-id="3984e-104">O elemento **addresslistid** especifica o identificador de uma lista de endereços.</span><span class="sxs-lookup"><span data-stu-id="3984e-104">The **AddressListId** element specifies the identifier of an address list.</span></span> 
  
```XML
<AddressListId Id="">
</AddressListId>
```

 <span data-ttu-id="3984e-105">**AddressListIdType**</span><span class="sxs-lookup"><span data-stu-id="3984e-105">**AddressListIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3984e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3984e-106">Attributes and elements</span></span>

<span data-ttu-id="3984e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3984e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3984e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3984e-108">Attributes</span></span>

|<span data-ttu-id="3984e-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="3984e-109">**Attribute**</span></span>|<span data-ttu-id="3984e-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3984e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3984e-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="3984e-111">**Id**</span></span> <br/> |<span data-ttu-id="3984e-112">Um identificador de lista de endereços de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="3984e-112">A string address list identifier.</span></span> <span data-ttu-id="3984e-113">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="3984e-113">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3984e-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3984e-114">Child elements</span></span>

<span data-ttu-id="3984e-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3984e-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3984e-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3984e-116">Parent elements</span></span>

|<span data-ttu-id="3984e-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3984e-117">**Element**</span></span>|<span data-ttu-id="3984e-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3984e-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3984e-119">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="3984e-119">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="3984e-120">Indica a pasta que é direcionada para ações que usam pastas.</span><span class="sxs-lookup"><span data-stu-id="3984e-120">Indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="3984e-121">Esse elemento deve estar presente ao copiar, excluir, mover e definir o estado de leitura em itens de conversa em uma pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="3984e-121">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span>  <br/> |
|[<span data-ttu-id="3984e-122">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="3984e-122">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="3984e-123">Especifica o identificador da pasta para a qual os itens de email são copiados.</span><span class="sxs-lookup"><span data-stu-id="3984e-123">Specifies the identifier of the folder to which email items are copied.</span></span>  <br/> |
|[<span data-ttu-id="3984e-124">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="3984e-124">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="3984e-125">Indica a pasta de destino para ações de copiar e mover.</span><span class="sxs-lookup"><span data-stu-id="3984e-125">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="3984e-126">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="3984e-126">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="3984e-127">Especifica o identificador da pasta para a qual os itens de email são movidos</span><span class="sxs-lookup"><span data-stu-id="3984e-127">Specifies the identifier of the folder to which email items are moved</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3984e-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="3984e-128">Remarks</span></span>

<span data-ttu-id="3984e-129">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3984e-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3984e-130">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3984e-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3984e-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3984e-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3984e-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="3984e-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3984e-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3984e-133">Schema Name</span></span>  <br/> |<span data-ttu-id="3984e-134">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="3984e-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="3984e-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3984e-135">Validation File</span></span>  <br/> |<span data-ttu-id="3984e-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3984e-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="3984e-137">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="3984e-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="3984e-138">Também consulte</span><span class="sxs-lookup"><span data-stu-id="3984e-138">See also</span></span>

- [<span data-ttu-id="3984e-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3984e-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

