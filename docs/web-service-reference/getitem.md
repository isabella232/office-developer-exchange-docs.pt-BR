---
title: GetItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: 769df8eb-9c72-48b5-a49f-82c6b86bc5fc
description: O elemento GetItem define uma solicitação para obter um item de uma caixa de correio no repositório do Exchange.
ms.openlocfilehash: a02403ee84195a41387d5dbe1785ae6d12b47da5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458695"
---
# <a name="getitem"></a><span data-ttu-id="495ec-103">GetItem</span><span class="sxs-lookup"><span data-stu-id="495ec-103">GetItem</span></span>

<span data-ttu-id="495ec-104">O elemento **GetItem** define uma solicitação para obter um item de uma caixa de correio no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="495ec-104">The **GetItem** element defines a request to get an item from a mailbox in the Exchange store.</span></span> 
  
```xml
<GetItem>
   <ItemShape/>
   <ItemIds/>
</GetItem>
```

 <span data-ttu-id="495ec-105">**GetItemType**</span><span class="sxs-lookup"><span data-stu-id="495ec-105">**GetItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="495ec-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="495ec-106">Attributes and elements</span></span>

<span data-ttu-id="495ec-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="495ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="495ec-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="495ec-108">Attributes</span></span>

<span data-ttu-id="495ec-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="495ec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="495ec-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="495ec-110">Child elements</span></span>

|<span data-ttu-id="495ec-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="495ec-111">**Element**</span></span>|<span data-ttu-id="495ec-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="495ec-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="495ec-113">Shape</span><span class="sxs-lookup"><span data-stu-id="495ec-113">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="495ec-114">Identifica as propriedades e o conteúdo do item que serão incluídos em uma resposta **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="495ec-114">Identifies the item properties and content to include in a **GetItem** response.</span></span>  <br/> |
|[<span data-ttu-id="495ec-115">ItemIds</span><span class="sxs-lookup"><span data-stu-id="495ec-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="495ec-116">Contém as identidades exclusivas de itens, itens de ocorrência e itens mestre recorrentes que são usados para obter itens do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="495ec-116">Contains the unique identities of items, occurrence items, and recurring master items that are used to get items from the Exchange store.</span></span> <span data-ttu-id="495ec-117">Estes itens representam contatos, tarefas, mensagens, itens de calendário, solicitações de reunião e outros itens válidos em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="495ec-117">These items represent contacts, tasks, messages, calendar items, meeting requests, and other valid items in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="495ec-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="495ec-118">Parent elements</span></span>

<span data-ttu-id="495ec-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="495ec-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="495ec-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="495ec-120">Remarks</span></span>

<span data-ttu-id="495ec-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="495ec-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="495ec-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="495ec-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="495ec-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="495ec-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="495ec-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="495ec-124">Schema Name</span></span>  <br/> |<span data-ttu-id="495ec-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="495ec-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="495ec-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="495ec-126">Validation File</span></span>  <br/> |<span data-ttu-id="495ec-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="495ec-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="495ec-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="495ec-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="495ec-129">False</span><span class="sxs-lookup"><span data-stu-id="495ec-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="495ec-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="495ec-130">See also</span></span>



[<span data-ttu-id="495ec-131">Operação GetItem</span><span class="sxs-lookup"><span data-stu-id="495ec-131">GetItem operation</span></span>](getitem-operation.md)

