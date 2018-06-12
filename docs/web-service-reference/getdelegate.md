---
title: GetDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetDelegate
api_type:
- schema
ms.assetid: 6d5efe59-596f-46f8-bdc6-ca9cded9bb8e
description: O elemento de GetDelegate define uma solicitação para obter mais informações sobre os representantes para uma caixa de correio. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: e31d6bd4f4387094beb467fcc4dff31ca7ec5d62
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752455"
---
# <a name="getdelegate"></a><span data-ttu-id="d8f26-104">GetDelegate</span><span class="sxs-lookup"><span data-stu-id="d8f26-104">GetDelegate</span></span>

<span data-ttu-id="d8f26-105">O elemento de **GetDelegate** define uma solicitação para obter mais informações sobre os representantes para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d8f26-105">The **GetDelegate** element defines a request to get information about delegates to a mailbox.</span></span> <span data-ttu-id="d8f26-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d8f26-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<GetDelegate IncludePermissions="">
      <Mailbox/>
   <UserIds/>
</GetDelegate>
```

 <span data-ttu-id="d8f26-107">**GetDelegateType**</span><span class="sxs-lookup"><span data-stu-id="d8f26-107">**GetDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8f26-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d8f26-108">Attributes and elements</span></span>

<span data-ttu-id="d8f26-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d8f26-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8f26-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="d8f26-110">Attributes</span></span>

|<span data-ttu-id="d8f26-111">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="d8f26-111">**Attribute**</span></span>|<span data-ttu-id="d8f26-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d8f26-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d8f26-113">**IncludePermissions**</span><span class="sxs-lookup"><span data-stu-id="d8f26-113">**IncludePermissions**</span></span> <br/> |<span data-ttu-id="d8f26-114">Indica se a resposta contém configurações de permissão para cada usuário delegado.</span><span class="sxs-lookup"><span data-stu-id="d8f26-114">Indicates whether the response contains permission settings for each delegate user.</span></span>  <br/> |
   
#### <a name="includepermissions-attribute-values"></a><span data-ttu-id="d8f26-115">Valores de atributo IncludePermissions</span><span class="sxs-lookup"><span data-stu-id="d8f26-115">IncludePermissions attribute values</span></span>

|<span data-ttu-id="d8f26-116">**Valor**</span><span class="sxs-lookup"><span data-stu-id="d8f26-116">**Value**</span></span>|<span data-ttu-id="d8f26-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d8f26-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d8f26-118">**True**</span><span class="sxs-lookup"><span data-stu-id="d8f26-118">**True**</span></span> <br/> |<span data-ttu-id="d8f26-119">Delega permissões são retornadas além das informações do usuário delegado são retornadas no elemento [UserId](userid.md) do usuário.</span><span class="sxs-lookup"><span data-stu-id="d8f26-119">Delegate user permissions are returned in addition to the delegate user information that is returned in the [UserId](userid.md) element.</span></span>  <br/> |
|<span data-ttu-id="d8f26-120">**False**</span><span class="sxs-lookup"><span data-stu-id="d8f26-120">**False**</span></span> <br/> |<span data-ttu-id="d8f26-121">[UserId](userid.md) informação é retornada.</span><span class="sxs-lookup"><span data-stu-id="d8f26-121">[UserId](userid.md) information is returned.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d8f26-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d8f26-122">Child elements</span></span>

|<span data-ttu-id="d8f26-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d8f26-123">**Element**</span></span>|<span data-ttu-id="d8f26-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d8f26-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8f26-125">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="d8f26-125">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="d8f26-126">Identifica a caixa de correio do principal.</span><span class="sxs-lookup"><span data-stu-id="d8f26-126">Identifies the principal's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d8f26-127">UserIds</span><span class="sxs-lookup"><span data-stu-id="d8f26-127">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="d8f26-128">Contém uma matriz de representante aos usuários obter da caixa de correio da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="d8f26-128">Contains an array of delegate users to get from a principal's mailbox.</span></span> <span data-ttu-id="d8f26-129">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d8f26-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d8f26-130">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d8f26-130">Parent elements</span></span>

<span data-ttu-id="d8f26-131">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d8f26-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d8f26-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="d8f26-132">Remarks</span></span>

<span data-ttu-id="d8f26-133">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="d8f26-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8f26-134">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d8f26-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8f26-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="d8f26-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d8f26-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d8f26-136">Schema Name</span></span>  <br/> |<span data-ttu-id="d8f26-137">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d8f26-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d8f26-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d8f26-138">Validation File</span></span>  <br/> |<span data-ttu-id="d8f26-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d8f26-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d8f26-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d8f26-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="d8f26-141">False</span><span class="sxs-lookup"><span data-stu-id="d8f26-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d8f26-142">Ver também</span><span class="sxs-lookup"><span data-stu-id="d8f26-142">See also</span></span>



[<span data-ttu-id="d8f26-143">Operação GetDelegate</span><span class="sxs-lookup"><span data-stu-id="d8f26-143">GetDelegate operation</span></span>](getdelegate-operation.md)


- [<span data-ttu-id="d8f26-144">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d8f26-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

