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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461342"
---
# <a name="foldershape"></a><span data-ttu-id="08ede-103">FolderShape</span><span class="sxs-lookup"><span data-stu-id="08ede-103">FolderShape</span></span>

<span data-ttu-id="08ede-104">O elemento **FolderShape** identifica as propriedades da pasta a serem incluídas em uma resposta [GetFolder](getfolder.md), [FindFolder](findfolder.md)ou [SyncFolderHierarchy](syncfolderhierarchy.md) .</span><span class="sxs-lookup"><span data-stu-id="08ede-104">The **FolderShape** element identifies the folder properties to include in a [GetFolder](getfolder.md), [FindFolder](findfolder.md), or [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span> 
  
```xml
<FolderShape>
   <BaseShape/>
   <AdditionalProperties/>
</FolderShape>
```

 <span data-ttu-id="08ede-105">**FolderResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="08ede-105">**FolderResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08ede-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="08ede-106">Attributes and elements</span></span>

<span data-ttu-id="08ede-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="08ede-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08ede-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="08ede-108">Attributes</span></span>

<span data-ttu-id="08ede-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="08ede-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08ede-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="08ede-110">Child elements</span></span>

|<span data-ttu-id="08ede-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="08ede-111">**Element**</span></span>|<span data-ttu-id="08ede-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="08ede-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08ede-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="08ede-113">BaseShape</span></span>](baseshape.md) <br/> |<span data-ttu-id="08ede-114">Identifica a configuração básica das propriedades a serem retornadas em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="08ede-114">Identifies the basic configuration of properties to return in a response.</span></span>  <br/> |
|[<span data-ttu-id="08ede-115">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="08ede-115">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="08ede-116">Identifica propriedades adicionais a serem retornadas em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="08ede-116">Identifies additional properties to return in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="08ede-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="08ede-117">Parent elements</span></span>

|<span data-ttu-id="08ede-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="08ede-118">**Element**</span></span>|<span data-ttu-id="08ede-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="08ede-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08ede-120">FindFolder</span><span class="sxs-lookup"><span data-stu-id="08ede-120">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="08ede-121">Define uma solicitação para identificar pastas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="08ede-121">Defines a request to identify folders in a mailbox.</span></span>  <br/> <span data-ttu-id="08ede-122">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="08ede-122">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
|[<span data-ttu-id="08ede-123">GetFolder</span><span class="sxs-lookup"><span data-stu-id="08ede-123">GetFolder</span></span>](getfolder.md) <br/> |<span data-ttu-id="08ede-124">Define uma solicitação para obter uma pasta do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="08ede-124">Defines a request to get a folder from the Exchange store.</span></span>  <br/> <span data-ttu-id="08ede-125">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="08ede-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetFolder` <br/> |
|[<span data-ttu-id="08ede-126">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="08ede-126">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="08ede-127">Define uma solicitação para sincronizar uma hierarquia de pastas em um cliente.</span><span class="sxs-lookup"><span data-stu-id="08ede-127">Defines a request to synchronize a folder hierarchy on a client.</span></span>  <br/> <span data-ttu-id="08ede-128">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="08ede-128">The following is the XPath expression to this element:</span></span>  <br/>  `/SyncFolderHierarchy` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="08ede-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="08ede-129">Remarks</span></span>

<span data-ttu-id="08ede-130">O elemento **FolderShape** é um elemento filho obrigatório do elemento [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="08ede-130">The **FolderShape** element is a required child element of the [FindFolder](findfolder.md) element.</span></span> 
  
<span data-ttu-id="08ede-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="08ede-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="08ede-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08ede-132">Example</span></span>

<span data-ttu-id="08ede-133">O exemplo a seguir de uma solicitação demonstra como localizar todas as pastas localizadas no primeiro nível da pasta caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="08ede-133">The following example of a request demonstrates how to find all folders located in the first level of the Inbox folder.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="08ede-134">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="08ede-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08ede-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="08ede-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="08ede-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="08ede-136">Schema Name</span></span>  <br/> |<span data-ttu-id="08ede-137">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="08ede-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="08ede-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="08ede-138">Validation File</span></span>  <br/> |<span data-ttu-id="08ede-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="08ede-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="08ede-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="08ede-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="08ede-141">False</span><span class="sxs-lookup"><span data-stu-id="08ede-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="08ede-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="08ede-142">See also</span></span>



[<span data-ttu-id="08ede-143">FindFolder</span><span class="sxs-lookup"><span data-stu-id="08ede-143">FindFolder</span></span>](findfolder.md)

