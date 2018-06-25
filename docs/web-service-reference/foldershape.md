---
title: FolderShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderShape
api_type:
- schema
ms.assetid: 244f4f46-a33d-4764-92e3-1bddb4dc6a49
description: O elemento FolderShape identifica as propriedades da pasta para incluir em uma resposta GetFolder, FindFolder ou SyncFolderHierarchy.
ms.openlocfilehash: 8ebdd70ef13ee9f0cce9020b9212576cba782be4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752350"
---
# <a name="foldershape"></a><span data-ttu-id="3db5a-103">FolderShape</span><span class="sxs-lookup"><span data-stu-id="3db5a-103">FolderShape</span></span>

<span data-ttu-id="3db5a-104">O elemento **FolderShape** identifica as propriedades da pasta para incluir em uma resposta [GetFolder](getfolder.md), [FindFolder](findfolder.md)ou [SyncFolderHierarchy](syncfolderhierarchy.md) .</span><span class="sxs-lookup"><span data-stu-id="3db5a-104">The **FolderShape** element identifies the folder properties to include in a [GetFolder](getfolder.md), [FindFolder](findfolder.md), or [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span> 
  
```xml
<FolderShape>
   <BaseShape/>
   <AdditionalProperties/>
</FolderShape>
```

 <span data-ttu-id="3db5a-105">**FolderResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="3db5a-105">**FolderResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3db5a-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3db5a-106">Attributes and elements</span></span>

<span data-ttu-id="3db5a-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3db5a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3db5a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3db5a-108">Attributes</span></span>

<span data-ttu-id="3db5a-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3db5a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3db5a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3db5a-110">Child elements</span></span>

|<span data-ttu-id="3db5a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3db5a-111">**Element**</span></span>|<span data-ttu-id="3db5a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3db5a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3db5a-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="3db5a-113">BaseShape</span></span>](baseshape.md) <br/> |<span data-ttu-id="3db5a-114">Identifica a configuração básica de propriedades para retornar em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="3db5a-114">Identifies the basic configuration of properties to return in a response.</span></span>  <br/> |
|[<span data-ttu-id="3db5a-115">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="3db5a-115">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="3db5a-116">Identifica as propriedades adicionais para retornar em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="3db5a-116">Identifies additional properties to return in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3db5a-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3db5a-117">Parent elements</span></span>

|<span data-ttu-id="3db5a-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3db5a-118">**Element**</span></span>|<span data-ttu-id="3db5a-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3db5a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3db5a-120">FindFolder</span><span class="sxs-lookup"><span data-stu-id="3db5a-120">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="3db5a-121">Define uma solicitação para identificar pastas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="3db5a-121">Defines a request to identify folders in a mailbox.</span></span>  <br/> <span data-ttu-id="3db5a-122">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="3db5a-122">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
|[<span data-ttu-id="3db5a-123">GetFolder</span><span class="sxs-lookup"><span data-stu-id="3db5a-123">GetFolder</span></span>](getfolder.md) <br/> |<span data-ttu-id="3db5a-124">Define uma solicitação para obter uma pasta do Exchange store.</span><span class="sxs-lookup"><span data-stu-id="3db5a-124">Defines a request to get a folder from the Exchange store.</span></span>  <br/> <span data-ttu-id="3db5a-125">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="3db5a-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetFolder` <br/> |
|[<span data-ttu-id="3db5a-126">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="3db5a-126">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="3db5a-127">Define uma solicitação para sincronizar uma hierarquia de pastas em um cliente.</span><span class="sxs-lookup"><span data-stu-id="3db5a-127">Defines a request to synchronize a folder hierarchy on a client.</span></span>  <br/> <span data-ttu-id="3db5a-128">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="3db5a-128">The following is the XPath expression to this element:</span></span>  <br/>  `/SyncFolderHierarchy` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3db5a-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="3db5a-129">Remarks</span></span>

<span data-ttu-id="3db5a-130">O **FolderShape** é um elemento necessário filho do elemento [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="3db5a-130">The **FolderShape** element is a required child element of the [FindFolder](findfolder.md) element.</span></span> 
  
<span data-ttu-id="3db5a-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="3db5a-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="3db5a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3db5a-132">Example</span></span>

<span data-ttu-id="3db5a-133">O exemplo a seguir de uma solicitação demonstra como localizar todas as pastas localizadas no primeiro nível da pasta caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="3db5a-133">The following example of a request demonstrates how to find all folders located in the first level of the Inbox folder.</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="3db5a-134">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3db5a-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3db5a-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="3db5a-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3db5a-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3db5a-136">Schema Name</span></span>  <br/> |<span data-ttu-id="3db5a-137">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="3db5a-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3db5a-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3db5a-138">Validation File</span></span>  <br/> |<span data-ttu-id="3db5a-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3db5a-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3db5a-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3db5a-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="3db5a-141">False</span><span class="sxs-lookup"><span data-stu-id="3db5a-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3db5a-142">Ver também</span><span class="sxs-lookup"><span data-stu-id="3db5a-142">See also</span></span>



[<span data-ttu-id="3db5a-143">FindFolder</span><span class="sxs-lookup"><span data-stu-id="3db5a-143">FindFolder</span></span>](findfolder.md)

