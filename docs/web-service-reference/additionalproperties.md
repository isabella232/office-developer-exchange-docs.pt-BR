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
description: O elemento AdditionalProperties identifica propriedades adicionais para uso em GetItem, UpdateItem, CreateItem, FindItem ou FindFolder solicitações.
ms.openlocfilehash: 64e4f1ee6b24cf8015b7893dc4a904ca8b32d58e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751056"
---
# <a name="additionalproperties"></a><span data-ttu-id="d6b1b-103">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="d6b1b-103">AdditionalProperties</span></span>

<span data-ttu-id="d6b1b-104">O elemento **AdditionalProperties** identifica propriedades adicionais para uso em [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md)ou [FindFolder](findfolder.md) solicitações.</span><span class="sxs-lookup"><span data-stu-id="d6b1b-104">The **AdditionalProperties** element identifies additional properties for use in [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md), or [FindFolder](findfolder.md) requests.</span></span> 
  
```xml
<AdditionalProperties>
   <ExtendedFieldURI/>
   <FieldURI/>
   <IndexedFieldURI/>
</AdditionalProperties>
```

 <span data-ttu-id="d6b1b-105">**NonEmptyArrayOfPathsToElementType**</span><span class="sxs-lookup"><span data-stu-id="d6b1b-105">**NonEmptyArrayOfPathsToElementType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d6b1b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d6b1b-106">Attributes and elements</span></span>

<span data-ttu-id="d6b1b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d6b1b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d6b1b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d6b1b-108">Attributes</span></span>

<span data-ttu-id="d6b1b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d6b1b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d6b1b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d6b1b-110">Child elements</span></span>

|<span data-ttu-id="d6b1b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d6b1b-111">**Element**</span></span>|<span data-ttu-id="d6b1b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d6b1b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6b1b-113">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="d6b1b-113">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="d6b1b-114">Identifica as propriedades estendidas de MAPI para obter, definir ou criar.</span><span class="sxs-lookup"><span data-stu-id="d6b1b-114">Identifies extended MAPI properties to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="d6b1b-115">FieldURI</span><span class="sxs-lookup"><span data-stu-id="d6b1b-115">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="d6b1b-116">Identifica as propriedades frequentemente referenciadas pelo URI.</span><span class="sxs-lookup"><span data-stu-id="d6b1b-116">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="d6b1b-117">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="d6b1b-117">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="d6b1b-118">Identifica as propriedades de dicionário frequentemente referenciado pelo URI.</span><span class="sxs-lookup"><span data-stu-id="d6b1b-118">Identifies frequently referenced dictionary properties by URI.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d6b1b-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d6b1b-119">Parent elements</span></span>

|<span data-ttu-id="d6b1b-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d6b1b-120">**Element**</span></span>|<span data-ttu-id="d6b1b-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d6b1b-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6b1b-122">FolderShape</span><span class="sxs-lookup"><span data-stu-id="d6b1b-122">FolderShape</span></span>](foldershape.md) <br/> | <span data-ttu-id="d6b1b-123">Identifica as propriedades de pasta para incluir em uma resposta [GetFolder](getfolder.md), [FindFolder](findfolder.md)ou [SyncFolderHierarchy](syncfolderhierarchy.md) .</span><span class="sxs-lookup"><span data-stu-id="d6b1b-123">Identifies the folder properties to include in a [GetFolder](getfolder.md), [FindFolder](findfolder.md), or [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span><br/><br/>  <span data-ttu-id="d6b1b-124">A seguir estão as expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="d6b1b-124">The following are the XPath expressions to this element:</span></span><br/><br/>  `/FindFolder/FolderShape` <br/>  `/GetFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[<span data-ttu-id="d6b1b-125">ItemShape</span><span class="sxs-lookup"><span data-stu-id="d6b1b-125">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="d6b1b-126">Identifica as propriedades do item e o conteúdo a ser incluído em uma resposta [GetItem](getitem.md), [FindItem](finditem.md)ou [SyncFolderItems](syncfolderitems.md) .</span><span class="sxs-lookup"><span data-stu-id="d6b1b-126">Identifies the item properties and content to include in a [GetItem](getitem.md), [FindItem](finditem.md), or [SyncFolderItems](syncfolderitems.md) response.</span></span><br/><br/>  <span data-ttu-id="d6b1b-127">A seguir estão as expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="d6b1b-127">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
|[<span data-ttu-id="d6b1b-128">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="d6b1b-128">AttachmentShape</span></span>](attachmentshape.md) <br/> |<span data-ttu-id="d6b1b-129">Identifica as propriedades de item estendido adicional para retornar em resposta a uma solicitação de [GetItem](getitem.md) .</span><span class="sxs-lookup"><span data-stu-id="d6b1b-129">Identifies additional extended item properties to return in a response to a [GetItem](getitem.md) request.</span></span><br/><br/> <span data-ttu-id="d6b1b-130">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="d6b1b-130">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d6b1b-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="d6b1b-131">Remarks</span></span>

<span data-ttu-id="d6b1b-132">Não todos os elementos filhos podem ser usados com [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md)ou solicitações [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="d6b1b-132">Not all the child elements can be used with [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md), or [FindFolder](findfolder.md) requests.</span></span> <span data-ttu-id="d6b1b-133">A propriedade deve ser aplica à pasta ou item é acessado.</span><span class="sxs-lookup"><span data-stu-id="d6b1b-133">The property must be applicable to the folder or item that is accessed.</span></span> <span data-ttu-id="d6b1b-134">Use propriedades estendidas para acessar outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="d6b1b-134">Use extended properties to access other properties.</span></span> <span data-ttu-id="d6b1b-135">Se a propriedade não existe para um determinado item, nenhum elemento correspondente será emitido para o XML resultante.</span><span class="sxs-lookup"><span data-stu-id="d6b1b-135">If the property does not exist for a given item, no corresponding element will be emitted into the resulting XML.</span></span> 
  
<span data-ttu-id="d6b1b-136">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="d6b1b-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="d6b1b-137">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="d6b1b-137">This element is optional.</span></span>
  
## <a name="example"></a><span data-ttu-id="d6b1b-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6b1b-138">Example</span></span>

<span data-ttu-id="d6b1b-139">O exemplo de solicitação a seguir mostra como obter um assunto do item usando o elemento **AdditionalProperties** .</span><span class="sxs-lookup"><span data-stu-id="d6b1b-139">The following request example shows how to get an item subject by using the **AdditionalProperties** element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="d6b1b-140">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d6b1b-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d6b1b-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="d6b1b-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d6b1b-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d6b1b-142">Schema Name</span></span>  <br/> |<span data-ttu-id="d6b1b-143">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d6b1b-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="d6b1b-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d6b1b-144">Validation File</span></span>  <br/> |<span data-ttu-id="d6b1b-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d6b1b-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d6b1b-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d6b1b-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="d6b1b-147">False</span><span class="sxs-lookup"><span data-stu-id="d6b1b-147">False</span></span>  <br/> |
   

