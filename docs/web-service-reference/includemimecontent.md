---
title: IncludeMimeContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IncludeMimeContent
api_type:
- schema
ms.assetid: 3f3c2300-55cd-41c0-900e-b470b290d52f
description: O elemento IncludeMimeContent especifica se o conteúdo MIME (Multipurpose Internet Mail Extensions) de um item ou anexo é retornado na resposta.
ms.openlocfilehash: 6198e4bef2dc59e6e56a8d3cbe463dad13e544e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457190"
---
# <a name="includemimecontent"></a><span data-ttu-id="8d29c-103">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="8d29c-103">IncludeMimeContent</span></span>

<span data-ttu-id="8d29c-104">O elemento **IncludeMimeContent** especifica se o conteúdo MIME (Multipurpose Internet Mail Extensions) de um item ou anexo é retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="8d29c-104">The **IncludeMimeContent** element specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item or attachment is returned in the response.</span></span> 
  
```xml
<IncludeMimeContent>true or false</IncludeMimeContent>
```

 <span data-ttu-id="8d29c-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="8d29c-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8d29c-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8d29c-106">Attributes and elements</span></span>

<span data-ttu-id="8d29c-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8d29c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d29c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8d29c-108">Attributes</span></span>

<span data-ttu-id="8d29c-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8d29c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d29c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8d29c-110">Child elements</span></span>

<span data-ttu-id="8d29c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8d29c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8d29c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8d29c-112">Parent elements</span></span>

|<span data-ttu-id="8d29c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8d29c-113">**Element**</span></span>|<span data-ttu-id="8d29c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8d29c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d29c-115">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="8d29c-115">AttachmentShape</span></span>](attachmentshape.md) <br/> | <span data-ttu-id="8d29c-116">Identifica propriedades adicionais para retornar em uma resposta a uma solicitação [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="8d29c-116">Identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span>  <br/> <br/> <span data-ttu-id="8d29c-117">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="8d29c-117">The following is the XPath expression to this element:</span></span>  <br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
|[<span data-ttu-id="8d29c-118">Shape</span><span class="sxs-lookup"><span data-stu-id="8d29c-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="8d29c-119">Identifica as propriedades e o conteúdo do item que serão incluídos em uma resposta GetItem, FindItem ou SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="8d29c-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/> <br/> <span data-ttu-id="8d29c-120">A seguir estão as expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="8d29c-120">The following are the XPath expressions to this element:</span></span><br/>  <br/>  `/GetItem/ItemShape` <br/><br/>  `/FindItem/ItemShape` <br/><br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8d29c-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="8d29c-121">Text value</span></span>

<span data-ttu-id="8d29c-122">Esse elemento pode ser **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="8d29c-122">This element can be either **true** or **false**.</span></span> <span data-ttu-id="8d29c-123">O valor padrão é **false**.</span><span class="sxs-lookup"><span data-stu-id="8d29c-123">The default value is **false**.</span></span> <span data-ttu-id="8d29c-124">Este é um tipo de dados Boolean.</span><span class="sxs-lookup"><span data-stu-id="8d29c-124">This is a Boolean data type.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8d29c-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="8d29c-125">Remarks</span></span>

<span data-ttu-id="8d29c-126">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="8d29c-126">This element is optional.</span></span>
  
<span data-ttu-id="8d29c-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="8d29c-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="8d29c-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d29c-128">Example</span></span>

<span data-ttu-id="8d29c-129">O exemplo a seguir de uma solicitação demonstra como definir o elemento **IncludeMimeContent** .</span><span class="sxs-lookup"><span data-stu-id="8d29c-129">The following example of a request demonstrates a how to set the **IncludeMimeContent** element.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape>
        <t:IncludeMimeContent>true</t:IncludeMimeContent>
        <t:BodyType>Best</t:BodyType>
      </AttachmentShape>
      <AttachmentIds>
        <t:AttachmentId Id="ASkAS="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="8d29c-130">O atributo ID do anexo é truncado para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8d29c-130">The attachment Id attribute is truncated to preserve readability.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8d29c-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="8d29c-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8d29c-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="8d29c-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8d29c-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8d29c-133">Schema Name</span></span>  <br/> |<span data-ttu-id="8d29c-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8d29c-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="8d29c-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8d29c-135">Validation File</span></span>  <br/> |<span data-ttu-id="8d29c-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8d29c-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8d29c-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8d29c-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="8d29c-138">Falso</span><span class="sxs-lookup"><span data-stu-id="8d29c-138">False</span></span>  <br/> |
   

