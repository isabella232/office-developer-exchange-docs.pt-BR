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
description: O elemento FindFolder define uma solicitação para localizar pastas em uma caixa de correio.
ms.openlocfilehash: 248047206a661afe723543e52c51b57847148423
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462574"
---
# <a name="findfolder"></a><span data-ttu-id="77aa4-103">FindFolder</span><span class="sxs-lookup"><span data-stu-id="77aa4-103">FindFolder</span></span>

<span data-ttu-id="77aa4-104">O elemento **FindFolder** define uma solicitação para localizar pastas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="77aa4-104">The **FindFolder** element defines a request to find folders in a mailbox.</span></span> 
  
```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <IndexedPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <FractionalPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

<span data-ttu-id="77aa4-105">**FindFolderType**</span><span class="sxs-lookup"><span data-stu-id="77aa4-105">**FindFolderType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="77aa4-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="77aa4-106">Attributes and elements</span></span>

<span data-ttu-id="77aa4-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="77aa4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="77aa4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="77aa4-108">Attributes</span></span>

|<span data-ttu-id="77aa4-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="77aa4-109">**Attribute**</span></span>|<span data-ttu-id="77aa4-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="77aa4-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="77aa4-111">Passagem</span><span class="sxs-lookup"><span data-stu-id="77aa4-111">Traversal</span></span>  <br/> |<span data-ttu-id="77aa4-112">Define como uma pesquisa é realizada.</span><span class="sxs-lookup"><span data-stu-id="77aa4-112">Defines how a search is performed.</span></span> <span data-ttu-id="77aa4-113">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="77aa4-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="77aa4-114">Valores de atributos de passagem</span><span class="sxs-lookup"><span data-stu-id="77aa4-114">Traversal attribute values</span></span>

|<span data-ttu-id="77aa4-115">**Valor**</span><span class="sxs-lookup"><span data-stu-id="77aa4-115">**Value**</span></span>|<span data-ttu-id="77aa4-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="77aa4-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="77aa4-117">Superficial</span><span class="sxs-lookup"><span data-stu-id="77aa4-117">Shallow</span></span>  <br/> |<span data-ttu-id="77aa4-118">Instrui a operação FindFolder a pesquisar somente a pasta identificada e retornar apenas as IDs de pasta para itens que não foram excluídos.</span><span class="sxs-lookup"><span data-stu-id="77aa4-118">Instructs the FindFolder operation to search only the identified folder and to return only the folder IDs for items that have not been deleted.</span></span> <span data-ttu-id="77aa4-119">Isso é chamado de passagem superficial.</span><span class="sxs-lookup"><span data-stu-id="77aa4-119">This is called a shallow traversal.</span></span>  <br/> |
|<span data-ttu-id="77aa4-120">Detalhadas</span><span class="sxs-lookup"><span data-stu-id="77aa4-120">Deep</span></span>  <br/> |<span data-ttu-id="77aa4-121">Instrui a operação FindFolder para pesquisar em todas as pastas filhas da pasta pai identificada e para retornar apenas as IDs de pasta para itens que não foram excluídos.</span><span class="sxs-lookup"><span data-stu-id="77aa4-121">Instructs the FindFolder operation to search in all child folders of the identified parent folder and to return only the folder IDs for items that have not been deleted.</span></span> <span data-ttu-id="77aa4-122">Isso é chamado de passagem profunda.</span><span class="sxs-lookup"><span data-stu-id="77aa4-122">This is called a deep traversal.</span></span>  <br/> |
|<span data-ttu-id="77aa4-123">SoftDeleted</span><span class="sxs-lookup"><span data-stu-id="77aa4-123">SoftDeleted</span></span>  <br/> |<span data-ttu-id="77aa4-124">Instrui a operação FindFolder a realizar uma pesquisa de passagem superficial para itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="77aa4-124">Instructs the FindFolder operation to perform a shallow traversal search for deleted items.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="77aa4-125">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="77aa4-125">Child elements</span></span>

|<span data-ttu-id="77aa4-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="77aa4-126">**Element**</span></span>|<span data-ttu-id="77aa4-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="77aa4-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77aa4-128">FolderShape</span><span class="sxs-lookup"><span data-stu-id="77aa4-128">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="77aa4-129">Identifica as propriedades da pasta a serem incluídas em uma resposta FindFolder.</span><span class="sxs-lookup"><span data-stu-id="77aa4-129">Identifies the folder properties to include in a FindFolder response.</span></span>  <br/> |
|[<span data-ttu-id="77aa4-130">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="77aa4-130">IndexedPageFolderView</span></span>](indexedpagefolderview.md) <br/> |<span data-ttu-id="77aa4-131">Descreve como as informações de item paginado são retornadas em uma resposta FindFolder.</span><span class="sxs-lookup"><span data-stu-id="77aa4-131">Describes how paged item information is returned in a FindFolder response.</span></span> <span data-ttu-id="77aa4-132">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="77aa4-132">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="77aa4-133">FractionalPageFolderView</span><span class="sxs-lookup"><span data-stu-id="77aa4-133">FractionalPageFolderView</span></span>](fractionalpagefolderview.md) <br/> |<span data-ttu-id="77aa4-134">Descreve onde o modo de exibição paginado começa e o número máximo de pastas retornadas em uma solicitação FindFolder.</span><span class="sxs-lookup"><span data-stu-id="77aa4-134">Describes where the paged view starts and the maximum number of folders returned in a FindFolder request.</span></span> <span data-ttu-id="77aa4-135">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="77aa4-135">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="77aa4-136">Restriction</span><span class="sxs-lookup"><span data-stu-id="77aa4-136">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="77aa4-137">Define uma restrição ou consulta usada para filtrar pastas em uma operação FindFolder.</span><span class="sxs-lookup"><span data-stu-id="77aa4-137">Defines a restriction or query that is used to filter folders in a FindFolder operation.</span></span> <span data-ttu-id="77aa4-138">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="77aa4-138">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="77aa4-139">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="77aa4-139">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="77aa4-140">Identifica pastas para a operação FindFolder a ser pesquisada.</span><span class="sxs-lookup"><span data-stu-id="77aa4-140">Identifies folders for the FindFolder operation to search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="77aa4-141">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="77aa4-141">Parent elements</span></span>

<span data-ttu-id="77aa4-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="77aa4-142">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="77aa4-143">Comentários</span><span class="sxs-lookup"><span data-stu-id="77aa4-143">Remarks</span></span>

<span data-ttu-id="77aa4-144">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="77aa4-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="77aa4-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77aa4-145">Example</span></span>

<span data-ttu-id="77aa4-146">O exemplo a seguir de uma solicitação FindFolder mostra como formar uma solicitação para localizar todas as pastas localizadas em uma caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="77aa4-146">The following example of a FindFolder request shows how to form a request to find all the folders located in an Inbox.</span></span>
  
```xml
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

## <a name="element-information"></a><span data-ttu-id="77aa4-147">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="77aa4-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="77aa4-148">Namespace</span><span class="sxs-lookup"><span data-stu-id="77aa4-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="77aa4-149">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="77aa4-149">Schema Name</span></span>  <br/> |<span data-ttu-id="77aa4-150">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="77aa4-150">Messages schema</span></span>  <br/> |
|<span data-ttu-id="77aa4-151">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="77aa4-151">Validation File</span></span>  <br/> |<span data-ttu-id="77aa4-152">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="77aa4-152">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="77aa4-153">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="77aa4-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="77aa4-154">False</span><span class="sxs-lookup"><span data-stu-id="77aa4-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="77aa4-155">Confira também</span><span class="sxs-lookup"><span data-stu-id="77aa4-155">See also</span></span>

- [<span data-ttu-id="77aa4-156">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="77aa4-156">FindFolder operation</span></span>](findfolder-operation.md)

