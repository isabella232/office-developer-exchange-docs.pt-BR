---
title: FindFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolder
api_type:
- schema
ms.assetid: b8a59740-d978-454c-9629-a10792385ba0
description: O elemento de FindFolder define uma solicitação para localizar pastas em uma caixa de correio.
ms.openlocfilehash: d41283547c443e38e2e87379a7224df9c89f901d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752269"
---
# <a name="findfolder"></a><span data-ttu-id="c101f-103">FindFolder</span><span class="sxs-lookup"><span data-stu-id="c101f-103">FindFolder</span></span>

<span data-ttu-id="c101f-104">O elemento de **FindFolder** define uma solicitação para localizar pastas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c101f-104">The **FindFolder** element defines a request to find folders in a mailbox.</span></span> 
  
```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <IndexedPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

 <span data-ttu-id="c101f-105">**FindFolderType**</span><span class="sxs-lookup"><span data-stu-id="c101f-105">**FindFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c101f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c101f-106">Attributes and elements</span></span>

<span data-ttu-id="c101f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c101f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c101f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c101f-108">Attributes</span></span>

|<span data-ttu-id="c101f-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="c101f-109">**Attribute**</span></span>|<span data-ttu-id="c101f-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c101f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c101f-111">Passagem</span><span class="sxs-lookup"><span data-stu-id="c101f-111">Traversal</span></span>  <br/> |<span data-ttu-id="c101f-112">Define como uma pesquisa é executada.</span><span class="sxs-lookup"><span data-stu-id="c101f-112">Defines how a search is performed.</span></span> <span data-ttu-id="c101f-113">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="c101f-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="c101f-114">Valores de atributos de passagem</span><span class="sxs-lookup"><span data-stu-id="c101f-114">Traversal attribute values</span></span>

|<span data-ttu-id="c101f-115">**Valor**</span><span class="sxs-lookup"><span data-stu-id="c101f-115">**Value**</span></span>|<span data-ttu-id="c101f-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c101f-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c101f-117">Raso</span><span class="sxs-lookup"><span data-stu-id="c101f-117">Shallow</span></span>  <br/> |<span data-ttu-id="c101f-118">Instrui a operação FindFolder para pesquisar somente a pasta identificada e retornar somente a pasta IDs para itens que não foram excluídos.</span><span class="sxs-lookup"><span data-stu-id="c101f-118">Instructs the FindFolder operation to search only the identified folder and to return only the folder IDs for items that have not been deleted.</span></span> <span data-ttu-id="c101f-119">Isso é chamado uma passagem superficial.</span><span class="sxs-lookup"><span data-stu-id="c101f-119">This is called a shallow traversal.</span></span>  <br/> |
|<span data-ttu-id="c101f-120">Profundo</span><span class="sxs-lookup"><span data-stu-id="c101f-120">Deep</span></span>  <br/> |<span data-ttu-id="c101f-121">Instrui a operação FindFolder para pesquisar em todas as pastas filho da pasta pai identificados e retornar somente a pasta IDs para itens que não foram excluídos.</span><span class="sxs-lookup"><span data-stu-id="c101f-121">Instructs the FindFolder operation to search in all child folders of the identified parent folder and to return only the folder IDs for items that have not been deleted.</span></span> <span data-ttu-id="c101f-122">Isso é chamado um percurso profundo.</span><span class="sxs-lookup"><span data-stu-id="c101f-122">This is called a deep traversal.</span></span>  <br/> |
|<span data-ttu-id="c101f-123">SoftDeleted</span><span class="sxs-lookup"><span data-stu-id="c101f-123">SoftDeleted</span></span>  <br/> |<span data-ttu-id="c101f-124">Instrui a operação FindFolder para realizar uma pesquisa de passagem superficial para itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="c101f-124">Instructs the FindFolder operation to perform a shallow traversal search for deleted items.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c101f-125">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c101f-125">Child elements</span></span>

|<span data-ttu-id="c101f-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c101f-126">**Element**</span></span>|<span data-ttu-id="c101f-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c101f-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c101f-128">FolderShape</span><span class="sxs-lookup"><span data-stu-id="c101f-128">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="c101f-129">Identifica as propriedades de pasta para incluir em uma resposta FindFolder.</span><span class="sxs-lookup"><span data-stu-id="c101f-129">Identifies the folder properties to include in a FindFolder response.</span></span>  <br/> |
|[<span data-ttu-id="c101f-130">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="c101f-130">IndexedPageFolderView</span></span>](indexedpagefolderview.md) <br/> |<span data-ttu-id="c101f-131">Descreve como paginados informações de item são retornados em uma resposta FindFolder.</span><span class="sxs-lookup"><span data-stu-id="c101f-131">Describes how paged item information is returned in a FindFolder response.</span></span> <span data-ttu-id="c101f-132">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="c101f-132">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="c101f-133">FractionalPageFolderView</span><span class="sxs-lookup"><span data-stu-id="c101f-133">FractionalPageFolderView</span></span>](fractionalpagefolderview.md) <br/> |<span data-ttu-id="c101f-134">Descreve o modo de exibição paginado inicia onde e o número máximo de pastas retornados em uma solicitação de FindFolder.</span><span class="sxs-lookup"><span data-stu-id="c101f-134">Describes where the paged view starts and the maximum number of folders returned in a FindFolder request.</span></span> <span data-ttu-id="c101f-135">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="c101f-135">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="c101f-136">Restriction</span><span class="sxs-lookup"><span data-stu-id="c101f-136">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="c101f-137">Define uma restrição ou a consulta que é usada para filtrar as pastas em uma operação FindFolder.</span><span class="sxs-lookup"><span data-stu-id="c101f-137">Defines a restriction or query that is used to filter folders in a FindFolder operation.</span></span> <span data-ttu-id="c101f-138">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="c101f-138">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="c101f-139">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="c101f-139">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="c101f-140">Identifica as pastas para a operação FindFolder pesquisar.</span><span class="sxs-lookup"><span data-stu-id="c101f-140">Identifies folders for the FindFolder operation to search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c101f-141">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c101f-141">Parent elements</span></span>

<span data-ttu-id="c101f-142">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c101f-142">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c101f-143">Comentários</span><span class="sxs-lookup"><span data-stu-id="c101f-143">Remarks</span></span>

<span data-ttu-id="c101f-144">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="c101f-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="c101f-145">Example</span><span class="sxs-lookup"><span data-stu-id="c101f-145">Example</span></span>

<span data-ttu-id="c101f-146">O exemplo a seguir de uma solicitação de FindFolder mostra como uma solicitação para localizar todas as pastas localizadas em uma caixa de entrada de formulário.</span><span class="sxs-lookup"><span data-stu-id="c101f-146">The following example of a FindFolder request shows how to form a request to find all the folders located in an Inbox.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="c101f-147">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c101f-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c101f-148">Namespace</span><span class="sxs-lookup"><span data-stu-id="c101f-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c101f-149">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c101f-149">Schema Name</span></span>  <br/> |<span data-ttu-id="c101f-150">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c101f-150">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c101f-151">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c101f-151">Validation File</span></span>  <br/> |<span data-ttu-id="c101f-152">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c101f-152">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c101f-153">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c101f-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="c101f-154">False</span><span class="sxs-lookup"><span data-stu-id="c101f-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c101f-155">Ver também</span><span class="sxs-lookup"><span data-stu-id="c101f-155">See also</span></span>



[<span data-ttu-id="c101f-156">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="c101f-156">FindFolder operation</span></span>](findfolder-operation.md)

