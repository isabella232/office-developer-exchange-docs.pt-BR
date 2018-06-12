---
title: RemoveDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveDelegate
api_type:
- schema
ms.assetid: f21c5171-62e7-47c8-99b1-22e1ff5883bb
description: O elemento de RemoveDelegate define uma solicitação para remover representantes de uma caixa de correio. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 27618b1767c99b26a5f4c06e97a20e063b598d9d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825085"
---
# <a name="removedelegate"></a><span data-ttu-id="9ed0a-104">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="9ed0a-104">RemoveDelegate</span></span>

<span data-ttu-id="9ed0a-105">O elemento de **RemoveDelegate** define uma solicitação para remover representantes de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="9ed0a-105">The **RemoveDelegate** element defines a request to remove delegates from a mailbox.</span></span> <span data-ttu-id="9ed0a-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9ed0a-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<RemoveDelegate>
      <Mailbox/>
   <UserIds/>
</RemoveDelegate>
```

 <span data-ttu-id="9ed0a-107">**RemoveDelegateType**</span><span class="sxs-lookup"><span data-stu-id="9ed0a-107">**RemoveDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9ed0a-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9ed0a-108">Attributes and elements</span></span>

<span data-ttu-id="9ed0a-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9ed0a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ed0a-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="9ed0a-110">Attributes</span></span>

<span data-ttu-id="9ed0a-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9ed0a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9ed0a-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9ed0a-112">Child elements</span></span>

|<span data-ttu-id="9ed0a-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9ed0a-113">**Element**</span></span>|<span data-ttu-id="9ed0a-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9ed0a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ed0a-115">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="9ed0a-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="9ed0a-116">Identifica a caixa de correio do principal.</span><span class="sxs-lookup"><span data-stu-id="9ed0a-116">Identifies the principal's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9ed0a-117">UserIds</span><span class="sxs-lookup"><span data-stu-id="9ed0a-117">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="9ed0a-118">Contém uma matriz de usuários do representante para remover da caixa de correio da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="9ed0a-118">Contains an array of delegate users to remove from a principal's mailbox.</span></span> <span data-ttu-id="9ed0a-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="9ed0a-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9ed0a-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9ed0a-120">Parent elements</span></span>

<span data-ttu-id="9ed0a-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9ed0a-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9ed0a-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="9ed0a-122">Remarks</span></span>

<span data-ttu-id="9ed0a-123">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="9ed0a-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9ed0a-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9ed0a-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ed0a-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="9ed0a-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9ed0a-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9ed0a-126">Schema Name</span></span>  <br/> |<span data-ttu-id="9ed0a-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="9ed0a-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9ed0a-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9ed0a-128">Validation File</span></span>  <br/> |<span data-ttu-id="9ed0a-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9ed0a-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9ed0a-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9ed0a-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="9ed0a-131">False</span><span class="sxs-lookup"><span data-stu-id="9ed0a-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9ed0a-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="9ed0a-132">See also</span></span>



[<span data-ttu-id="9ed0a-133">Operação RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="9ed0a-133">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="9ed0a-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9ed0a-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

