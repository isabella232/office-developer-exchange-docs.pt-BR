---
title: ItemShape
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
description: O elemento ItemShape identifica um conjunto de propriedades para retornar em uma operação de GetItem, operação FindItem ou resposta de operação SyncFolderItems.
ms.openlocfilehash: 95174a85a8fa05cb2612e1289d46c8db32b6e052
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824191"
---
# <a name="itemshape"></a><span data-ttu-id="b9f9b-103">ItemShape</span><span class="sxs-lookup"><span data-stu-id="b9f9b-103">ItemShape</span></span>

<span data-ttu-id="b9f9b-104">O elemento **ItemShape** identifica um conjunto de propriedades para retornar em uma resposta de [operação GetItem](getitem-operation.md), [operação FindItem](finditem-operation.md)ou [SyncFolderItems operação](syncfolderitems-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b9f9b-104">The **ItemShape** element identifies a set of properties to return in a [GetItem operation](getitem-operation.md), [FindItem operation](finditem-operation.md), or [SyncFolderItems operation](syncfolderitems-operation.md) response.</span></span> 
  
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

 <span data-ttu-id="b9f9b-105">**ItemResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="b9f9b-105">**ItemResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b9f9b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b9f9b-106">Attributes and elements</span></span>

<span data-ttu-id="b9f9b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b9f9b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b9f9b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b9f9b-108">Attributes</span></span>

<span data-ttu-id="b9f9b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b9f9b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b9f9b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b9f9b-110">Child elements</span></span>

|<span data-ttu-id="b9f9b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b9f9b-111">**Element**</span></span>|<span data-ttu-id="b9f9b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b9f9b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9f9b-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="b9f9b-113">BaseShape</span></span>](baseshape.md) <br/> |<span data-ttu-id="b9f9b-114">Identifica a configuração básica de propriedades para retornar em uma resposta de item ou uma pasta.</span><span class="sxs-lookup"><span data-stu-id="b9f9b-114">Identifies the basic configuration of properties to return in an item or folder response.</span></span>  <br/> |
|[<span data-ttu-id="b9f9b-115">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="b9f9b-115">IncludeMimeContent</span></span>](includemimecontent.md) <br/> |<span data-ttu-id="b9f9b-116">Especifica se o conteúdo de email extensões MIME (Multipurpose Internet) de um item é retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="b9f9b-116">Specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item is returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="b9f9b-117">BodyType</span><span class="sxs-lookup"><span data-stu-id="b9f9b-117">BodyType</span></span>](bodytype.md) <br/> |<span data-ttu-id="b9f9b-118">Identifica como o corpo de texto é formatado na resposta.</span><span class="sxs-lookup"><span data-stu-id="b9f9b-118">Identifies how the body text is formatted in the response.</span></span>  <br/> |
|[<span data-ttu-id="b9f9b-119">ConvertHtmlCodePageToUTF8</span><span class="sxs-lookup"><span data-stu-id="b9f9b-119">ConvertHtmlCodePageToUTF8</span></span>](converthtmlcodepagetoutf8.md) <br/> |<span data-ttu-id="b9f9b-120">Indica se o item do corpo em HTML é convertido em UTF8.</span><span class="sxs-lookup"><span data-stu-id="b9f9b-120">Indicates whether the item HTML body is converted to UTF8.</span></span>  <br/> |
|[<span data-ttu-id="b9f9b-121">FilterHtmlContent</span><span class="sxs-lookup"><span data-stu-id="b9f9b-121">FilterHtmlContent</span></span>](filterhtmlcontent.md) <br/> |<span data-ttu-id="b9f9b-122">Especifica se a filtragem de conteúdo de HTML está habilitado.</span><span class="sxs-lookup"><span data-stu-id="b9f9b-122">Specifies whether HTML content filtering is enabled.</span></span>  <br/> |
|[<span data-ttu-id="b9f9b-123">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="b9f9b-123">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="b9f9b-124">Identifica as propriedades adicionais para retornar em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="b9f9b-124">Identifies additional properties to return in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b9f9b-125">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b9f9b-125">Parent elements</span></span>

|<span data-ttu-id="b9f9b-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b9f9b-126">**Element**</span></span>|<span data-ttu-id="b9f9b-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b9f9b-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9f9b-128">GetItem</span><span class="sxs-lookup"><span data-stu-id="b9f9b-128">GetItem</span></span>](getitem.md) <br/> |<span data-ttu-id="b9f9b-129">Define uma solicitação para recuperar itens de uma caixa de correio no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b9f9b-129">Defines a request to retrieve items from a mailbox in the Exchange store.</span></span>  <br/> <span data-ttu-id="b9f9b-130">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="b9f9b-130">The following is the XPath expression to this element:</span></span>  <br/>  `/GetItem` <br/> |
|[<span data-ttu-id="b9f9b-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="b9f9b-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="b9f9b-132">Define uma solicitação para localizar todos os itens que estão contidos em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="b9f9b-132">Defines a request to find all items that are contained in a folder.</span></span>  <br/> <span data-ttu-id="b9f9b-133">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="b9f9b-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
|[<span data-ttu-id="b9f9b-134">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="b9f9b-134">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="b9f9b-135">Define uma solicitação para sincronizar os itens em uma pasta de repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b9f9b-135">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> <span data-ttu-id="b9f9b-136">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="b9f9b-136">The following is the XPath expression to this element:</span></span>  <br/>  `/SyncFolderItems` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b9f9b-137">Text value</span><span class="sxs-lookup"><span data-stu-id="b9f9b-137">Text value</span></span>

<span data-ttu-id="b9f9b-138">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b9f9b-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b9f9b-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="b9f9b-139">Remarks</span></span>

<span data-ttu-id="b9f9b-140">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b9f9b-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b9f9b-141">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b9f9b-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b9f9b-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="b9f9b-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b9f9b-143">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b9f9b-143">Schema Name</span></span>  <br/> |<span data-ttu-id="b9f9b-144">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="b9f9b-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b9f9b-145">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b9f9b-145">Validation File</span></span>  <br/> |<span data-ttu-id="b9f9b-146">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b9f9b-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b9f9b-147">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b9f9b-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="b9f9b-148">False</span><span class="sxs-lookup"><span data-stu-id="b9f9b-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b9f9b-149">Ver também</span><span class="sxs-lookup"><span data-stu-id="b9f9b-149">See also</span></span>



[<span data-ttu-id="b9f9b-150">Operação GetItem</span><span class="sxs-lookup"><span data-stu-id="b9f9b-150">GetItem operation</span></span>](getitem-operation.md)
  
[<span data-ttu-id="b9f9b-151">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="b9f9b-151">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="b9f9b-152">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="b9f9b-152">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="b9f9b-153">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b9f9b-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

