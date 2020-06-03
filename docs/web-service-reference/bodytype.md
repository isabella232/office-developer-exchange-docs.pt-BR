---
title: BodyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BodyType
api_type:
- schema
ms.assetid: d42ec77b-fb9f-404a-9bf2-1801e8744676
description: O elemento BodyType identifica como o corpo de texto é formatado na resposta.
ms.openlocfilehash: 448d20ac54b09a2f4f6a273a1099519371ac7f5b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465944"
---
# <a name="bodytype"></a><span data-ttu-id="5bc75-103">BodyType</span><span class="sxs-lookup"><span data-stu-id="5bc75-103">BodyType</span></span>

<span data-ttu-id="5bc75-104">O elemento **BodyType** identifica como o corpo de texto é formatado na resposta.</span><span class="sxs-lookup"><span data-stu-id="5bc75-104">The **BodyType** element identifies how the body text is formatted in the response.</span></span> 
  
```xml
<BodyType>Best or HTML or Text</BodyType>
```

<span data-ttu-id="5bc75-105">**BodyTypeResponseType**</span><span class="sxs-lookup"><span data-stu-id="5bc75-105">**BodyTypeResponseType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5bc75-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5bc75-106">Attributes and elements</span></span>

<span data-ttu-id="5bc75-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5bc75-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5bc75-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5bc75-108">Attributes</span></span>

<span data-ttu-id="5bc75-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5bc75-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5bc75-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5bc75-110">Child elements</span></span>

<span data-ttu-id="5bc75-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5bc75-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5bc75-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5bc75-112">Parent elements</span></span>

|<span data-ttu-id="5bc75-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5bc75-113">**Element**</span></span>|<span data-ttu-id="5bc75-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5bc75-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5bc75-115">Shape</span><span class="sxs-lookup"><span data-stu-id="5bc75-115">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="5bc75-116">Identifica as propriedades e o conteúdo do item que serão incluídos em uma resposta GetItem, FindItem ou SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="5bc75-116">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/><br/><span data-ttu-id="5bc75-117">A seguir estão as expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="5bc75-117">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape`<br/><br/>`/FindItem/ItemShape`<br/><br/>`/SyncFolderItems/ItemShape` <br/> |
|[<span data-ttu-id="5bc75-118">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="5bc75-118">AttachmentShape</span></span>](attachmentshape.md) <br/> |<span data-ttu-id="5bc75-119">Identifica Propriedades de item estendido adicionais para retornar em uma resposta a uma solicitação [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="5bc75-119">Identifies additional extended item properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span>  <br/><br/><span data-ttu-id="5bc75-120">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="5bc75-120">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5bc75-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="5bc75-121">Text value</span></span>

<span data-ttu-id="5bc75-122">A tabela a seguir lista os valores possíveis para o elemento **BodyType** .</span><span class="sxs-lookup"><span data-stu-id="5bc75-122">The following table lists the possible values for the **BodyType** element.</span></span> 
  
|<span data-ttu-id="5bc75-123">**Valor**</span><span class="sxs-lookup"><span data-stu-id="5bc75-123">**Value**</span></span>|<span data-ttu-id="5bc75-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5bc75-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5bc75-125">Melhor</span><span class="sxs-lookup"><span data-stu-id="5bc75-125">Best</span></span>  <br/> |<span data-ttu-id="5bc75-126">A resposta retornará o conteúdo mais avançado disponível do corpo de texto.</span><span class="sxs-lookup"><span data-stu-id="5bc75-126">The response will return the richest available content of body text.</span></span> <span data-ttu-id="5bc75-127">Isso é útil se for desconhecido se o conteúdo for texto ou HTML.</span><span class="sxs-lookup"><span data-stu-id="5bc75-127">This is useful if it is unknown whether the content is text or HTML.</span></span><br/><br/> <span data-ttu-id="5bc75-128">O corpo retornado será texto se o corpo armazenado for texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="5bc75-128">The returned body will be text if the stored body is plain text.</span></span> <span data-ttu-id="5bc75-129">Caso contrário, a resposta retornará HTML se o corpo armazenado estiver em formato HTML ou RTF.</span><span class="sxs-lookup"><span data-stu-id="5bc75-129">Otherwise, the response will return HTML if the stored body is in either HTML or RTF format.</span></span><br/><br/> <span data-ttu-id="5bc75-130">Esse é o valor padrão.</span><span class="sxs-lookup"><span data-stu-id="5bc75-130">This is the default value.</span></span>  <br/> |
|<span data-ttu-id="5bc75-131">HTML</span><span class="sxs-lookup"><span data-stu-id="5bc75-131">HTML</span></span>  <br/> |<span data-ttu-id="5bc75-132">A resposta retornará um corpo de item como HTML.</span><span class="sxs-lookup"><span data-stu-id="5bc75-132">The response will return an item body as HTML.</span></span>  <br/> |
|<span data-ttu-id="5bc75-133">Texto</span><span class="sxs-lookup"><span data-stu-id="5bc75-133">Text</span></span>  <br/> |<span data-ttu-id="5bc75-134">A resposta retornará um corpo de item como texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="5bc75-134">The response will return an item body as plain text.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5bc75-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="5bc75-135">Remarks</span></span>

<span data-ttu-id="5bc75-136">Você pode identificar o tipo de corpo retornado na resposta verificando o atributo **BodyType** do elemento [Body](body.md) .</span><span class="sxs-lookup"><span data-stu-id="5bc75-136">You can identify the type of body returned in the response by checking the **BodyType** attribute of the [Body](body.md) element.</span></span> <span data-ttu-id="5bc75-137">O atributo **BodyType** identificará o corpo como HTML ou texto.</span><span class="sxs-lookup"><span data-stu-id="5bc75-137">The **BodyType** attribute will identify the body as either HTML or text.</span></span> 
  
<span data-ttu-id="5bc75-138">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="5bc75-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="5bc75-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5bc75-139">Example</span></span>

<span data-ttu-id="5bc75-140">O exemplo a seguir de uma solicitação mostra onde um elemento **BodyType** é usado.</span><span class="sxs-lookup"><span data-stu-id="5bc75-140">The following example of a request shows where a **BodyType** element is used.</span></span> 
  
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
        <t:BodyType>Best</t:BodyType>
      </AttachmentShape>
      <AttachmentIds>
        <t:AttachmentId Id="ASkAS="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="5bc75-141">O atributo ID foi reduzido para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5bc75-141">The Id attribute has been shortened to preserve readability.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5bc75-142">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5bc75-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5bc75-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="5bc75-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5bc75-144">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5bc75-144">Schema Name</span></span>  <br/> |<span data-ttu-id="5bc75-145">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5bc75-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="5bc75-146">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5bc75-146">Validation File</span></span>  <br/> |<span data-ttu-id="5bc75-147">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5bc75-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5bc75-148">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5bc75-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="5bc75-149">Falso</span><span class="sxs-lookup"><span data-stu-id="5bc75-149">False</span></span>  <br/> |
   

