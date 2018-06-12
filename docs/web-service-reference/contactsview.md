---
title: ContactsView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactsView
api_type:
- schema
ms.assetid: 8534f44b-a5af-4a9f-9621-23a3eff5f9d8
description: O elemento de ContactsView define uma pesquisa de itens de contato, com base em nomes para exibição em ordem alfabética.
ms.openlocfilehash: e578eb4dd0042b8c478e883c7fa54d7f2e984229
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751462"
---
# <a name="contactsview"></a><span data-ttu-id="876a6-103">ContactsView</span><span class="sxs-lookup"><span data-stu-id="876a6-103">ContactsView</span></span>

<span data-ttu-id="876a6-104">O elemento de **ContactsView** define uma pesquisa de itens de contato, com base em nomes para exibição em ordem alfabética.</span><span class="sxs-lookup"><span data-stu-id="876a6-104">The **ContactsView** element defines a search for contact items based on alphabetical display names.</span></span> 
  
[<span data-ttu-id="876a6-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="876a6-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="876a6-106">ContactsView</span><span class="sxs-lookup"><span data-stu-id="876a6-106">ContactsView</span></span>](contactsview.md)
  
```xml
<ContactsView MaxEntriesReturned="" InitialName="" FinalName="" />
```

<span data-ttu-id="876a6-107">**ContactsViewType**</span><span class="sxs-lookup"><span data-stu-id="876a6-107">**ContactsViewType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="876a6-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="876a6-108">Attributes and elements</span></span>

<span data-ttu-id="876a6-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="876a6-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="876a6-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="876a6-110">Attributes</span></span>

|<span data-ttu-id="876a6-111">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="876a6-111">**Attribute**</span></span>|<span data-ttu-id="876a6-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="876a6-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="876a6-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="876a6-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="876a6-114">Descreve o número máximo de resultados a serem retornados na resposta [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="876a6-114">Describes the maximum number of results to return in the [FindItem](finditem.md) response.</span></span>  <br/> |
|<span data-ttu-id="876a6-115">**InitialName**</span><span class="sxs-lookup"><span data-stu-id="876a6-115">**InitialName**</span></span> <br/> |<span data-ttu-id="876a6-116">Define o primeiro nome na lista de contatos para retornar na resposta.</span><span class="sxs-lookup"><span data-stu-id="876a6-116">Defines the first name in the contacts list to return in the response.</span></span> <span data-ttu-id="876a6-117">Se o nome inicial especificado não estiver na lista de contatos, o próximo nome em ordem alfabética conforme definido pela cultura contexto será retornado, exceto se o próximo nome vem após **FinalName**.</span><span class="sxs-lookup"><span data-stu-id="876a6-117">If the specified initial name is not in the contacts list, the next alphabetical name as defined by the cultural context will be returned, except if the next name comes after **FinalName**.</span></span> <span data-ttu-id="876a6-118">Se o atributo **InitialName** for omitido, a resposta conterá uma lista de contatos que começa com o primeiro nome na lista de contatos.</span><span class="sxs-lookup"><span data-stu-id="876a6-118">If the **InitialName** attribute is omitted, the response will contain a list of contacts that starts with the first name in the contact list.</span></span> <span data-ttu-id="876a6-119">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="876a6-119">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="876a6-120">**FinalName**</span><span class="sxs-lookup"><span data-stu-id="876a6-120">**FinalName**</span></span> <br/> |<span data-ttu-id="876a6-121">Define o sobrenome na lista de contatos para retornar na resposta.</span><span class="sxs-lookup"><span data-stu-id="876a6-121">Defines the last name in the contacts list to return in the response.</span></span> <span data-ttu-id="876a6-122">Se o atributo **FinalName** for omitido, a resposta conterá todos os contatos subsequentes na ordem de classificação especificado.</span><span class="sxs-lookup"><span data-stu-id="876a6-122">If the **FinalName** attribute is omitted, the response will contain all subsequent contacts in the specified sort order.</span></span> <span data-ttu-id="876a6-123">Se o nome final especificado não estiver na lista de contatos, o próximo nome em ordem alfabética conforme definido pelo contexto de cultura não será excluído.</span><span class="sxs-lookup"><span data-stu-id="876a6-123">If the specified final name is not in the contacts list, the next alphabetical name as defined by the cultural context will be excluded.</span></span>  <br/><br/><span data-ttu-id="876a6-124">Por exemplo, se FinalName = "Name", mas nome não estiver na lista de contatos, contatos que tenham exibem nomes do Nome1 ou nome não serão incluído.</span><span class="sxs-lookup"><span data-stu-id="876a6-124">For example, if FinalName="Name", but Name is not in the contacts list, contacts that have display names of Name1 or NAME will not be included.</span></span>  <br/><br/><span data-ttu-id="876a6-125">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="876a6-125">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="876a6-126">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="876a6-126">Child elements</span></span>

<span data-ttu-id="876a6-127">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="876a6-127">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="876a6-128">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="876a6-128">Parent elements</span></span>

|<span data-ttu-id="876a6-129">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="876a6-129">**Element**</span></span>|<span data-ttu-id="876a6-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="876a6-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="876a6-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="876a6-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="876a6-132">Define uma solicitação para localizar itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="876a6-132">Defines a request to find items in a mailbox.</span></span><br/><br/> <span data-ttu-id="876a6-133">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="876a6-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="876a6-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="876a6-134">Remarks</span></span>

<span data-ttu-id="876a6-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="876a6-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="876a6-136">Example</span><span class="sxs-lookup"><span data-stu-id="876a6-136">Example</span></span>

<span data-ttu-id="876a6-137">O exemplo a seguir de uma solicitação demonstra como localizar os três primeiros contatos começando com o contato que possui o nome de exibição de Kelly Rollin.</span><span class="sxs-lookup"><span data-stu-id="876a6-137">The following example of a request demonstrates how to find the first three contacts starting with the contact that has the display name of Kelly Rollin.</span></span>
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="contacts:DisplayName"/>
        </t:AdditionalProperties>
      </ItemShape>
      <ContactsView MaxEntriesReturned="3" InitialName="Kelly Rollin" />
      <SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="contacts:DisplayName"/>
        </t:FieldOrder>
        </SortOrder>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="contacts"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="876a6-138">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="876a6-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="876a6-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="876a6-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="876a6-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="876a6-140">Schema Name</span></span>  <br/> |<span data-ttu-id="876a6-141">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="876a6-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="876a6-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="876a6-142">Validation File</span></span>  <br/> |<span data-ttu-id="876a6-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="876a6-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="876a6-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="876a6-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="876a6-145">False</span><span class="sxs-lookup"><span data-stu-id="876a6-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="876a6-146">Ver também</span><span class="sxs-lookup"><span data-stu-id="876a6-146">See also</span></span>

- [<span data-ttu-id="876a6-147">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="876a6-147">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="876a6-148">Localizando itens</span><span class="sxs-lookup"><span data-stu-id="876a6-148">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

