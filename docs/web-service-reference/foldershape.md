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
description: O elemento FolderShape identifica as propriedades da pasta a serem incluídas em uma resposta GetFolder, FindFolder ou SyncFolderHierarchy.
ms.openlocfilehash: f841fcc4570604c474387dfa24ec07c9d2784f62
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461342"
---
# <a name="foldershape"></a><span data-ttu-id="d0a9f-103">FolderShape</span><span class="sxs-lookup"><span data-stu-id="d0a9f-103">FolderShape</span></span>

<span data-ttu-id="d0a9f-104">O elemento **FolderShape** identifica as propriedades da pasta a serem incluídas em uma resposta [GetFolder](getfolder.md), [FindFolder](findfolder.md)ou [SyncFolderHierarchy](syncfolderhierarchy.md) .</span><span class="sxs-lookup"><span data-stu-id="d0a9f-104">The **FolderShape** element identifies the folder properties to include in a [GetFolder](getfolder.md), [FindFolder](findfolder.md), or [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span> 
  
```xml
<FolderShape>
   <BaseShape/>
   <AdditionalProperties/>
</FolderShape>
```

 <span data-ttu-id="d0a9f-105">**FolderResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="d0a9f-105">**FolderResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d0a9f-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d0a9f-106">Attributes and elements</span></span>

<span data-ttu-id="d0a9f-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d0a9f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d0a9f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d0a9f-108">Attributes</span></span>

<span data-ttu-id="d0a9f-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d0a9f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d0a9f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d0a9f-110">Child elements</span></span>

|<span data-ttu-id="d0a9f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d0a9f-111">**Element**</span></span>|<span data-ttu-id="d0a9f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d0a9f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0a9f-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="d0a9f-113">BaseShape</span></span>](baseshape.md) <br/> |<span data-ttu-id="d0a9f-114">Identifica a configuração básica das propriedades a serem retornadas em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="d0a9f-114">Identifies the basic configuration of properties to return in a response.</span></span>  <br/> |
|[<span data-ttu-id="d0a9f-115">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="d0a9f-115">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="d0a9f-116">Identifica propriedades adicionais a serem retornadas em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="d0a9f-116">Identifies additional properties to return in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d0a9f-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d0a9f-117">Parent elements</span></span>

|<span data-ttu-id="d0a9f-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d0a9f-118">**Element**</span></span>|<span data-ttu-id="d0a9f-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d0a9f-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0a9f-120">FindFolder</span><span class="sxs-lookup"><span data-stu-id="d0a9f-120">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="d0a9f-121">Define uma solicitação para identificar pastas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d0a9f-121">Defines a request to identify folders in a mailbox.</span></span>  <br/> <span data-ttu-id="d0a9f-122">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="d0a9f-122">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
|[<span data-ttu-id="d0a9f-123">GetFolder</span><span class="sxs-lookup"><span data-stu-id="d0a9f-123">GetFolder</span></span>](getfolder.md) <br/> |<span data-ttu-id="d0a9f-124">Define uma solicitação para obter uma pasta do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0a9f-124">Defines a request to get a folder from the Exchange store.</span></span>  <br/> <span data-ttu-id="d0a9f-125">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="d0a9f-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetFolder` <br/> |
|[<span data-ttu-id="d0a9f-126">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="d0a9f-126">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="d0a9f-127">Define uma solicitação para sincronizar uma hierarquia de pastas em um cliente.</span><span class="sxs-lookup"><span data-stu-id="d0a9f-127">Defines a request to synchronize a folder hierarchy on a client.</span></span>  <br/> <span data-ttu-id="d0a9f-128">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="d0a9f-128">The following is the XPath expression to this element:</span></span>  <br/>  `/SyncFolderHierarchy` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d0a9f-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="d0a9f-129">Remarks</span></span>

<span data-ttu-id="d0a9f-130">O elemento **FolderShape** é um elemento filho obrigatório do elemento [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="d0a9f-130">The **FolderShape** element is a required child element of the [FindFolder](findfolder.md) element.</span></span> 
  
<span data-ttu-id="d0a9f-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="d0a9f-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="d0a9f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0a9f-132">Example</span></span>

<span data-ttu-id="d0a9f-133">O exemplo a seguir de uma solicitação demonstra como localizar todas as pastas localizadas no primeiro nível da pasta caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="d0a9f-133">The following example of a request demonstrates how to find all folders located in the first level of the Inbox folder.</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="element-information"></a><span data-ttu-id="d0a9f-134">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d0a9f-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d0a9f-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="d0a9f-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d0a9f-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d0a9f-136">Schema Name</span></span>  <br/> |<span data-ttu-id="d0a9f-137">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d0a9f-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d0a9f-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d0a9f-138">Validation File</span></span>  <br/> |<span data-ttu-id="d0a9f-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d0a9f-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d0a9f-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d0a9f-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="d0a9f-141">False</span><span class="sxs-lookup"><span data-stu-id="d0a9f-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d0a9f-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="d0a9f-142">See also</span></span>



[<span data-ttu-id="d0a9f-143">FindFolder</span><span class="sxs-lookup"><span data-stu-id="d0a9f-143">FindFolder</span></span>](findfolder.md)

