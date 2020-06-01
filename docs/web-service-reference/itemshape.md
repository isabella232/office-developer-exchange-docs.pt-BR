---
title: Shape
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemShape
api_type:
- schema
ms.assetid: c5604161-bbc0-40bc-ad75-ff7e837d745f
description: O elemento doshape identifica um conjunto de propriedades para retornar em uma operação GetItem, FindItem ou uma resposta de operação SyncFolderItems.
ms.openlocfilehash: ffb666ee331b55a4f04cad076c705e4bec980e03
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458121"
---
# <a name="itemshape"></a><span data-ttu-id="f7de6-103">Shape</span><span class="sxs-lookup"><span data-stu-id="f7de6-103">ItemShape</span></span>

<span data-ttu-id="f7de6-104">O elemento **doshape** identifica um conjunto de propriedades para retornar em uma [operação GetItem](getitem-operation.md), [FindItem](finditem-operation.md)ou uma resposta de [operação SyncFolderItems](syncfolderitems-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f7de6-104">The **ItemShape** element identifies a set of properties to return in a [GetItem operation](getitem-operation.md), [FindItem operation](finditem-operation.md), or [SyncFolderItems operation](syncfolderitems-operation.md) response.</span></span> 
  
```XML
<ItemShape>
   <BaseShape/>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <ConvertHtmlCodePageToUTF8/>
   <AdditionalProperties/>
</ItemShape>
```

 <span data-ttu-id="f7de6-105">**ItemResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="f7de6-105">**ItemResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f7de6-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f7de6-106">Attributes and elements</span></span>

<span data-ttu-id="f7de6-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f7de6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7de6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f7de6-108">Attributes</span></span>

<span data-ttu-id="f7de6-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f7de6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f7de6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f7de6-110">Child elements</span></span>

|<span data-ttu-id="f7de6-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f7de6-111">**Element**</span></span>|<span data-ttu-id="f7de6-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f7de6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7de6-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="f7de6-113">BaseShape</span></span>](baseshape.md) <br/> |<span data-ttu-id="f7de6-114">Identifica a configuração básica de propriedades a serem retornadas em uma resposta de item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="f7de6-114">Identifies the basic configuration of properties to return in an item or folder response.</span></span>  <br/> |
|[<span data-ttu-id="f7de6-115">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="f7de6-115">IncludeMimeContent</span></span>](includemimecontent.md) <br/> |<span data-ttu-id="f7de6-116">Especifica se o conteúdo MIME (Multipurpose Internet Mail Extensions) de um item é retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="f7de6-116">Specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item is returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="f7de6-117">BodyType</span><span class="sxs-lookup"><span data-stu-id="f7de6-117">BodyType</span></span>](bodytype.md) <br/> |<span data-ttu-id="f7de6-118">Identifica como o corpo de texto é formatado na resposta.</span><span class="sxs-lookup"><span data-stu-id="f7de6-118">Identifies how the body text is formatted in the response.</span></span>  <br/> |
|[<span data-ttu-id="f7de6-119">ConvertHtmlCodePageToUTF8</span><span class="sxs-lookup"><span data-stu-id="f7de6-119">ConvertHtmlCodePageToUTF8</span></span>](converthtmlcodepagetoutf8.md) <br/> |<span data-ttu-id="f7de6-120">Indica se o corpo de HTML do item é convertido em UTF8.</span><span class="sxs-lookup"><span data-stu-id="f7de6-120">Indicates whether the item HTML body is converted to UTF8.</span></span>  <br/> |
|[<span data-ttu-id="f7de6-121">FilterHtmlContent</span><span class="sxs-lookup"><span data-stu-id="f7de6-121">FilterHtmlContent</span></span>](filterhtmlcontent.md) <br/> |<span data-ttu-id="f7de6-122">Especifica se a filtragem de conteúdo HTML está habilitada.</span><span class="sxs-lookup"><span data-stu-id="f7de6-122">Specifies whether HTML content filtering is enabled.</span></span>  <br/> |
|[<span data-ttu-id="f7de6-123">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="f7de6-123">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="f7de6-124">Identifica propriedades adicionais a serem retornadas em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="f7de6-124">Identifies additional properties to return in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f7de6-125">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f7de6-125">Parent elements</span></span>

|<span data-ttu-id="f7de6-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f7de6-126">**Element**</span></span>|<span data-ttu-id="f7de6-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f7de6-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7de6-128">GetItem</span><span class="sxs-lookup"><span data-stu-id="f7de6-128">GetItem</span></span>](getitem.md) <br/> |<span data-ttu-id="f7de6-129">Define uma solicitação para recuperar itens de uma caixa de correio no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7de6-129">Defines a request to retrieve items from a mailbox in the Exchange store.</span></span>  <br/> <span data-ttu-id="f7de6-130">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="f7de6-130">The following is the XPath expression to this element:</span></span>  <br/>  `/GetItem` <br/> |
|[<span data-ttu-id="f7de6-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="f7de6-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="f7de6-132">Define uma solicitação para localizar todos os itens contidos em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="f7de6-132">Defines a request to find all items that are contained in a folder.</span></span>  <br/> <span data-ttu-id="f7de6-133">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="f7de6-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
|[<span data-ttu-id="f7de6-134">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="f7de6-134">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="f7de6-135">Define uma solicitação para sincronizar itens em uma pasta do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7de6-135">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> <span data-ttu-id="f7de6-136">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="f7de6-136">The following is the XPath expression to this element:</span></span>  <br/>  `/SyncFolderItems` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f7de6-137">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="f7de6-137">Text value</span></span>

<span data-ttu-id="f7de6-138">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f7de6-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f7de6-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="f7de6-139">Remarks</span></span>

<span data-ttu-id="f7de6-140">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7de6-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f7de6-141">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f7de6-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7de6-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="f7de6-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f7de6-143">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f7de6-143">Schema Name</span></span>  <br/> |<span data-ttu-id="f7de6-144">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="f7de6-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f7de6-145">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f7de6-145">Validation File</span></span>  <br/> |<span data-ttu-id="f7de6-146">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f7de6-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f7de6-147">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f7de6-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="f7de6-148">False</span><span class="sxs-lookup"><span data-stu-id="f7de6-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f7de6-149">Confira também</span><span class="sxs-lookup"><span data-stu-id="f7de6-149">See also</span></span>



[<span data-ttu-id="f7de6-150">Operação GetItem</span><span class="sxs-lookup"><span data-stu-id="f7de6-150">GetItem operation</span></span>](getitem-operation.md)
  
[<span data-ttu-id="f7de6-151">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="f7de6-151">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="f7de6-152">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="f7de6-152">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="f7de6-153">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f7de6-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

