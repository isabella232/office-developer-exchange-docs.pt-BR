---
title: Getdelegate
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
description: O elemento getdelegate define uma solicitação para obter informações sobre representantes para uma caixa de correio. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: bd7fb55800b51eb2d69184bc4e04cdef3e6b9a89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461027"
---
# <a name="getdelegate"></a><span data-ttu-id="ba09a-104">Getdelegate</span><span class="sxs-lookup"><span data-stu-id="ba09a-104">GetDelegate</span></span>

<span data-ttu-id="ba09a-105">O elemento **Getdelegate** define uma solicitação para obter informações sobre representantes para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ba09a-105">The **GetDelegate** element defines a request to get information about delegates to a mailbox.</span></span> <span data-ttu-id="ba09a-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ba09a-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<GetDelegate IncludePermissions="">
      <Mailbox/>
   <UserIds/>
</GetDelegate>
```

 <span data-ttu-id="ba09a-107">**Getdelegatetype**</span><span class="sxs-lookup"><span data-stu-id="ba09a-107">**GetDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ba09a-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ba09a-108">Attributes and elements</span></span>

<span data-ttu-id="ba09a-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ba09a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba09a-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="ba09a-110">Attributes</span></span>

|<span data-ttu-id="ba09a-111">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="ba09a-111">**Attribute**</span></span>|<span data-ttu-id="ba09a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ba09a-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ba09a-113">**IncludePermissions**</span><span class="sxs-lookup"><span data-stu-id="ba09a-113">**IncludePermissions**</span></span> <br/> |<span data-ttu-id="ba09a-114">Indica se a resposta contém as configurações de permissão para cada usuário delegado.</span><span class="sxs-lookup"><span data-stu-id="ba09a-114">Indicates whether the response contains permission settings for each delegate user.</span></span>  <br/> |
   
#### <a name="includepermissions-attribute-values"></a><span data-ttu-id="ba09a-115">Valores de atributo IncludePermissions</span><span class="sxs-lookup"><span data-stu-id="ba09a-115">IncludePermissions attribute values</span></span>

|<span data-ttu-id="ba09a-116">**Valor**</span><span class="sxs-lookup"><span data-stu-id="ba09a-116">**Value**</span></span>|<span data-ttu-id="ba09a-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ba09a-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ba09a-118">**True**</span><span class="sxs-lookup"><span data-stu-id="ba09a-118">**True**</span></span> <br/> |<span data-ttu-id="ba09a-119">As permissões de usuário delegadas são retornadas além das informações de usuário delegado que são retornadas no elemento [userid](userid.md) .</span><span class="sxs-lookup"><span data-stu-id="ba09a-119">Delegate user permissions are returned in addition to the delegate user information that is returned in the [UserId](userid.md) element.</span></span>  <br/> |
|<span data-ttu-id="ba09a-120">**Falso**</span><span class="sxs-lookup"><span data-stu-id="ba09a-120">**False**</span></span> <br/> |<span data-ttu-id="ba09a-121">As informações de [userid](userid.md) são retornadas.</span><span class="sxs-lookup"><span data-stu-id="ba09a-121">[UserId](userid.md) information is returned.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ba09a-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ba09a-122">Child elements</span></span>

|<span data-ttu-id="ba09a-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ba09a-123">**Element**</span></span>|<span data-ttu-id="ba09a-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ba09a-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ba09a-125">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="ba09a-125">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="ba09a-126">Identifica a caixa de correio da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="ba09a-126">Identifies the principal's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ba09a-127">UserIds</span><span class="sxs-lookup"><span data-stu-id="ba09a-127">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="ba09a-128">Contém uma matriz de usuários delegados para obter da caixa de correio de uma entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="ba09a-128">Contains an array of delegate users to get from a principal's mailbox.</span></span> <span data-ttu-id="ba09a-129">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="ba09a-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ba09a-130">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ba09a-130">Parent elements</span></span>

<span data-ttu-id="ba09a-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ba09a-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ba09a-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="ba09a-132">Remarks</span></span>

<span data-ttu-id="ba09a-133">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="ba09a-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ba09a-134">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ba09a-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ba09a-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="ba09a-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ba09a-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ba09a-136">Schema Name</span></span>  <br/> |<span data-ttu-id="ba09a-137">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ba09a-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ba09a-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ba09a-138">Validation File</span></span>  <br/> |<span data-ttu-id="ba09a-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ba09a-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ba09a-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ba09a-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="ba09a-141">False</span><span class="sxs-lookup"><span data-stu-id="ba09a-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ba09a-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="ba09a-142">See also</span></span>



[<span data-ttu-id="ba09a-143">Operação getdelegate</span><span class="sxs-lookup"><span data-stu-id="ba09a-143">GetDelegate operation</span></span>](getdelegate-operation.md)


- [<span data-ttu-id="ba09a-144">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ba09a-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

