---
title: AdditionalProperties
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AdditionalProperties
api_type:
- schema
ms.assetid: 7a269aed-dcfd-4c3e-9e14-094e53828101
description: O elemento AdditionalProperties identifica propriedades adicionais para uso em solicitações GetItem, UpdateItem, CreateItem, FindItem ou FindFolder.
ms.openlocfilehash: 90a307ba4d5ece10e15d2cec56cf5042c3d38685
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455811"
---
# <a name="additionalproperties"></a><span data-ttu-id="41a05-103">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="41a05-103">AdditionalProperties</span></span>

<span data-ttu-id="41a05-104">O **elemento AdditionalProperties** identifica propriedades adicionais para uso em solicitações [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md)ou [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="41a05-104">The **AdditionalProperties** element identifies additional properties for use in [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md), or [FindFolder](findfolder.md) requests.</span></span> 
  
```xml
<AdditionalProperties>
   <ExtendedFieldURI/>
   <FieldURI/>
   <IndexedFieldURI/>
</AdditionalProperties>
```

 <span data-ttu-id="41a05-105">**NonEmptyArrayOfPathsToElementType**</span><span class="sxs-lookup"><span data-stu-id="41a05-105">**NonEmptyArrayOfPathsToElementType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="41a05-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="41a05-106">Attributes and elements</span></span>

<span data-ttu-id="41a05-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="41a05-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="41a05-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="41a05-108">Attributes</span></span>

<span data-ttu-id="41a05-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="41a05-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="41a05-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="41a05-110">Child elements</span></span>

|<span data-ttu-id="41a05-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="41a05-111">**Element**</span></span>|<span data-ttu-id="41a05-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="41a05-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41a05-113">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="41a05-113">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="41a05-114">Identifica as propriedades de MAPI estendidas a serem obtidas, definidas ou criadas.</span><span class="sxs-lookup"><span data-stu-id="41a05-114">Identifies extended MAPI properties to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="41a05-115">FieldURI</span><span class="sxs-lookup"><span data-stu-id="41a05-115">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="41a05-116">Identifica as propriedades com frequência referenciadas por URI.</span><span class="sxs-lookup"><span data-stu-id="41a05-116">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="41a05-117">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="41a05-117">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="41a05-118">Identifica as propriedades de dicionário referenciadas frequentemente por URI.</span><span class="sxs-lookup"><span data-stu-id="41a05-118">Identifies frequently referenced dictionary properties by URI.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="41a05-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="41a05-119">Parent elements</span></span>

|<span data-ttu-id="41a05-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="41a05-120">**Element**</span></span>|<span data-ttu-id="41a05-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="41a05-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41a05-122">FolderShape</span><span class="sxs-lookup"><span data-stu-id="41a05-122">FolderShape</span></span>](foldershape.md) <br/> | <span data-ttu-id="41a05-123">Identifica as propriedades da pasta a serem incluídas em uma resposta [GetFolder](getfolder.md), [FindFolder](findfolder.md)ou [SyncFolderHierarchy](syncfolderhierarchy.md) .</span><span class="sxs-lookup"><span data-stu-id="41a05-123">Identifies the folder properties to include in a [GetFolder](getfolder.md), [FindFolder](findfolder.md), or [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span><br/><br/>  <span data-ttu-id="41a05-124">A seguir estão as expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="41a05-124">The following are the XPath expressions to this element:</span></span><br/><br/>  `/FindFolder/FolderShape` <br/>  `/GetFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[<span data-ttu-id="41a05-125">Shape</span><span class="sxs-lookup"><span data-stu-id="41a05-125">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="41a05-126">Identifica as propriedades e o conteúdo do item que serão incluídos em uma resposta [GetItem](getitem.md), [FindItem](finditem.md)ou [SyncFolderItems](syncfolderitems.md) .</span><span class="sxs-lookup"><span data-stu-id="41a05-126">Identifies the item properties and content to include in a [GetItem](getitem.md), [FindItem](finditem.md), or [SyncFolderItems](syncfolderitems.md) response.</span></span><br/><br/>  <span data-ttu-id="41a05-127">A seguir estão as expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="41a05-127">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
|[<span data-ttu-id="41a05-128">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="41a05-128">AttachmentShape</span></span>](attachmentshape.md) <br/> |<span data-ttu-id="41a05-129">Identifica Propriedades de item estendido adicionais para retornar em uma resposta a uma solicitação [GetItem](getitem.md) .</span><span class="sxs-lookup"><span data-stu-id="41a05-129">Identifies additional extended item properties to return in a response to a [GetItem](getitem.md) request.</span></span><br/><br/> <span data-ttu-id="41a05-130">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="41a05-130">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="41a05-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="41a05-131">Remarks</span></span>

<span data-ttu-id="41a05-132">Nem todos os elementos filho podem ser usados com solicitações [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md)ou [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="41a05-132">Not all the child elements can be used with [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md), or [FindFolder](findfolder.md) requests.</span></span> <span data-ttu-id="41a05-133">A propriedade deve ser aplicável à pasta ou ao item que é acessado.</span><span class="sxs-lookup"><span data-stu-id="41a05-133">The property must be applicable to the folder or item that is accessed.</span></span> <span data-ttu-id="41a05-134">Use propriedades estendidas para acessar outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="41a05-134">Use extended properties to access other properties.</span></span> <span data-ttu-id="41a05-135">Se a propriedade não existir para um determinado item, nenhum elemento correspondente será emitido no XML resultante.</span><span class="sxs-lookup"><span data-stu-id="41a05-135">If the property does not exist for a given item, no corresponding element will be emitted into the resulting XML.</span></span> 
  
<span data-ttu-id="41a05-136">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="41a05-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="41a05-137">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="41a05-137">This element is optional.</span></span>
  
## <a name="example"></a><span data-ttu-id="41a05-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41a05-138">Example</span></span>

<span data-ttu-id="41a05-139">O exemplo de solicitação a seguir mostra como obter um assunto de item usando o elemento **adicionalproperties** .</span><span class="sxs-lookup"><span data-stu-id="41a05-139">The following request example shows how to get an item subject by using the **AdditionalProperties** element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="ASkAS="/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="41a05-140">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="41a05-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="41a05-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="41a05-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="41a05-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="41a05-142">Schema Name</span></span>  <br/> |<span data-ttu-id="41a05-143">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="41a05-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="41a05-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="41a05-144">Validation File</span></span>  <br/> |<span data-ttu-id="41a05-145">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="41a05-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="41a05-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="41a05-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="41a05-147">Falso</span><span class="sxs-lookup"><span data-stu-id="41a05-147">False</span></span>  <br/> |
   

