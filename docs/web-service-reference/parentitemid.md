---
title: ParentItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentItemId
api_type:
- schema
ms.assetid: 72dc4391-72db-44d2-85d9-4718d59886a7
description: O elemento ParentItemId identifica o item pai que é vinculado a um anexo associado.
ms.openlocfilehash: 4f3e33da0af2438948313f0e335cd03e076d135a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465741"
---
# <a name="parentitemid"></a><span data-ttu-id="73416-103">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="73416-103">ParentItemId</span></span>

<span data-ttu-id="73416-104">O elemento **ParentItemId** identifica o item pai que é vinculado a um anexo associado.</span><span class="sxs-lookup"><span data-stu-id="73416-104">The **ParentItemId** element identifies the parent item that links to an associated attachment.</span></span> 
  
- [<span data-ttu-id="73416-105">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="73416-105">CreateAttachment</span></span>](createattachment.md)
  
- [<span data-ttu-id="73416-106">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="73416-106">ParentItemId</span></span>](parentitemid.md)
  
```xml
<ParentItemId Id="" ChangeKey="" />
```

<span data-ttu-id="73416-107">**ItemIdtype**</span><span class="sxs-lookup"><span data-stu-id="73416-107">**ItemIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="73416-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="73416-108">Attributes and elements</span></span>

<span data-ttu-id="73416-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="73416-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="73416-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="73416-110">Attributes</span></span>

|<span data-ttu-id="73416-111">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="73416-111">**Attribute**</span></span>|<span data-ttu-id="73416-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="73416-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="73416-113">**Id**</span><span class="sxs-lookup"><span data-stu-id="73416-113">**Id**</span></span> <br/> |<span data-ttu-id="73416-114">Identifica um único item no repositório do Exchange para associar a um anexo.</span><span class="sxs-lookup"><span data-stu-id="73416-114">Identifies a single item in the Exchange store to associate with an attachment.</span></span> <span data-ttu-id="73416-115">Este valor é uma cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="73416-115">This value is a string.</span></span> <span data-ttu-id="73416-116">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="73416-116">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="73416-117">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="73416-117">**ChangeKey**</span></span> <br/> |<span data-ttu-id="73416-118">Identifica uma versão não especificada de um item que é identificada pelo atributo **ID** no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="73416-118">Identifies an unspecified version of an item that is identified by the **Id** attribute in the Exchange store.</span></span> <span data-ttu-id="73416-119">Isso é usado para garantir que um item atual é usado quando é atualizado com um anexo.</span><span class="sxs-lookup"><span data-stu-id="73416-119">This is used to make sure that a current item is used when it is updated with an attachment.</span></span> <span data-ttu-id="73416-120">Este valor é uma cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="73416-120">This value is a string.</span></span> <span data-ttu-id="73416-121">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="73416-121">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="73416-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="73416-122">Child elements</span></span>

<span data-ttu-id="73416-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="73416-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="73416-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="73416-124">Parent elements</span></span>

|<span data-ttu-id="73416-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="73416-125">**Element**</span></span>|<span data-ttu-id="73416-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="73416-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73416-127">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="73416-127">CreateAttachment</span></span>](createattachment.md) <br/> |<span data-ttu-id="73416-128">Define uma solicitação para criar um anexo a um item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="73416-128">Defines a request to create an attachment to an item in a mailbox.</span></span>  <br/> <span data-ttu-id="73416-129">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="73416-129">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateAttachment` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="73416-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="73416-130">Remarks</span></span>

<span data-ttu-id="73416-131">Esse elemento é necessário na [operação CreateAttachment](createattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="73416-131">This element is required in the [CreateAttachment operation](createattachment-operation.md).</span></span> <span data-ttu-id="73416-132">Este elemento é basicamente o mesmo que o elemento [ItemId](itemid.md) .</span><span class="sxs-lookup"><span data-stu-id="73416-132">This element is basically the same as the [ItemId](itemid.md) element.</span></span> 
  
<span data-ttu-id="73416-133">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="73416-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="73416-134">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="73416-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="73416-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="73416-135">Namespace</span></span>  <br/> |[https://schemas.microsoft.com/exchange/services/2006/messages](https://schemas.microsoft.com/exchange/services/2006/messages) <br/> |
|<span data-ttu-id="73416-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="73416-136">Schema Name</span></span>  <br/> |<span data-ttu-id="73416-137">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="73416-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="73416-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="73416-138">Validation File</span></span>  <br/> |<span data-ttu-id="73416-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="73416-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="73416-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="73416-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="73416-141">False</span><span class="sxs-lookup"><span data-stu-id="73416-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="73416-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="73416-142">See also</span></span>

- [<span data-ttu-id="73416-143">Operação CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="73416-143">CreateAttachment operation</span></span>](createattachment-operation.md)

