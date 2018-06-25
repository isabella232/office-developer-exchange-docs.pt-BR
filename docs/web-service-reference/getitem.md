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
description: O elemento de GetItem define uma solicitação para obter um item de uma caixa de correio no armazenamento do Exchange.
ms.openlocfilehash: 39db141bad62c34bec5ae6a937ba94c2d1288090
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752548"
---
# <a name="getitem"></a><span data-ttu-id="269fb-103">GetItem</span><span class="sxs-lookup"><span data-stu-id="269fb-103">GetItem</span></span>

<span data-ttu-id="269fb-104">O elemento de **GetItem** define uma solicitação para obter um item de uma caixa de correio no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="269fb-104">The **GetItem** element defines a request to get an item from a mailbox in the Exchange store.</span></span> 
  
```xml
<GetItem>
   <ItemShape/>
   <ItemIds/>
</GetItem>
```

 <span data-ttu-id="269fb-105">**GetItemType**</span><span class="sxs-lookup"><span data-stu-id="269fb-105">**GetItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="269fb-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="269fb-106">Attributes and elements</span></span>

<span data-ttu-id="269fb-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="269fb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="269fb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="269fb-108">Attributes</span></span>

<span data-ttu-id="269fb-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="269fb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="269fb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="269fb-110">Child elements</span></span>

|<span data-ttu-id="269fb-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="269fb-111">**Element**</span></span>|<span data-ttu-id="269fb-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="269fb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="269fb-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="269fb-113">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="269fb-114">Identifica o conteúdo a ser incluído em uma resposta **GetItem** e propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="269fb-114">Identifies the item properties and content to include in a **GetItem** response.</span></span>  <br/> |
|[<span data-ttu-id="269fb-115">ItemIds</span><span class="sxs-lookup"><span data-stu-id="269fb-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="269fb-116">Contém as identidades exclusivas dos itens, itens de ocorrência e itens recorrentes de mestres que são usados para obter os itens do armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="269fb-116">Contains the unique identities of items, occurrence items, and recurring master items that are used to get items from the Exchange store.</span></span> <span data-ttu-id="269fb-117">Esses itens representam contatos, tarefas, mensagens, itens de calendário, solicitações de reunião e outros itens válidos em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="269fb-117">These items represent contacts, tasks, messages, calendar items, meeting requests, and other valid items in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="269fb-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="269fb-118">Parent elements</span></span>

<span data-ttu-id="269fb-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="269fb-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="269fb-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="269fb-120">Remarks</span></span>

<span data-ttu-id="269fb-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="269fb-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="269fb-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="269fb-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="269fb-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="269fb-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="269fb-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="269fb-124">Schema Name</span></span>  <br/> |<span data-ttu-id="269fb-125">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="269fb-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="269fb-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="269fb-126">Validation File</span></span>  <br/> |<span data-ttu-id="269fb-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="269fb-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="269fb-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="269fb-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="269fb-129">False</span><span class="sxs-lookup"><span data-stu-id="269fb-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="269fb-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="269fb-130">See also</span></span>



[<span data-ttu-id="269fb-131">Operação GetItem</span><span class="sxs-lookup"><span data-stu-id="269fb-131">GetItem operation</span></span>](getitem-operation.md)

